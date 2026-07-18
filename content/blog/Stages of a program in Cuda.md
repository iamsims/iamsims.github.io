---
title: Stages of a program in Cuda
date: 2026-07-17T18:58:45-05:00
draft: false
share: true
tags:
summary: ""
---


**1. Kernel Launched**  
The CPU pushes a grid of threads into the GPU's work queue by calling `kernel<<<gridDim, blockDim>>>(...)`. The chip-level global scheduler (Nvidia calls it the GigaThread Engine) then distributes blocks to SMs based on each SM's available capacity. This is a rolling assignment: as SMs free up space, they get handed the next block, so the whole grid doesn't need to be planned out beforehand.

**2. Resident/Active Warps**  
When an SM has enough free registers, shared memory, thread slots, and a free block slot, the global scheduler admits a block onto it, and the block becomes **resident** on that SM. The block is then split into warps (the actual unit of execution on a GPU), and each warp is assigned to one of the SM's warp schedulers in a round robin fashion. These are now called **resident warps**.

**3. Eligible/Stalled Warps**  
Each of the resident warps in the pool maintains a flag that classifies it as either **eligible** or **stalled**. Modern SMs typically have 4 warp schedulers, one per processing block (sub-partition) of the SM. Each cycle, a scheduler picks one eligible warp and issues its next instruction to its corresponding processing block. Since a processing block has a single instruction fetch/dispatch unit, all 32 threads in that warp execute the same instruction together, in lockstep. This is what gives a warp its **SIMT execution model**. A warp goes stalled when its next instruction depends on something long-latency like a memory fetch, a `__syncthreads()` barrier, or an unresolved data dependency. When the memory result comes back, that warp's flag flips back to eligible at that moment. 

**4. Warp Retirement**  
When all of a warp's instructions finish executing, it **retires**, so it's removed from its scheduler's schedulable pool and never gets picked again. Its registers and thread slots, however, are _not_ freed at this point. 

**5. Block Retirement**  
Once every warp in a block has retired, the block itself retires, and only then, its resources - registers, shared memory, thread slot, and block slot are released back to the SM. This frees up space for another block from the grid, and the chip-level scheduler immediately tries to admit a new pending block into the space that just opened up.

**6. Grid Complete**  
Once every block in the grid has been assigned, executed, and retired, the kernel call returns control to the host (CPU) asynchronously, unless the host explicitly synchronizes.



![Pasted image 20260717171814.png](/blog/Pasted%20image%2020260717171814.png)





