---
title: "Blog"
description: "My thoughts, experiences, and insights on development, technology, and more."
---

<!-- <div class="blog-intro">
<h2>Welcome to my blog!</h2>
<p>Here you'll find my thoughts on software development, technology trends, and various projects I'm working on. Each post includes practical insights, code examples, and lessons learned from real-world development.</p>
</div> -->

<div class="blog-grid">

<div class="blog-card">
<h3><a href="/blog/active-llm/">Paper Review: ActiveLLM — Large Language Model-Based Active Learning</a></h3>
<div class="blog-meta">
<span class="date">October 12, 2025</span>
<span class="tags">LLM • Active Learning • Labelling Costs</span>
</div>
<p class="blog-description">
A comprehensive review of the ActiveLLM paper exploring how instruction-tuned LLMs can revolutionize active learning by selecting high-impact training samples without cold-start problems or iterative retraining delays.
</p>
<div class="blog-links">
<a href="/blog/active-llm/" class="read-more">Read Full Post →</a>
<a href="https://arxiv.org/abs/2405.10808" class="external-link" target="_blank">arXiv Paper</a>
</div>
</div>

</div>

<style>
.blog-intro {
    text-align: center;
    margin-bottom: 3rem;
    padding: 2rem;
    background: var(--theme-bg);
    border-radius: 10px;
}

.blog-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
    gap: 2rem;
    margin-top: 2rem;
}

.blog-card {
    background: var(--code-bg);
    border-radius: 12px;
    padding: 2rem;
    border: 1px solid var(--border);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    height: fit-content;
}

.blog-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 25px rgba(0,0,0,0.1);
}

.blog-card h3 {
    margin-bottom: 1rem;
    font-size: 1.4rem;
}

.blog-card h3 a {
    text-decoration: none;
    color: var(--primary);
}

.blog-meta {
    display: flex;
    justify-content: space-between;
    margin-bottom: 1rem;
    font-size: 0.9rem;
    color: var(--secondary);
}

.blog-description {
    line-height: 1.6;
    margin-bottom: 1.5rem;
    color: var(--content);
}

.blog-links {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 1rem;
}

.read-more {
    color: var(--primary);
    text-decoration: none;
    font-weight: 500;
}

.external-link {
    color: var(--secondary);
    text-decoration: none;
    font-size: 0.9rem;
}

.external-link:hover {
    color: var(--primary);
}

.coming-soon {
    color: var(--secondary);
    font-style: italic;
}

@media (max-width: 768px) {
    .blog-grid {
        grid-template-columns: 1fr;
        gap: 1.5rem;
    }

    .blog-card {
        padding: 1.5rem;
    }

    .blog-meta {
        flex-direction: column;
        gap: 0.5rem;
    }

    .blog-links {
        flex-direction: column;
        align-items: flex-start;
    }
}
</style>