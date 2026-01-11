---
layout: landing
title: "The R&D Lab"
description: "Experimental prototypes, Motion Capture (MOCAP) workflows, and technical workshops."
image: assets/images/lab-banner.jpg
nav-menu: true
#show_tile: true
weight: 4
---

<div id="main">
    <section id="one" class="spotlights">
        <section>
            <a href="#filters" data-select="heritage" class="image scrolly">
                <img src="{{ 'assets/images/projectshowcase1.png' | relative_url }}" alt="" data-position="center center" />
            </a>
            <div class="content">
                <div class="inner">
                    <header class="major">
                        <h3>Exploration & Education</h3>
                    </header>
                    <p>The Lab is where I test new SDKs, experiment with MOCAP data, and share knowledge through technical workshops for the next generation of XR creators.</p>
                    <div class="featured-links">
                        <span class="label">Featured Projects:</span>
                        <div class="link-group">
                            <a href="/projects/rising-tide" class="button small icon solid fa-arrow-right">Rising Tide</a>
                            <a href="/projects/sidewalks-asia" class="button small icon solid fa-arrow-right">Sidewalks Asia</a>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        <section>
            <a href="#filters" data-select="retail" class="image scrolly">
                <img src="{{ 'assets/images/projectshowcase1.png' | relative_url }}" alt="" data-position="top center" />
            </a>
            <div class="content">
                <div class="inner">
                    <header class="major">
                        <h3>MOCAP & DanceXR Workshops</h3>
                    </header>
                    <p>Utilizing Rokoko Suits to capture and retarget high-fidelity motion data into Unity environments for theatrical and artistic performances.</p>
                    <div class="featured-links">
                        <span class="label">Featured Projects:</span>
                        <div class="link-group">
                            <a href="/projects/decora" class="button small icon solid fa-arrow-right">DECORA</a>
                            <a href="/projects/ardino" class="button small icon solid fa-arrow-right">AR Dino T-Shirt</a>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        <section>
            <a href="#filters" data-select="heritage" class="image scrolly">
                <img src="{{ 'assets/images/projectshowcase1.png' | relative_url }}" alt="" data-position="center center" />
            </a>
            <div class="content">
                <div class="inner">
                    <header class="major">
                        <h3>AR Magic Hand & AI Pets</h3>
                    </header>
                    <p>Experimental prototypes testing hand-tracking latency and AI-driven interactions within the Meta Movement SDK ecosystem.</p>
                    <div class="featured-links">
                        <span class="label">Featured Projects:</span>
                        <div class="link-group">
                            <a href="/projects/deepavali-postcard" class="button small icon solid fa-arrow-right">Deepavali Postcard</a>
                            <a href="/projects/planterengganu-postcard" class="button small icon solid fa-arrow-right">Terengganu Postcard</a>
                        </div>
                    </div>      
                </div>
            </div>
        </section>
    </section>
    <section class="inner">
        <ul class="actions" id="filters">
            <li><a href="#" data-filter="*" class="button primary small">All</a></li>
            <li><a href="#" data-filter=".heritage" class="button small">Heritage</a></li>
            <li><a href="#" data-filter=".retail" class="button small">Retail</a></li>
            <li><a href="#" data-filter=".event" class="button small">Event</a></li>
            <li><a href="#" data-filter=".marketing" class="button small">Marketing</a></li>
        </ul>
       <div id="project-list-container">
            <div class="project-tags-grid" id="project-grid">
               {% for project in site.projects %}
                {% if project.pillar == "augmented-reality" %}
                <div class="project-tag-item project-item {{ project.genre | downcase }}" 
                    data-image="{{ project.image | relative_url }}">
                    <a href="{{ project.url | relative_url }}" class="tag-link">
                        <div class="tag-content">
                            <div class="tag-thumb">
                                <img src="{{ project.image | relative_url }}" alt="" />
                            </div>
                            <div class="tag-text">
                                <span class="project-title">{{ project.title }}</span>
                                <span class="project-hardware">{{ project.hardware }}</span>
                            </div>
                        </div>
                    </a>
                </div>
                {% endif %}
                {% endfor %}
            </div>
        </div>
    </section>
</div>