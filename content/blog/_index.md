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
<h3><a href="/blog/modern-web-development/">Building Modern Web Applications with FastAPI and Vue.js</a></h3>
<div class="blog-meta">
<span class="date">March 15, 2024</span>
<span class="tags">FastAPI • Vue.js • Python • JavaScript</span>
</div>
<p class="blog-description">
A comprehensive guide to modern web development using Python FastAPI for backend and Vue.js for frontend development. Learn about architecture, authentication, deployment, and best practices for building scalable applications.
</p>
<div class="blog-links">
<a href="/blog/modern-web-development/" class="read-more">Read Full Post →</a>
<a href="https://fastapi.tiangolo.com" class="external-link" target="_blank">FastAPI Docs</a>
</div>
</div>

<div class="blog-card">
<h3><a href="/blog/hugo-guide/">Getting Started with Hugo Static Sites</a></h3>
<div class="blog-meta">
<span class="date">March 10, 2024</span>
<span class="tags">Hugo • Static Sites • Web Development</span>
</div>
<p class="blog-description">
Learn the basics of Hugo static site generator and how to build fast, secure websites. This guide covers installation, content creation, themes, and deployment options for getting started with Hugo.
</p>
<div class="blog-links">
<a href="/blog/hugo-guide/" class="read-more">Read Full Post →</a>
<a href="https://gohugo.io" class="external-link" target="_blank">Hugo Documentation</a>
</div>
</div>

<div class="blog-card">
<h3>Blockchain Development Insights</h3>
<div class="blog-meta">
<span class="date">Coming Soon</span>
<span class="tags">Blockchain • Smart Contracts • Web3</span>
</div>
<p class="blog-description">
Deep dive into blockchain technology and smart contract development. Exploring different blockchain platforms, development tools, and real-world applications.
</p>
<div class="blog-links">
<span class="coming-soon">Coming Soon</span>
<a href="https://ethereum.org" class="external-link" target="_blank">Ethereum Resources</a>
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