---
title: "Graduate Research Assistant"
description: "NASA IMPACT"
dateString: August 2024 - Present
draft: false
tags: ["Python", "FastAPI", "Model Serving", "LLM Agents", "MCP", "RAG", "Redis", "PyTorch"]
showToc: false
weight: 301
unlisted: true
build:
  list: false
  render: true
---

## Role Overview

Contributing to NASA's Accelerated Knowledge Discovery project, building the model-serving infrastructure and ML pipelines behind a deep research LLM agent with human-in-the-loop guidance for scientific exploration.

## Key Achievements

- **Multi-Model Inference Service**: Owned end-to-end design and deployment of a scalable inference service in Python and FastAPI, serving multiple ML models through a single endpoint with dynamic resource management; Redis-based distributed task queuing reduced API response latency by 40%

- **Guardrails System**: Designed a two-level guardrails system (IBM Granite Guardian served via local Ollama inference as a first-pass filter, followed by a dynamic Risk Agent), achieving ~80% cost reduction over single-model approaches

- **Model Fine-Tuning & Evaluation**: Fine-tuned and evaluated classifiers (Indus, ModernBERT, BERT, FastText) on large scientific corpora, reaching 98% precision on multi-label division tagging and 96% recall on single-label indexing, with conformal prediction (α = 0.05) confidence filtering to reduce false negatives across temporally separated validation sets

- **Agentic AI**: Architected multi-agent workflows for NASA's Deep Research Agent, including LLM orchestration, multi-rubric evaluation, self-analysis for autonomous research synthesis, and RAG-based agents for code, data, and gap search; built MCP tools and servers with FastMCP exposing NASA's Science Discovery Engine

- **Agent Evaluation**: Designed benchmark evaluations for agent architectures using synthetic datasets and A/B testing across configurations (tools, web search, refined prompts), and benchmarked IBM Granite Guardian models against dynamically generated risk criteria

- **Data Pipelines**: Built production data pipelines with custom web resolvers and scrapers, improving data acquisition throughput by 3x

## Technologies Used

- **Languages**: Python
- **Frameworks**: FastAPI, PyTorch, Hugging Face Transformers
- **ML/NLP**: Indus, ModernBERT, BERT, FastText, Conformal Prediction, Active Learning
- **GenAI**: MCP, FastMCP, Ollama, OpenAI Agent SDK, RAG
- **Infrastructure**: Redis, Docker
- **Domains**: Model Serving, LLM Agents, Scientific Text Analysis

## Impact

Cut inference API latency by 40% and guardrails cost by ~80% while serving multiple models under tight resource constraints. Automated classification pipelines (98% precision / 96% recall) freed NASA scientists from manual curation, and the Deep Research Agent infrastructure now powers autonomous scientific knowledge discovery.
