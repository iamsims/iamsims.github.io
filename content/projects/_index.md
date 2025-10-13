---
title: "Projects"
description: "A showcase of my development projects and technical work (WIP)"
---

<!-- <div class="projects-intro">
<h2>Project Showcase</h2>
<p>Here's a collection of my personal and professional development work, demonstrating my skills in various technologies and frameworks. Each project includes live demos, source code, and detailed technical information.</p>
</div> -->

<div class="projects-grid">

<div class="project-card">
<h3>Personal Portfolio Website</h3>
<div class="project-meta">
<span class="status">Live</span>
<span class="tech">Hugo • GitHub Pages • Responsive Design</span>
</div>
<p class="project-description">
A modern, responsive portfolio website built with Hugo static site generator and deployed on GitHub Pages. Features automated deployment pipeline, 95+ Google PageSpeed score, and mobile-responsive design supporting all device sizes.
</p>
<div class="project-features">
<ul>
<li>Automated CI/CD with GitHub Actions</li>
<li>SEO optimized with structured data</li>
<li>Fast loading with static site generation</li>
<li>Responsive design for all devices</li>
</ul>
</div>
<div class="project-links">
<a href="/projects/web-portfolio/" class="read-more">Read More →</a>
<a href="https://simrankc.com.np" class="live-demo" target="_blank">Live Demo →</a>
<a href="https://github.com/iamsims/iamsims.github.io" class="source-code" target="_blank">View Source</a>
<a href="https://gohugo.io" class="external-link" target="_blank">Hugo Docs</a>
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
    margin-bottom: 1rem;
    font-size: 1.5rem;
    color: var(--primary);
}

.project-meta {
    display: flex;
    justify-content: space-between;
    margin-bottom: 1rem;
    font-size: 0.9rem;
}

.status {
    padding: 0.25rem 0.75rem;
    border-radius: 20px;
    font-weight: 500;
    font-size: 0.8rem;
}

.status:contains("Live") { background: #10b981; color: white; }
.project-meta .status { background: var(--primary); color: white; }

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