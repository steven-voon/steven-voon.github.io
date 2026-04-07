---
layout: post
title: "Template"
image: "/assets/images/pic04.jpg"
pillar: "augmented-reality"
genre: "heritage"
company: "Maitree House"
company_url: "https://www.maitreehouse.com/"
hardware: "Mobile"
technologies: ["AR", "Unity"]
project_url: "https://www.ceritalah.app/" 
achievement_url_1: "https://www.ceritalah.app/" 
achievement_url_2: "https://www.ceritalah.app/" 
achievement_url_3: "https://www.ceritalah.app/" 

# CASE A: YouTube
video_id: "dGrWmW-sRdM"
video_type: "youtube"

# CASE B: Vimeo
# video_id: "123456789"
# video_type: "vimeo"

project_images: 
  - "/assets/images/bioticX-ss0.png"
  - "/assets/images/bioticX-ss1.png"
  - "/assets/images/bioticX-ss2.png"
  - "/assets/images/bioticX-ss3.png"
  - "/assets/images/bioticX-ss4.png"
  - "/assets/images/bioticX-ss5.png"
  - "/assets/images/bioticX-ss6.png"
  - "/assets/images/bioticX-ss7.png"
media_caption: "Interaction Design: User Flow and AR Interface Mockups"
---

<div class="project-dashboard" style="display: flex; flex-wrap: wrap; justify-content: center; align-items: stretch; gap: 0; background: rgba(255, 255, 255, 0.07); backdrop-filter: blur(10px); padding: 1.5rem; border: 1px solid rgba(255, 255, 255, 0.15); border-radius: 16px; margin-top: -2.5rem; margin-bottom: 4rem; box-shadow: 0 20px 40px rgba(0,0,0,0.3); position: relative; z-index: 10;"> 
    <div class="dash-item">
        <span class="dash-label">Client</span>
        <a href="{{ page.company_url }}" target="_blank" class="dash-client-link">
            {{ page.company }} <span style="font-size: 0.8rem; opacity: 0.7;">↗</span>
        </a>
    </div>
    <div class="dash-sep"></div>
    <div class="dash-item">
        <span class="dash-label">Role</span>
        <span class="dash-value" style="color: #9bf1ff;">Technical Lead</span>
    </div>
    <div class="dash-sep"></div>
    <div class="dash-item">
        <span class="dash-label">Team Size</span>
        <span class="dash-value">3 Devs + 1 Agency</span>
    </div>
    <div class="dash-sep"></div>
    <div class="dash-item">
        <span class="dash-label">Timeline</span>
        <div style="display: flex; flex-direction: column; align-items: center;">
            <span class="dash-value">2 Years</span>
            <span style="font-size: 0.6rem; color: #9bf1ff; text-transform: uppercase; letter-spacing: 1px; margin-top: 4px; opacity: 0.9;">R&D • Proto • Live Ops</span>
        </div>
    </div>
    <div class="dash-sep"></div>
    <div class="dash-item">
        <span class="dash-label">Performance</span>
        <span class="dash-value" style="color: #9bff9b;">60 FPS</span>
    </div>
    <div class="dash-sep"></div>
    <div class="dash-item" style="min-width: 180px;">
        <a href="{{ page.project_url }}" target="_blank" class="dash-btn">Project Site ↗</a>
    </div>
</div>

<div class="achievement-breakout"> 
    <div class="breakout-label">Featured & Recognized</div>
    <a href="{{ page.achievement_url_1 }}" target="_blank" class="achievement-link">
        <span class="achievement-icon">🖼️</span> Digital Heritage Exhibition 2025
    </a>
    <a href="{{ page.achievement_url_2 }}" target="_blank" class="achievement-link">
        <span class="achievement-icon">📰</span> Featured on [Media Name]
    </a>
    <a href="{{ page.achievement_url_3 }}" target="_blank" class="achievement-link">
        <span class="achievement-icon">🎤</span> XR Summit Malaysia Showcase
    </a>
</div>

<div style="display: flex; align-items: center; gap: 15px; margin-bottom: 2.5rem; margin-top: 4rem;">
    <div style="width: 5px; height: 35px; background: #9bf1ff; border-radius: 10px; box-shadow: 0 0 15px rgba(155, 241, 255, 0.6);"></div>
    <h3 style="margin: 0; font-size: 1.8rem; letter-spacing: 2px; text-transform: uppercase; color: #ffffff; font-weight: 800;">The Vision</h3>
</div>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(320px, 1fr)); gap: 4rem; align-items: start; margin-bottom: 6rem;">   
    <div style="display: flex; flex-direction: column; gap: 2rem;">
        <div>
            <h5 style="font-size: 0.7rem; color: #9bf1ff; text-transform: uppercase; letter-spacing: 2px; margin-bottom: 10px;">Project Overview</h5>
            <p style="font-size: 1.2rem; line-height: 1.7; color: #ffffff; margin: 0; opacity: 0.9;">
                <strong>Ceritalah</strong> is a digital heritage platform leveraging <strong>Augmented Reality</strong> to transform physical landmarks into storytelling hubs.
            </p>
        </div>
        <div style="background: rgba(155, 241, 255, 0.05); padding: 1.5rem; border-radius: 12px; border-left: 2px solid rgba(155, 241, 255, 0.3);">
            <h5 style="font-size: 0.7rem; color: #9bf1ff; text-transform: uppercase; letter-spacing: 2px; margin-bottom: 10px;">My Role & Strategic Goal</h5>
            <p style="font-size: 1.2rem; line-height: 1.7; color: #ffffff; margin: 0;">
                Architected a <strong>modular delivery pipeline</strong> ensuring high-fidelity AR stability under outdoor environmental constraints.
            </p>
        </div>
    </div>
    <<div class="vision-media-container">
        <div class="carousel-container">
            <div class="carousel-scroll">             
                {% if page.video_id %}
                <div class="carousel-item video-slide">
                    <div class="video-wrapper">
                        <div class="video-shield"></div>                   
                        {% if page.video_type == "youtube" %}
                            <iframe 
                                src="https://www.youtube.com/embed/{{ page.video_id }}?autoplay=1&mute=1&loop=1&playlist={{ page.video_id }}&modestbranding=1&rel=0&iv_load_policy=3&controls=0" 
                                frameborder="0" allow="autoplay; encrypted-media" allowfullscreen>
                            </iframe>                     
                        {% elsif page.video_type == "vimeo" %}
                            <iframe src="https://player.vimeo.com/video/{{ page.video_id }}?autoplay=1&muted=1&loop=1&background=1" frameborder="0" allowfullscreen></iframe>
                        {% endif %}
                    </div>
                </div>
                {% endif %}
                {% for img in page.project_images %}
                <div class="carousel-item">
                    <img src="{{ img }}" alt="Project Detail Image">
                </div>
                {% endfor %}               
            </div>                
        </div>      
        <div class="carousel-hint">
            <span>⟵ Swipe to see details ⟶</span>
        </div> 
        <p class="media-caption">
            {{ page.media_caption | default: "Project Media Gallery" }}
        </p>
    </div>
</div>

<div style="background: rgba(155, 241, 255, 0.05); padding: 2rem; border-radius: 20px; border: 1px dashed rgba(155, 241, 255, 0.3); margin-bottom: 4rem; backdrop-filter: blur(5px);">
    <div style="display: flex; align-items: center; gap: 12px; margin-bottom: 1.5rem;">
        <div style="width: 4px; height: 20px; background: #9bf1ff; border-radius: 4px;"></div>
        <h5 style="font-size: 0.85rem; color: #9bf1ff; text-transform: uppercase; letter-spacing: 2px; margin: 0; font-weight: 700;">Leadership & Agency Management</h5>
    </div>
    <p style="font-size: 1.2rem; line-height: 1.8; color: #eee; margin-bottom: 2rem;">
        Coordinated a remote team of 3 developers and an external agency. Managed the project through a 24-month lifecycle from R&D to regional deployment.
    </p>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: 1.5rem;">
        <div style="font-size: 1rem; color: #9bff9b; display: flex; align-items: center; gap: 8px;"><span>✔</span> <strong>Weekly Syncs:</strong> Sprint goals & blockers.</div>
        <div style="font-size: 1rem; color: #9bff9b; display: flex; align-items: center; gap: 8px;"><span>✔</span> <strong>QA Gatekeeper:</strong> Code & asset reviews.</div>
        <div style="font-size: 1rem; color: #9bff9b; display: flex; align-items: center; gap: 8px;"><span>✔</span> <strong>CI/CD Workflow:</strong> Enforced 0% regression.</div>
    </div>
</div>

<div style="display: flex; align-items: center; gap: 15px; margin-bottom: 2.5rem;">
    <div style="width: 5px; height: 35px; background: #9bf1ff; border-radius: 10px; box-shadow: 0 0 15px rgba(155, 241, 255, 0.6);"></div>
    <h3 style="margin: 0; font-size: 1.8rem; letter-spacing: 2px; text-transform: uppercase; color: #ffffff; font-weight: 800;">Project Ecosystem</h3>
</div>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 2rem; margin-bottom: 4.5rem;">
    <div class="tech-box">
        <h5 class="tech-label">Core Engine</h5>
        <div style="display: flex; flex-wrap: wrap; gap: 8px;"><span class="tech-tag">Unity 2022.3</span><span class="tech-tag">URP</span><span class="tech-tag">ARFoundation</span></div>
    </div>
    <div class="tech-box">
        <h5 class="tech-label">Infrastructure</h5>
        <div style="display: flex; flex-wrap: wrap; gap: 8px;"><span class="tech-tag">AWS S3</span><span class="tech-tag">Addressables</span><span class="tech-tag">Google VPS</span></div>
    </div>
    <div class="tech-box">
        <h5 class="tech-label">Production</h5>
        <div style="display: flex; flex-wrap: wrap; gap: 8px;"><span class="tech-tag">GitHub CI/CD</span><span class="tech-tag">Slack API</span><span class="tech-tag">Jira</span></div>
    </div>
</div>

<div style="display: flex; align-items: center; gap: 15px; margin-bottom: 2.5rem;">
    <div style="width: 5px; height: 35px; background: #9bf1ff; border-radius: 10px; box-shadow: 0 0 15px rgba(155, 241, 255, 0.6);"></div>
    <h3 style="margin: 0; font-size: 1.8rem; letter-spacing: 2px; text-transform: uppercase; color: #ffffff; font-weight: 800;">Engineering Post-Mortem</h3>
</div>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 2rem; margin-bottom: 6rem;">
    <div class="challenge-card" style="border-top-color: #ff9b9b; background: rgba(255, 155, 155, 0.05);">
        <h4 style="color: #ff9b9b; font-size: 1.1rem; text-transform: uppercase; margin-bottom: 1rem;">Spatial Logic</h4>
        <p style="font-size: 1.1rem; color: #f0f0f0; margin-bottom: 1.5rem;">Hybrid Localization to solve 10m GPS inaccuracy.</p>
        <div class="result-tag" style="border-left-color: #9bff9b; color: #9bff9b;">✔ Sub-centimeter anchoring.</div>
    </div>
    <div class="challenge-card" style="border-top-color: #9bf1ff; background: rgba(155, 241, 255, 0.05);">
        <h4 style="color: #9bf1ff; font-size: 1.1rem; text-transform: uppercase; margin-bottom: 1rem;">Performance</h4>
        <p style="font-size: 1.1rem; color: #f0f0f0; margin-bottom: 1.5rem;">Mitigated 38°C thermal throttling.</p>
        <div class="result-tag" style="border-left-color: #9bf1ff; color: #9bf1ff;">✔ Stable 60FPS.</div>
    </div>
    <div class="challenge-card" style="border-top-color: #ffcc66; background: rgba(255, 204, 102, 0.05);">
        <h4 style="color: #ffcc66; font-size: 1.1rem; text-transform: uppercase; margin-bottom: 1rem;">Strategic UX</h4>
        <p style="font-size: 1.1rem; color: #f0f0f0; margin-bottom: 1.5rem;">Solved User Placement friction.</p>
        <div class="result-tag" style="border-left-color: #ffcc66; color: #ffcc66;">✔ Ghosting guide system.</div>
    </div>
</div>

<div style="display: flex; align-items: center; gap: 15px; margin-bottom: 2.5rem;">
    <div style="width: 5px; height: 35px; background: #9bf1ff; border-radius: 10px; box-shadow: 0 0 15px rgba(155, 241, 255, 0.6);"></div>
    <h3 style="margin: 0; font-size: 1.8rem; letter-spacing: 2px; text-transform: uppercase; color: #ffffff; font-weight: 800;">Architect's Retrospective</h3>
</div>

<div style="background: rgba(255, 255, 255, 0.07); backdrop-filter: blur(20px); border: 1px solid rgba(255, 255, 255, 0.15); border-radius: 20px; padding: 3rem; margin-bottom: 5rem;">
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 3rem;">
        <div><h5 class="retro-label" style="color: #ff9b9b;">Technical Debt</h5><ul class="retro-list"><li>5G/3G handover</li><li>Device fragmentation</li></ul></div>
        <div><h5 class="retro-label" style="color: #9bff9b;">Future Roadmap</h5><ul class="retro-list"><li>Occlusion 2.0</li><li>Solar light estimation</li></ul></div>
        <div><h5 class="retro-label" style="color: #9bf1ff;">The Verdict</h5><p style="font-size: 1.1rem; color: #eee; line-height: 1.8;">Mobile AR success depends on <strong>Environmental UX</strong>.</p></div>
    </div>
</div>

<style>
    /* Global Layout Safety */
    body { overflow-x: hidden; }

    /* --- Project Dashboard --- */
    .dash-item {
        flex: 1 1 150px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        text-align: center;
        padding: 1rem;
        min-height: 100px; /* Refined for better vertical rhythm */
    }

    .dash-sep {
        width: 1px;
        background: rgba(255, 255, 255, 0.15);
        margin: 1.5rem 0;
    }

    .dash-label {
        display: block;
        font-size: 0.75rem;
        color: #aaa;
        text-transform: uppercase;
        letter-spacing: 2px;
        margin-bottom: 8px;
    }

    .dash-value {
        color: #ffffff;
        font-weight: 800;
        font-size: 1.15rem;
        line-height: 1.2;
    }

    .dash-client-link {
        color: #9bf1ff !important;
        font-weight: 800;
        font-size: 1.15rem;
        text-decoration: none !important;
        border-bottom: none !important;
        transition: opacity 0.3s ease;
    }

    .dash-btn {
        display: inline-flex;
        align-items: center;
        justify-content: center;
        background: #9bf1ff;
        color: #0b1118 !important;
        padding: 12px 20px;
        border-radius: 12px;
        font-weight: 700;
        text-decoration: none !important;
        font-size: 0.85rem;
        box-shadow: 0 4px 15px rgba(155, 241, 255, 0.3);
        white-space: nowrap;
        transition: transform 0.2s ease;
    }

    .dash-btn:hover { transform: scale(1.05); }

    /* --- Achievement Ribbon --- */
    .achievement-breakout {
        position: relative;
        left: 50%; right: 50%;
        margin-left: -50vw; margin-right: -50vw;
        width: 100vw;
        display: flex; align-items: center; justify-content: center; flex-wrap: wrap; gap: 2rem;
        padding: 3rem 0;
        background: rgba(155, 241, 255, 0.08);
        backdrop-filter: blur(10px);
        -webkit-backdrop-filter: blur(10px);
        border-top: 1px solid rgba(155, 241, 255, 0.2);
        border-bottom: 1px solid rgba(155, 241, 255, 0.2);
        margin-bottom: 5rem;
        z-index: 1;
    }

    .breakout-label { font-size: 0.75rem; color: #9bf1ff; text-transform: uppercase; letter-spacing: 2px; font-weight: 800; border-right: 2px solid rgba(155, 241, 255, 0.3); padding-right: 2rem; }
    
    .achievement-link { 
        display: flex; align-items: center; color: #ffffff !important; text-decoration: none !important; font-size: 1rem; font-weight: 600; padding: 10px 18px; border-radius: 8px; border: 1px solid rgba(255,255,255,0.1); transition: all 0.3s ease; 
    }

    .achievement-link:hover { background: rgba(155, 241, 255, 0.15); color: #9bf1ff !important; transform: translateY(-3px); border-color: #9bf1ff; }
    
    .achievement-icon { font-size: 1.2rem; margin-right: 8px; }

    /* --- Media Carousel --- */
    .vision-media-container {
        background: rgba(0,0,0,0.4); padding: 12px; border-radius: 20px; border: 1px solid rgba(255,255,255,0.15); box-shadow: 0 20px 50px rgba(0,0,0,0.5);
    }

    .video-wrapper {
        position: relative;
        width: 100%;
        padding-bottom: 56.25%;
        height: 0;
        overflow: hidden;
        border-radius: 8px;
        background: #000;
    }

    .video-shield {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        z-index: 10; 
        background: rgba(0,0,0,0); /* Invisible but physically there */
        pointer-events: auto; /* This captures the swipe */
    }

    .video-wrapper iframe {
        position: absolute; 
        top: 0; 
        left: 0; 
        width: 100%; 
        height: 100%; 
        z-index: 1; 
        pointer-events: none; /* This prevents the iframe from stealing the touch */
    }

    .video-wrapper video {
        position: absolute; 
        top: 0; 
        left: 0; 
        width: 100%; 
        height: 100%; 
        object-fit: cover; 
        background: #000;
        z-index: 1; /* Sits below the shield */
    }

    .carousel-container { position: relative; width: 100%; border-radius: 12px; overflow: hidden; }
    
    .carousel-scroll {
        display: flex;
        overflow-x: auto !important;
        scroll-snap-type: x mandatory;
        scroll-behavior: smooth;
        scrollbar-width: none;     /* Firefox */
        gap: 20px;
        padding-bottom: 10px;
        -webkit-overflow-scrolling: touch; /* Essential for iOS */
        -ms-overflow-style: none;  /* IE and Edge */
        touch-action: pan-x; /* Essential for Android: tells browser to ignore vertical scroll here */
    }

    .carousel-scroll::-webkit-scrollbar { display: none; }

    .carousel-item { flex: 0 0 100%; scroll-snap-align: start; display: flex; align-items: center; justify-content: center; transform: translateZ(0);}

    .carousel-item img { width: 100%; height: auto; aspect-ratio: 16/9; display: block; border-radius: 8px; object-fit: cover; }

    .carousel-hint { text-align: center; font-size: 0.65rem; color: #9bf1ff; text-transform: uppercase; letter-spacing: 1px; margin-top: 10px; opacity: 0.6; }

    .media-caption { font-size: 0.7rem; text-align: center; margin: 1.5rem 0 0.5rem 0; color: #9bf1ff; letter-spacing: 1px; text-transform: uppercase; font-weight: 600; opacity: 0.8; }

    /* --- Technical Sections --- */
    .tech-box { background: rgba(255,255,255,0.05); padding: 1.8rem; border-radius: 12px; border: 1px solid rgba(255,255,255,0.1); }
    
    .tech-label { font-size: 0.9rem; color: #9bf1ff; text-transform: uppercase; margin-bottom: 1.2rem; letter-spacing: 1px; font-weight: 700; }
    
    .tech-tag { background: rgba(255,255,255,0.1); color: #fff; padding: 6px 14px; border-radius: 6px; font-size: 0.85rem; border: 1px solid rgba(255,255,255,0.2); }

    .challenge-card { background: rgba(0,0,0,0.25); padding: 2.5rem; border-radius: 0 0 20px 20px; border: 1px solid rgba(255,255,255,0.1); border-top: 4px solid; display: flex; flex-direction: column; justify-content: space-between; min-height: 250px; }
    
    .result-tag { background: rgba(255, 255, 255, 0.05); padding: 12px; border-left: 4px solid; font-size: 1rem; border-radius: 4px; font-weight: 600; margin-top: 10px; }
    
    .retro-label { font-size: 0.9rem; text-transform: uppercase; letter-spacing: 2px; margin-bottom: 1.2rem; font-weight: 700; }
    
    .retro-list { font-size: 1.1rem; padding-left: 1.2rem; color: #ddd; line-height: 2; margin: 0; }

    /* --- Responsive Fixes --- */
    @media (max-width: 900px) {
        .dash-sep { display: none; }
        .dash-item { flex: 1 1 45%; border-bottom: 1px solid rgba(255, 255, 255, 0.1); }
    }

    @media (max-width: 768px) {
        .achievement-breakout { flex-direction: column; padding: 3rem 1rem; }
        .breakout-label { border-right: none; border-bottom: 1px solid rgba(155, 241, 255, 0.2); padding-right: 0; padding-bottom: 10px; }
    }
</style>