---
layout: post
title: "No More Lazy Eyes (VR Amblyopia Treatment POC)"
image: "/assets/images/pic04.jpg"
pillar: "virtual-reality"
genre: "healthcare"
company: "Creatinno Tech"
hardware: "Meta Quest 3"
technologies: ["Unit", "OpenXR"]
project_url: "https://sidequestvr.com/app/53740/no-more-lazy-eyes"
video_id: "https://www.youtube.com/watch?v=h3KoZ5dodtY"
---

<div class="project-specs" style="display: grid; grid-template-columns: repeat(auto-fit, minmax(180px, 1fr)); gap: 1rem; background: rgba(155, 241, 255, 0.05); padding: 1.5rem; border-left: 4px solid #9bf1ff; margin-top: -2.5rem; margin-bottom: 2rem; border-radius: 0 8px 8px 0;">
    <div><strong style="font-size: 0.7rem; letter-spacing: 1px;">ROLE</strong><br><span style="color: #9bf1ff; font-weight: 600;">Technical Lead</span></div>
    <div><strong style="font-size: 0.7rem; letter-spacing: 1px;">PLATFORM</strong><br>Unity 6000.0.59f2 (URP)</div>
    <div><strong style="font-size: 0.7rem; letter-spacing: 1px;">CORE TECH</strong><br>OpenXR</div>
    <div><strong style="font-size: 0.7rem; letter-spacing: 1px;">LIVE SITE</strong><br><a href="{{ page.project_url }}" target="_blank" class="button small primary">Visit Project ↗</a></div>
</div>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 2.5rem; align-items: start; margin-bottom: 3rem;">   
    <div>
        <h2 style="margin-top: 0;">The Vision</h2>
        <p><strong>No More Lazy Eyes</strong> is a gamified XR proof-of-concept that uses a custom dichoptic rendering system to facilitate binocular vision therapy through interactive gameplay.</p> 
        <p>As <strong>Techincal Lead cum XR Engineer</strong>, my goal was to architected the dual-track rendering pipeline, engineered the core game logic, and developed calibration and data-logging systems to track coordination metrics.</p>     
    </div>
    {% if page.video_id %}
    <div style="background: rgba(255,255,255,0.05); padding: 10px; border-radius: 12px; border: 1px solid rgba(255,255,255,0.1);">
        <div class="video-container" style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; border-radius: 8px;">
            <iframe src="https://www.youtube.com/embed/{{ page.video_id }}" 
                    style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
                    frameborder="0" allowfullscreen></iframe>
        </div>
        <p style="font-size: 0.7rem; text-align: center; margin: 0.5rem 0 0 0; color: #9bf1ff; letter-spacing: 1px; text-transform: uppercase;">
            Technical Demo: POC for VR Amblyopia Treatment
        </p>
    </div>
    {% endif %}
</div>


### 💻 Technical Stack & Expertise
<div class="tech-tags" style="display: flex; flex-wrap: wrap; gap: 0.5rem; margin-top: 1rem; margin-bottom: 3rem;">
    <span style="background: rgba(155, 241, 255, 0.1); color: #9bf1ff; padding: 0.2rem 0.8rem; border-radius: 20px; font-size: 0.8rem; border: 1px solid rgba(155, 241, 255, 0.3);">Unity 6.000 LTS</span>
    <span style="background: rgba(155, 241, 255, 0.1); color: #9bf1ff; padding: 0.2rem 0.8rem; border-radius: 20px; font-size: 0.8rem; border: 1px solid rgba(155, 241, 255, 0.3);">OpenXR</span>
    <span style="background: rgba(155, 241, 255, 0.1); color: #9bf1ff; padding: 0.2rem 0.8rem; border-radius: 20px; font-size: 0.8rem; border: 1px solid rgba(155, 241, 255, 0.3);">C#</span>
    <span style="background: rgba(155, 241, 255, 0.1); color: #9bf1ff; padding: 0.2rem 0.8rem; border-radius: 20px; font-size: 0.8rem; border: 1px solid rgba(155, 241, 255, 0.3);">Blender</span>
</div>

> **Leadership Note:** Overseeing the fusion of game-feel and dichoptic mechanics to ensure technical stability and project alignment.

### 🛠️ Core Engineering Challenges

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 2rem; margin-bottom: 2rem;">
    <div style="background: rgba(255, 255, 255, 0.02); padding: 1.5rem; border-radius: 8px; border: 1px solid rgba(255,255,255,0.1);">
        <h4 style="color: #9bf1ff; margin-bottom: 0.5rem;">Dichoptic Separation</h4>
        <p style="font-size: 0.9rem; line-height: 1.6;">Preventing "visual leakage" so the left eye never sees the right eye’s traps (and vice versa) despite high-speed movement.</p>
        <span style="font-size: 0.8rem; color: #9bff9b;">✔ Result: Closing one eye results in the complete disappearance of its assigned obstacles (bombs or traps). No "ghosting" or faint outlines are visible.</span>
    </div>
    <div style="background: rgba(255, 255, 255, 0.02); padding: 1.5rem; border-radius: 8px; border: 1px solid rgba(255,255,255,0.1);">
        <h4 style="color: #9bf1ff; margin-bottom: 0.5rem;">Performance Stability</h4>
        <p style="font-size: 0.9rem; line-height: 1.6;">Maintaining a high, locked frame rate (60fps+) to prevent motion sickness caused by the brain processing two different data streams.</p>
        <span style="font-size: 0.8rem; color: #9bff9b;">✔ Result: Maintains a stable frame rate (a constant 60fps on Meta Quest 3) with zero dropped frames during high-speed movement.</span>
    </div>
</div>

### 🧠 Architect’s Retrospective

<div style="background: rgba(155, 241, 255, 0.03); border: 1px solid rgba(155, 241, 255, 0.2); padding: 2rem; border-radius: 8px; margin: 2rem 0;">
    <h4 style="color: #9bf1ff; margin-top: 0;">Post-Mortem & Lessons Learned</h4>
    <p style="font-size: 0.95rem;">The system employs a Dichoptic Event-Driven Architecture to treat amblyopia by isolating visual stimuli. A procedural spawner generates 13 rows of obstacles, utilizing a 3-lane snap-movement system to minimize cognitive load and maximize focus on binocular integration. By decoupling the Spawner, Vision Manager, and Analytics via an event bus, the system ensures medical data integrity. Scene reloading is utilized as the primary lifecycle anchor to guarantee a stable, clean state for every therapeutic session.</p>
    <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 1.5rem; margin-top: 1.5rem;">
        <div>
            <h5 style="font-size: 0.7rem; letter-spacing: 1px; color: #ff9b9b; text-transform: uppercase;">Technical Debt</h5>
            <ul style="font-size: 0.85rem; padding-left: 1.2rem;">
                <li>Hard-Coded Spawn Point: The 13-spawn point, 3-lane grid is currently hard-coded, adjusting difficulty (rows/lanes) currently requires a code refactor rather than a configuration change.</li>
            </ul>
            <ul style="font-size: 0.85rem; padding-left: 1.2rem;">
                <li>Static Layer Assignment: Eye-to-obstacle mapping is fixed, making it difficult to swap "weak eye" targets without manual script adjustments.</li>
            </ul>
        </div>
        <div>
            <h5 style="font-size: 0.7rem; letter-spacing: 1px; color: #9bff9b; text-transform: uppercase;">Future Roadmap</h5>
            <ul style="font-size: 0.85rem; padding-left: 1.2rem;">
                <li>Dynamic Difficulty Adjustment (DDA): Automatically decrease obstacle speed or increase contrast for the "weak eye" if the reporting system detects high failure rates.</li>
            </ul>
            <ul style="font-size: 0.85rem; padding-left: 1.2rem;">
                <li>Clinical Dashboard: Implement web-based dashboard for the reporting system so clinicians can monitor progress remotely without manual file extraction.</li>
            </ul>
             <ul style="font-size: 0.85rem; padding-left: 1.2rem;">
                <li>Visual Comfort Vignette: Apply a dynamic FOV mask during lane switching to further mitigate motion sickness for sensitive users.</li>
            </ul>
        </div>
    </div>
</div>

---