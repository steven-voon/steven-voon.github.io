---
layout: landing
title: "Tecnical Leadership"
description: "Architecting XR ecosystems and driving digital transformation through industry-academic partnerships."
image: assets/images/leadership-banner.jpg
nav-menu: true
#show_tile: true
weight: 3
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
                        <h3>Bridge Between Innovation & Execution</h3>
                    </header>
                    <p>With over 7 years in the XR space, my role has evolved from developer to strategist. I specialize in requirement analysis, technical feasibility studies, and leading cross-functional teams to deliver high-impact spatial solutions.</p>
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
                        <h3>Strategic Partnerships & MOUs</h3>
                    </header>
                    <p>I orchestrate formal collaborations between industry and academia to push the boundaries of XR R&D. This includes signing MOUs with <strong>UTHM</strong>, <strong>University of Xiamen Malaysia</strong>, and <strong>Catalyst 360</strong> for specialized virtual tour services.</p>
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
                        <h3>Exhibition & Public Engagement</h3>
                    </header>
                    <p>Regularly represent organizations (Maitree House, Creatinno Tech) at national-level events like <strong>Digital Penang</strong> and <strong>Higher Education Fairs</strong>. I translate complex Unity-based solutions into clear business value for government stakeholders and corporate clients.</p>
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
        <section>
            <a href="#filters" data-select="heritage" class="image scrolly">
                <img src="{{ 'assets/images/projectshowcase1.png' | relative_url }}" alt="" data-position="center center" />
            </a>
            <div class="content">
                <div class="inner">
                    <header class="major">
                        <h3>Industrial Training & Mentorship</h3>
                    </header>
                    <p>Technical Lead for the <strong>CahayaXR Mentorship</strong> programs. I guide artists and researchers through the XR pipeline, from Tiltbrush concepts to final Quest 2/Web deployment, ensuring technical stability and user-centric design.</p>
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