---
title: "Others"
description: "Certifications, awards, hackathon prizes, and achievements"
---

<div class="others-grid">

<div class="achievement-card certification">
<div class="achievement-icon">🏆</div>
<h3>AWS Certified Developer</h3>
<div class="achievement-meta">
<span class="type">Certification</span>
<span class="date">2023</span>
</div>
<p class="achievement-description">
Amazon Web Services Certified Developer Associate certification, demonstrating proficiency in developing and maintaining applications on the AWS platform with best practices for security, performance, and cost optimization.
</p>
<div class="achievement-links">
<a href="/others/aws-certification/" class="read-more">Read More →</a>
<a href="https://aws.amazon.com/certification/" class="external-link" target="_blank">AWS Certifications</a>
</div>
</div>

<div class="achievement-card award">
<div class="achievement-icon">🥇</div>
<h3>Best Innovation Award</h3>
<div class="achievement-meta">
<span class="type">Award</span>
<span class="date">2022</span>
</div>
<p class="achievement-description">
Recognized for developing innovative solutions during the annual company hackathon, focusing on blockchain integration and user experience improvements that enhanced overall platform functionality.
</p>
<div class="achievement-links">
<a href="/others/innovation-award/" class="read-more">Read More →</a>
<span class="company">Sireto Technology</span>
</div>
</div>

<div class="achievement-card hackathon">
<div class="achievement-icon">💻</div>
<h3>HackTheValley Winner</h3>
<div class="achievement-meta">
<span class="type">Hackathon</span>
<span class="date">2021</span>
</div>
<p class="achievement-description">
First place winner at HackTheValley hackathon for developing a real-time collaborative coding platform with integrated video chat and code review features, built using Vue.js and WebSocket technology.
</p>
<div class="achievement-links">
<a href="/others/hackthevalley/" class="read-more">Read More →</a>
<a href="https://hackthevalley.io" class="external-link" target="_blank">HackTheValley</a>
</div>
</div>

<div class="achievement-card certification">
<div class="achievement-icon">📜</div>
<h3>MongoDB Developer Certification</h3>
<div class="achievement-meta">
<span class="type">Certification</span>
<span class="date">2022</span>
</div>
<p class="achievement-description">
MongoDB Certified Developer Associate certification, validating expertise in MongoDB database design, development, and deployment with focus on performance optimization and scalability.
</p>
<div class="achievement-links">
<a href="/others/mongodb-certification/" class="read-more">Read More →</a>
<a href="https://university.mongodb.com/certification" class="external-link" target="_blank">MongoDB University</a>
</div>
</div>

<div class="achievement-card award">
<div class="achievement-icon">🌟</div>
<h3>Outstanding Performance Award</h3>
<div class="achievement-meta">
<span class="type">Award</span>
<span class="date">2023</span>
</div>
<p class="achievement-description">
Recognized for exceptional contribution to team projects and maintaining high code quality standards while delivering features ahead of schedule and mentoring junior developers.
</p>
<div class="achievement-links">
<a href="/others/performance-award/" class="read-more">Read More →</a>
<span class="company">Current Role</span>
</div>
</div>

<div class="achievement-card hackathon">
<div class="achievement-icon">🚀</div>
<h3>NASA Space Apps Challenge</h3>
<div class="achievement-meta">
<span class="type">Hackathon</span>
<span class="date">2020</span>
</div>
<p class="achievement-description">
Participated in NASA Space Apps Challenge, developing an Earth observation data visualization tool using satellite imagery and machine learning for environmental monitoring and climate research.
</p>
<div class="achievement-links">
<a href="/others/nasa-space-apps/" class="read-more">Read More →</a>
<a href="https://www.spaceappschallenge.org" class="external-link" target="_blank">Space Apps</a>
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

.achievement-card.hackathon {
    border-left: 4px solid #10b981;
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