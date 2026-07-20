---
title: "Projects"
description: ""
---

<!-- <div class="projects-intro">
<h2>Project Showcase</h2>
<p>Here's a collection of my personal and professional development work, demonstrating my skills in various technologies and frameworks. Each project includes live demos, source code, and detailed technical information.</p>
</div> -->

<div class="projects-grid">

<div class="project-card">
<h3>CUDA Kernels Suite</h3>
<div class="project-meta">
<span class="status">Work in Progress</span>
<span class="tech">CUDA C++ • Nsight Systems/Compute • PyTorch</span>
</div>
<p class="project-description">
A from-scratch suite of GPU kernels (vector add, tiled matrix multiplication, reduction, softmax, and attention) built to understand GPU performance from the hardware up. Every kernel is profiled with Nsight Systems/Compute and benchmarked head-to-head against cuBLAS and PyTorch using CUDA-event timing with warmup and median-of-many-iterations methodology.
</p>
<div class="project-features">
<ul>
<li>Hand-written CUDA kernels with standalone <code>nvcc</code> builds and self-tests</li>
<li>Benchmark harness plotting GFLOPS vs problem size against cuBLAS/PyTorch baselines</li>
<li>Profiling-driven optimization: memory coalescing, shared-memory tiling, occupancy analysis</li>
<li>In progress: full benchmark comparison table and per-kernel optimization writeups; next up: FlashAttention-style fused attention and KV caching</li>
</ul>
</div>
<div class="project-links">
<a href="https://github.com/iamsims/cuda-kernels-suite" class="source-code" target="_blank">View Source</a>
<a href="/blog/stages-of-a-program-in-cuda/" class="external-link">Related blog post →</a>
</div>
</div>

<div class="project-card">
<h3>Production Lifecycle Management for LLM Classifiers</h3>
<div class="project-meta">
<span class="status">MS Thesis</span>
<span class="tech">Python • PyTorch • HuggingFace • EvidentlyAI</span>
</div>
<p class="project-description">
An MLOps framework for keeping LLM classifiers reliable after deployment, treating the model not as a one-off artifact but as a system that must be monitored, evaluated, and retrained as the world drifts away from its training data.
</p>
<div class="project-features">
<ul>
<li>Production monitoring and data drift detection using statistical tests</li>
<li>Active learning strategies to select the highest-value samples for relabeling</li>
<li>Incremental fine-tuning pipelines for continuous model updates</li>
</ul>
</div>
<div class="project-links">
<a href="https://github.com/iamsims/thesis_code" class="source-code" target="_blank">View Source</a>
<span class="coming-soon">Repo going public soon</span>
</div>
</div>

<div class="project-card">
<h3>RAGstoRiches: Agentic Financial RAG System</h3>
<div class="project-meta">
<span class="status">Live</span>
<span class="tech">Python • FastAPI • React • Qdrant • FastMCP</span>
</div>
<p class="project-description">
An agentic RAG system for financial data that lets an LLM agent combine semantic retrieval with structured SQL analysis: SQL exposed as a FastMCP tool server, Qdrant Cloud for vector search, Supabase for authentication, and Databricks-hosted Postgres.
</p>
<div class="project-features">
<ul>
<li>Agentic tool use: SQL served to the agent as a FastMCP tool server</li>
<li>Qdrant Cloud vector database for semantic retrieval</li>
<li>FastAPI backend with a React/TypeScript frontend, hosted on Hugging Face Spaces</li>
</ul>
</div>
<div class="project-links">
<a href="https://github.com/AwaleSajil/rags_to_riches" class="source-code" target="_blank">View Source</a>
</div>
</div>

</div>

<style>
.projects-intro {
    text-align: center;
    margin-bottom: 3rem;
    padding: 2rem;
    background: var(--theme-bg);
    border-radius: 10px;
}

.projects-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
    gap: 2rem;
    margin-top: 2rem;
}

.project-card {
    background: var(--code-bg);
    border-radius: 12px;
    padding: 2rem;
    border: 1px solid var(--border);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    height: fit-content;
}

.project-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 25px rgba(0,0,0,0.15);
}

.project-card h3 {
    margin-bottom: 0.75rem;
    font-size: 1.25rem;
    line-height: 1.3;
    color: var(--primary);
}

.project-meta {
    display: flex;
    align-items: center;
    gap: 0.75rem;
    flex-wrap: wrap;
    margin-bottom: 1rem;
    font-size: 0.85rem;
}

.status {
    white-space: nowrap;
    padding: 0.15rem 0.6rem;
    border-radius: 4px;
    font-weight: 500;
    font-size: 0.75rem;
}

.project-meta .status { background: var(--theme-bg); color: var(--primary); border: 1px solid var(--border); }

.tech {
    color: var(--secondary);
}

.project-description {
    line-height: 1.6;
    margin-bottom: 1.5rem;
    color: var(--content);
}

.project-features ul {
    margin: 1rem 0;
    padding-left: 1.5rem;
}

.project-features li {
    margin-bottom: 0.5rem;
    color: var(--content);
}

.project-links {
    display: flex;
    gap: 1rem;
    flex-wrap: wrap;
    align-items: center;
    margin-top: 1.5rem;
}

.read-more {
    background: var(--secondary);
    color: white;
    padding: 0.5rem 1rem;
    border-radius: 6px;
    text-decoration: none;
    font-weight: 500;
    transition: opacity 0.3s;
}

.read-more:hover {
    opacity: 0.9;
}

.live-demo {
    background: var(--primary);
    color: white;
    padding: 0.5rem 1rem;
    border-radius: 6px;
    text-decoration: none;
    font-weight: 500;
    transition: opacity 0.3s;
}

.live-demo:hover {
    opacity: 0.9;
}

.source-code {
    border: 1px solid var(--border);
    color: var(--primary);
    padding: 0.5rem 1rem;
    border-radius: 6px;
    text-decoration: none;
    transition: background 0.3s;
}

.source-code:hover {
    background: var(--theme-bg);
}

.external-link {
    color: var(--secondary);
    text-decoration: none;
    font-size: 0.9rem;
}

.external-link:hover {
    color: var(--primary);
}

.coming-soon, .planning, .research {
    color: var(--secondary);
    font-style: italic;
    font-size: 0.9rem;
}

@media (max-width: 768px) {
    .projects-grid {
        grid-template-columns: 1fr;
        gap: 1.5rem;
    }

    .project-card {
        padding: 1.5rem;
    }

    .project-meta {
        flex-direction: column;
        gap: 0.5rem;
    }

    .project-links {
        flex-direction: column;
        align-items: flex-start;
        gap: 0.75rem;
    }
}
</style>