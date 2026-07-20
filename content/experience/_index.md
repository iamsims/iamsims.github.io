---
title: "Professional Experience"
description: "My professional journey across ML systems, agentic AI, and production systems"
---

<!-- <div class="experience-intro">
<h2>Professional Journey</h2>
<p>Here's a comprehensive overview of my professional experience, showcasing my growth as a developer and the diverse projects I've contributed to across different organizations and technologies.</p>
</div> -->

<div class="experience-timeline">

<div class="experience-card current">
<div class="experience-header">
<h3>Graduate Research Assistant</h3>
<div class="company-info">
<span class="company">NASA IMPACT</span>
<span class="duration">August 2024 - Present</span>
</div>
</div>
<span class="status current-role">Current Role</span>
<p class="experience-description">
Contributing to NASA's Accelerated Knowledge Discovery project, building the model-serving infrastructure and ML pipelines behind a deep research LLM agent with human-in-the-loop guidance for scientific exploration.
</p>
<div class="achievements">
<h4>Key Achievements:</h4>
<ul>
<li>Owned end-to-end design and deployment of a scalable multi-model inference service in Python and FastAPI, serving multiple ML models through a single endpoint with dynamic resource management; Redis-based distributed task queuing reduced API response latency by 40%</li>
<li>Designed a two-level guardrails system (IBM Granite Guardian served via local Ollama inference as a first-pass filter, followed by a dynamic Risk Agent), achieving ~80% cost reduction over single-model approaches</li>
<li>Fine-tuned and evaluated classifiers (Indus, ModernBERT, BERT, FastText) on large scientific corpora, reaching 98% precision on multi-label division tagging and 96% recall on single-label indexing, with conformal prediction (α = 0.05) confidence filtering to reduce false negatives</li>
<li>Architected multi-agent workflows for NASA's Deep Research Agent (LLM orchestration, multi-rubric evaluation, and RAG-based agents for code, data, and gap search) and built MCP tools and servers with FastMCP exposing NASA's Science Discovery Engine</li>
<li>Designed benchmark evaluations for agent architectures using synthetic datasets and A/B testing across configurations (tools, web search, refined prompts), and benchmarked IBM Granite Guardian models against dynamically generated risk criteria</li>
<li>Built production data pipelines with custom web resolvers and scrapers, improving data acquisition throughput by 3x</li>
</ul>
</div>
<div class="tech-stack">
<span class="tech-tag">Python</span>
<span class="tech-tag">FastAPI</span>
<span class="tech-tag">Model Serving</span>
<span class="tech-tag">Distributed Systems</span>
<span class="tech-tag">Redis</span>
<span class="tech-tag">Ollama</span>
<span class="tech-tag">LLM Agents</span>
<span class="tech-tag">MCP</span>
<span class="tech-tag">RAG</span>
<span class="tech-tag">PyTorch</span>
</div>
<div class="experience-links">
<a href="https://impact.earthdata.nasa.gov" class="company-link" target="_blank">NASA IMPACT</a>
</div>
</div>

<div class="experience-card">
<div class="experience-header">
<h3>Machine Learning Engineer</h3>
<div class="company-info">
<span class="company">MutualArt</span>
<span class="duration">September 2023 - June 2024</span>
</div>
</div>
<p class="experience-description">
Built GPU-backed inference services and ML-powered features for an art market intelligence platform serving thousands of users.
</p>
<div class="achievements">
<h4>Key Achievements:</h4>
<ul>
<li>Fine-tuned IDEFICS-2, an 8B vision-language model, with LoRA (rank-16, ~20M trainable parameters, 0.25% of total) and 4-bit NF4 quantization via BitsAndBytes with flash attention, reducing VRAM requirements by ~75% while maintaining accuracy</li>
<li>Developed a production microservice on GPU servers consuming AWS SQS events for automated description generation and validation with BLIP Image-Text Matching, improving content discoverability by 80% while maintaining 99.5% uptime</li>
<li>Engineered a multimodal embedding pipeline fusing text, categorical, and numerical features into unified 424-dim vectors; deployed as containerized services on AWS ECS/Fargate processing 80,000+ artworks weekly, with Qdrant ANN retrieval and OpenSearch scoring combined via Reciprocal Rank Fusion for real-time recommendations</li>
<li>Built a parallel image-processing pipeline for artwork duplicate detection using two-stage ORB + SSIM matching with Union-Find grouping, improving customer conversion by 200%</li>
<li>Separated the lightweight recommendation service (Qdrant and OpenSearch lookups) from the compute-heavy embedding service (Sentence Transformer inference) for independent scaling and cost efficiency</li>
</ul>
</div>
<div class="tech-stack">
<span class="tech-tag">PyTorch</span>
<span class="tech-tag">LoRA</span>
<span class="tech-tag">Quantization</span>
<span class="tech-tag">GPU Inference</span>
<span class="tech-tag">AWS ECS/SQS</span>
<span class="tech-tag">Qdrant</span>
<span class="tech-tag">Computer Vision</span>
</div>
<div class="experience-links">
<a href="https://www.mutualart.com" class="company-link" target="_blank">MutualArt</a>
</div>
</div>

<div class="experience-card">
<div class="experience-header">
<h3>Associate Software Engineer</h3>
<div class="company-info">
<span class="company">Sireto Technology</span>
<span class="duration">September 2022 - September 2023</span>
</div>
</div>
<p class="experience-description">
Developed KuberIDE, a web-based IDE for Cardano developers within a microservices architecture. Led backend development focusing on authentication, access management, and deployment optimization.
</p>
<div class="achievements">
<h4>Key Achievements:</h4>
<ul>
<li>Led development of KuberIDE, a web-based IDE (ReactJS, FastAPI) within a microservices architecture serving 500+ developers, reducing environment setup time from hours to minutes</li>
<li>Designed and implemented backend authentication, access management, and session handling using OAuth 2.0 cookies for browser-based access and API keys for secure multi-tenant direct access</li>
<li>Built an HTTPS gateway to in-house microservices and a WebSocket proxy providing real-time Haskell IntelliSense via the Haskell Language Server, increasing platform adoption by 300%</li>
<li>Optimized deployment with Docker multi-stage builds (40% image size reduction), Pytest automated testing (80% coverage), and GitHub Actions CI/CD pipelines</li>
<li>Mentored 2 junior developers on API design patterns and testing best practices through code reviews and pair programming</li>
</ul>
</div>
<div class="tech-stack">
<span class="tech-tag">Python</span>
<span class="tech-tag">FastAPI</span>
<span class="tech-tag">ReactJS</span>
<span class="tech-tag">Docker</span>
<span class="tech-tag">CI/CD</span>
<span class="tech-tag">OAuth</span>
<span class="tech-tag">WebSocket</span>
</div>
<div class="experience-links">
<a href="https://sireto.com" class="company-link" target="_blank">Sireto Technology</a>
</div>
</div>

<div class="experience-card">
<div class="experience-header">
<h3>Solutions Engineer Intern</h3>
<div class="company-info">
<span class="company">Logpoint</span>
<span class="duration">January 2022 - August 2022</span>
</div>
</div>
<span class="status internship">Internship</span>
<p class="experience-description">
Focused on Linux system administration, performance optimization, and automation. Gained extensive experience in system monitoring, troubleshooting, and scripting for enterprise-level infrastructure.
</p>
<div class="achievements">
<h4>Key Achievements:</h4>
<ul>
<li>Diagnosed and resolved critical incidents on enterprise Linux systems, monitoring and tuning for performance and reliability</li>
<li>Automated recurring operations with shell scripting, reducing manual intervention across the infrastructure</li>
</ul>
</div>
<div class="tech-stack">
<span class="tech-tag">Linux</span>
<span class="tech-tag">Shell Scripting</span>
<span class="tech-tag">System Administration</span>
<span class="tech-tag">Performance Optimization</span>
</div>
<div class="experience-links">
<a href="https://www.logpoint.com" class="company-link" target="_blank">Logpoint</a>
</div>
</div>

<div class="experience-card">
<div class="experience-header">
<h3>AI Research Intern</h3>
<div class="company-info">
<span class="company">NAAMII</span>
<span class="duration">May 2020 - August 2020</span>
</div>
</div>
<span class="status research">Research</span>
<p class="experience-description">
Research internship focused on Computer Vision and AI model development. Worked with state-of-the-art CV models and contributed to various projects involving object detection, facial recognition, and image segmentation.
</p>
<div class="achievements">
<h4>Key Achievements:</h4>
<ul>
<li>Built and fine-tuned computer vision models for object detection, facial recognition, and image segmentation using PyTorch, OpenCV, and scikit-learn</li>
<li>Collaborated with lead researchers to implement and improve state-of-the-art CV models across active research projects</li>
</ul>
</div>
<div class="tech-stack">
<span class="tech-tag">Python</span>
<span class="tech-tag">PyTorch</span>
<span class="tech-tag">OpenCV</span>
<span class="tech-tag">Computer Vision</span>
<span class="tech-tag">scikit-learn</span>
</div>
<div class="experience-links">
<a href="https://www.naamii.org.np" class="company-link" target="_blank">NAAMII</a>
</div>
</div>

</div>

<style>
.experience-intro {
    text-align: center;
    margin-bottom: 3rem;
    padding: 2rem;
    background: var(--theme-bg);
    border-radius: 10px;
}

.experience-timeline {
    position: relative;
    max-width: 900px;
    margin: 0 auto;
}

.experience-timeline::before {
    content: '';
    position: absolute;
    left: 20px;
    top: 0;
    bottom: 0;
    width: 2px;
    background: var(--primary);
    opacity: 0.3;
}

.experience-card {
    background: var(--code-bg);
    border-radius: 12px;
    padding: 2rem;
    margin-bottom: 2rem;
    margin-left: 50px;
    border: 1px solid var(--border);
    position: relative;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.experience-card::before {
    content: '';
    position: absolute;
    left: -41px;
    top: 2rem;
    width: 12px;
    height: 12px;
    background: var(--primary);
    border-radius: 50%;
    border: 3px solid var(--theme);
}

.experience-card:hover {
    transform: translateX(10px);
    box-shadow: 0 10px 25px rgba(0,0,0,0.15);
}

.experience-card.current::before {
    background: #10b981;
    animation: pulse 2s infinite;
}

@keyframes pulse {
    0% { box-shadow: 0 0 0 0 rgba(16, 185, 129, 0.7); }
    70% { box-shadow: 0 0 0 10px rgba(16, 185, 129, 0); }
    100% { box-shadow: 0 0 0 0 rgba(16, 185, 129, 0); }
}

.experience-header {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    margin-bottom: 1rem;
    flex-wrap: wrap;
    gap: 1rem;
}

.experience-header h3 {
    color: var(--primary);
    font-size: 1.5rem;
    margin: 0;
    flex: 1;
}

.company-info {
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    margin-left: auto;
}

.company {
    font-weight: 600;
    color: var(--content);
}

.duration {
    color: var(--secondary);
    font-size: 0.9rem;
}

.status {
    padding: 0.25rem 0.75rem;
    border-radius: 20px;
    font-weight: 500;
    font-size: 0.8rem;
    white-space: nowrap;
}

.current-role {
    background: #10b981;
    color: white;
}

.internship {
    background: var(--primary);
    color: white;
}

.research {
    background: #8b5cf6;
    color: white;
}

.experience-description {
    line-height: 1.6;
    margin-bottom: 1.5rem;
    color: var(--content);
}

.achievements h4 {
    color: var(--primary);
    margin-bottom: 0.75rem;
    font-size: 1.1rem;
}

.achievements ul {
    margin-bottom: 1.5rem;
    padding-left: 1.5rem;
}

.achievements li {
    margin-bottom: 0.5rem;
    color: var(--content);
    line-height: 1.5;
}

.tech-stack {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
    margin-bottom: 1.5rem;
}

.tech-tag {
    background: var(--theme-bg);
    color: var(--primary);
    padding: 0.25rem 0.75rem;
    border-radius: 15px;
    font-size: 0.8rem;
    border: 1px solid var(--border);
}

.experience-links {
    display: flex;
    gap: 1rem;
    flex-wrap: wrap;
    align-items: center;
}

.read-more {
    color: var(--primary);
    text-decoration: none;
    font-weight: 500;
}

.company-link {
    border: 1px solid var(--border);
    color: var(--primary);
    padding: 0.5rem 1rem;
    border-radius: 6px;
    text-decoration: none;
    transition: background 0.3s;
    font-size: 0.9rem;
}

.company-link:hover {
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

@media (max-width: 768px) {
    .experience-timeline::before {
        left: 10px;
    }

    .experience-card {
        margin-left: 30px;
        padding: 1.5rem;
    }

    .experience-card::before {
        left: -21px;
    }

    .experience-header {
        flex-direction: column;
        align-items: flex-start;
    }

    .company-info {
        align-items: flex-start;
    }

    .experience-links {
        flex-direction: column;
        align-items: flex-start;
        gap: 0.75rem;
    }

    .tech-stack {
        gap: 0.25rem;
    }

    .tech-tag {
        font-size: 0.75rem;
        padding: 0.2rem 0.6rem;
    }
}
</style>