---
title: "Machine Learning Engineer"
description: "MutualArt"
dateString: September 2023 - June 2024
draft: false
tags: ["PyTorch", "LoRA", "Quantization", "GPU Inference", "AWS", "Qdrant", "Computer Vision"]
showToc: false
weight: 302
unlisted: true
build:
  list: false
  render: true
---

## Role Overview

Built GPU-backed inference services and ML-powered features for an art market intelligence platform serving thousands of users worldwide.

## Key Achievements

- **Vision-Language Model Fine-Tuning**: Fine-tuned IDEFICS-2 (8B VLM) with PyTorch and LoRA (rank-16 decomposition across attention layers, ~20M trainable parameters, 0.25% of total), using 4-bit NF4 quantization via BitsAndBytes and flash attention, reducing VRAM requirements by ~75% while maintaining accuracy

- **GPU Inference Microservice**: Developed a production microservice on GPU servers consuming AWS SQS events for automated description generation and validation with BLIP Image-Text Matching, improving content discoverability by 80% with 99.5% uptime

- **Multimodal Recommendation Pipeline**: Engineered an embedding pipeline fusing text (Sentence Transformers), categorical, and numerical features into unified 424-dim vectors; deployed on AWS ECS/Fargate with auto-scaling, processing 80,000+ artworks weekly; combined Qdrant ANN retrieval with OpenSearch gaussian-decay scoring via Reciprocal Rank Fusion for real-time "similar artworks" recommendations

- **Duplicate Detection**: Built a parallel image-processing pipeline with two-stage ORB (keypoint) + SSIM (structural) matching and Union-Find grouping, improving customer conversion by 200%

- **Service Architecture**: Separated the lightweight recommendation service from the compute-heavy embedding service for independent scaling and cost efficiency

## Technologies Used

- **Languages**: Python, SQL
- **ML**: PyTorch, LoRA, BitsAndBytes (NF4), Flash Attention, Sentence Transformers, BLIP
- **Infrastructure**: AWS ECS/ECR/Fargate/SQS, Docker, GPU servers
- **Databases**: Qdrant, OpenSearch
- **Domains**: VLM Fine-Tuning, GPU Inference, Recommendation Systems, Computer Vision

## Impact

Cut fine-tuning VRAM requirements by ~75% through quantization and parameter-efficient training, ran GPU inference services at 99.5% uptime, and shipped recommendation and duplicate-detection features that improved content discoverability by 80% and customer conversion by 200%.
