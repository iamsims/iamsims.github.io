---
title: "Others"
description: "Certifications, awards, hackathon prizes, and achievements"
---

<div class="others-grid">

<div class="achievement-card certification">
<div class="achievement-icon">🚀</div>
<h3>Machine Learning in Production</h3>
<div class="achievement-meta">
<span class="type">Certification</span>
<span class="date">May 2025</span>
</div>
<p class="achievement-description">
Completed Machine Learning in Production course authorized by DeepLearning.AI and offered through Coursera. Covered MLOps best practices, model deployment, monitoring, and maintaining ML systems in production environments.
</p>
<div class="achievement-links">
<a href="https://coursera.org/verify/Q6ODQCJPOSE8" class="external-link" target="_blank">Verify Certificate</a>
<a href="https://www.coursera.org/learn/introduction-to-machine-learning-in-production" class="external-link" target="_blank">View Course</a>
</div>
</div>

<div class="achievement-card award">
<div class="achievement-icon">🥈</div>
<h3>Won 2nd Place, Impact X-athon 2024</h3>
<div class="achievement-meta">
<span class="type">Award</span>
<span class="date">2024</span>
</div>
<p class="achievement-description">
Secured 2nd place at NASA IMPACT X-athon 2024, developing a innovate solution for path finder in the building. 
</p>
<div class="achievement-links">
<span class="company">NASA IMPACT</span>
</div>
</div>

<div class="achievement-card fellowship">
<div class="achievement-icon">🎓</div>
<h3>Codepath Fellow</h3>
<div class="achievement-meta">
<span class="type">Fellowship</span>
<span class="date">2024</span>
</div>
<p class="achievement-description">
Selected as a Codepath Fellow, participating in complex problem solving and coordination with team members to collaborate on various kinds of problem solving. 
</p>
<div class="achievement-links">
<a href="https://www.codepath.org" class="external-link" target="_blank">Codepath</a>
</div>
</div>

<div class="achievement-card leadership">
<div class="achievement-icon">🎤</div>
<h3>Microsoft Learn Student Ambassador</h3>
<div class="achievement-meta">
<span class="type">Leadership</span>
<span class="date">2019 - 2021</span>
</div>
<p class="achievement-description">
Served as Microsoft Learn Student Ambassador, organizing technical workshops, promoting Microsoft technologies, and building a community of student developers on campus. Selected to join the Microsoft Student Summit 2020 APAC Region with full funding sponsored by Microsoft.
</p>
<div class="achievement-links">
<a href="https://studentambassadors.microsoft.com" class="external-link" target="_blank">Microsoft Learn</a>
</div>
</div>

<div class="achievement-card certification">
<div class="achievement-icon">📜</div>
<h3>Machine Learning Certification</h3>
<div class="achievement-meta">
<span class="type">Certification</span>
<span class="date">2019</span>
</div>
<p class="achievement-description">
Completed Machine Learning certification from Stanford Online via Coursera, covering supervised learning, unsupervised learning, neural networks, and best practices in machine learning.
</p>
<div class="achievement-links">
<a href="https://www.coursera.org/learn/machine-learning" class="external-link" target="_blank">Stanford ML Course</a>
</div>
</div>

<div class="achievement-card award">
<div class="achievement-icon">🎓</div>
<h3>Full Undergraduate Scholarship</h3>
<div class="achievement-meta">
<span class="type">Award</span>
<span class="date">2017</span>
</div>
<p class="achievement-description">
Awarded full undergraduate scholarship from Tribhuvan University for academic excellence, covering tuition and expenses throughout the Bachelor of Computer Engineering program.
</p>
<div class="achievement-links">
<span class="company">Tribhuvan University</span>
</div>
</div>

</div>

<style>
.others-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
    gap: 2rem;
    margin-top: 2rem;
}

.achievement-card {
    background: var(--code-bg);
    border-radius: 12px;
    padding: 2rem;
    border: 1px solid var(--border);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    height: fit-content;
    position: relative;
}

.achievement-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 25px rgba(0,0,0,0.15);
}

.achievement-card.certification {
    border-left: 4px solid #3b82f6;
}

.achievement-card.award {
    border-left: 4px solid #f59e0b;
}

.achievement-card.fellowship {
    border-left: 4px solid #8b5cf6;
}

.achievement-card.hackathon {
    border-left: 4px solid #10b981;
}

.achievement-card.leadership {
    border-left: 4px solid #ec4899;
}



.achievement-icon {
    font-size: 2.5rem;
    margin-bottom: 1rem;
    display: block;
}

.achievement-card h3 {
    margin-bottom: 1rem;
    font-size: 1.5rem;
    color: var(--primary);
}

.achievement-meta {
    display: flex;
    justify-content: space-between;
    margin-bottom: 1rem;
    font-size: 0.9rem;
}

.type {
    padding: 0.25rem 0.75rem;
    border-radius: 20px;
    font-weight: 500;
    font-size: 0.8rem;
    color: white;
}

.certification .type {
    background: #3b82f6;
}

.award .type {
    background: #f59e0b;
}

.fellowship .type {
    background: #8b5cf6;
}

.leadership .type {
    background: #ec4899;
}

.hackathon .type {
    background: #10b981;
}

.date {
    color: var(--secondary);
    font-weight: 500;
}

.achievement-description {
    line-height: 1.6;
    margin-bottom: 1.5rem;
    color: var(--content);
}

.achievement-links {
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

.external-link {
    color: var(--secondary);
    text-decoration: none;
    font-size: 0.9rem;
}

.external-link:hover {
    color: var(--primary);
}

.company {
    color: var(--secondary);
    font-style: italic;
    font-size: 0.9rem;
}

@media (max-width: 768px) {
    .others-grid {
        grid-template-columns: 1fr;
        gap: 1.5rem;
    }

    .achievement-card {
        padding: 1.5rem;
    }

    .achievement-meta {
        flex-direction: column;
        gap: 0.5rem;
    }

    .achievement-links {
        flex-direction: column;
        align-items: flex-start;
        gap: 0.75rem;
    }
}
</style>