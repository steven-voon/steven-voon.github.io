---
layout: post
title: "No More Lazy Eyes (VR Amblyopia Treatment POC)"
image: "/assets/images/pic04.jpg"
pillar: "virtual-reality"
genre: "healthcare"
company: "Creatinno Tech"
hardware: "Meta Quest 3"
technologies: ["Unity", "OpenXR"]
project_url: "https://sidequestvr.com/app/53740/no-more-lazy-eyes"
video_id: "https://www.youtube.com/watch?v=h3KoZ5dodtY"
---

<div class="project-specs" style="display: grid; grid-template-columns: repeat(auto-fit, minmax(180px, 1fr)); gap: 1rem; background: rgba(155, 241, 255, 0.05); padding: 1.5rem; border-left: 4px solid #9bf1ff; margin-top: -2.5rem; margin-bottom: 2rem; border-radius: 0 8px 8px 0;">
    <div><strong style="font-size: 0.7rem; letter-spacing: 1px;">ROLE</strong><br><span style="color: #9bf1ff; font-weight: 600;">Technical Lead</span></div>
    <div><strong style="font-size: 0.7rem; letter-spacing: 1px;">PLATFORM</strong><br>Unity 6.0 (LTS)</div>
    <div><strong style="font-size: 0.7rem; letter-spacing: 1px;">CORE TECH</strong><br>OpenXR & XR Interaction Toolkit</div>
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

<h3 style="display: flex; align-items: center; gap: 12px; color: #ffffff; margin-top: 3rem;">
    <span style="width: 30px; height: 2px; background: #9bf1ff; display: inline-block;"></span>
    <span style="letter-spacing: 1px; text-transform: uppercase; font-size: 0.9rem; color: #9bf1ff;">Engineering Deep-Dive</span>
</h3>
<h2 style="font-size: 2rem; margin-top: 0.5rem; color: #ffffff;">Core Engineering Challenges</h2>
### 💻 Technical Stack & Expertise
<div class="tech-tags" style="display: flex; flex-wrap: wrap; gap: 0.5rem; margin-top: 1rem; margin-bottom: 3rem;">
    <span style="background: rgba(155, 241, 255, 0.1); color: #9bf1ff; padding: 0.2rem 0.8rem; border-radius: 20px; font-size: 0.8rem; border: 1px solid rgba(155, 241, 255, 0.3);">Unity 6.0 (URP)</span>
    <span style="background: rgba(155, 241, 255, 0.1); color: #9bf1ff; padding: 0.2rem 0.8rem; border-radius: 20px; font-size: 0.8rem; border: 1px solid rgba(155, 241, 255, 0.3);">OpenXR</span>
    <span style="background: rgba(155, 241, 255, 0.1); color: #9bf1ff; padding: 0.2rem 0.8rem; border-radius: 20px; font-size: 0.8rem; border: 1px solid rgba(155, 241, 255, 0.3);">C#</span>
    <span style="background: rgba(155, 241, 255, 0.1); color: #9bf1ff; padding: 0.2rem 0.8rem; border-radius: 20px; font-size: 0.8rem; border: 1px solid rgba(155, 241, 255, 0.3);">Blender</span>
    <span style="background: rgba(155, 241, 255, 0.1); color: #9bf1ff; padding: 0.2rem 0.8rem; border-radius: 20px; font-size: 0.8rem; border: 1px solid rgba(155, 241, 255, 0.3);">GIMP</span>
</div>

> **Leadership Note:** Oversight of the end-to-end technical architecture was maintained, ensuring the integration of custom shaders with XR interaction protocols.

<h3 style="display: flex; align-items: center; gap: 12px; color: #ffffff; margin-top: 3rem;">
    <span style="width: 30px; height: 2px; background: #9bf1ff; display: inline-block;"></span>
    <span style="letter-spacing: 1px; text-transform: uppercase; font-size: 0.9rem; color: #9bf1ff;">Engineering Deep-Dive</span>
</h3>
<h2 style="font-size: 2rem; margin-top: 0.5rem; color: #ffffff;">Core Engineering Challenges</h2>
### 🛠️ Core Engineering Challenges
<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 2rem; margin-bottom: 2rem;">
    <div style="background: rgba(255, 255, 255, 0.03); padding: 1.75rem; border-radius: 12px; border: 1px solid rgba(255,255,255,0.1); display: flex; flex-direction: column; gap: 1rem;">
        <h4 style="color: #9bf1ff; margin: 0; font-size: 1.5rem; font-weight: 600; letter-spacing: -0.01em;">Dichoptic Rendering</h4>
        <div style="font-size: 1rem; line-height: 1.6; color: rgba(255,255,255,0.85);">
            <p style="margin: 0 0 0.75rem 0;">Standard rendering pipelines do not inherently support per-eye object culling without costly dual-camera setups that impact mobile XR performance.</p>
            <p style="margin: 0;">A custom shader and layer-masking architecture was developed. "Bombs" are assigned to a unique layer visible only to the Left Eye, while "Traps" are restricted to the Right Eye.</p>
        </div>
        <div style="margin-top: auto; padding-top: 1rem; border-top: 1px solid rgba(255,255,255,0.1); font-size: 0.95rem; color: #9bff9b; line-height: 1.5; display: flex; align-items: flex-start; gap: 0.6rem;">
            <span>✔ Result: Achieved absolute visual separation with zero "leakage" between ocular channels.</span>
        </div>
    </div>
        <div style="background: rgba(255, 255, 255, 0.03); padding: 1.75rem; border-radius: 12px; border: 1px solid rgba(255,255,255,0.1); display: flex; flex-direction: column; gap: 1rem;">
        <h4 style="color: #9bf1ff; margin: 0; font-size: 1.5rem; font-weight: 600; letter-spacing: -0.01em;">Event-Driven Interaction Pipeline</h4>
        <div style="font-size: 1rem; line-height: 1.6; color: rgba(255,255,255,0.85);">
            <p style="margin: 0 0 0.75rem 0;">The system required a decoupled method for the UI and scoring logic to react to collisions across 39 potential spawn spots.</p>
            <p style="margin: 0;">The architecture utilizes an Event-Driven Architecture (EDA). The ObstacleController broadcasts collision payloads via a central event bus, which the ResultManager and UI listeners consume independently.</p>
        </div>
        <div style="margin-top: auto; padding-top: 1rem; border-top: 1px solid rgba(255,255,255,0.1); font-size: 0.95rem; color: #9bff9b; line-height: 1.5; display: flex; align-items: flex-start; gap: 0.6rem;">
            <span>✔ Result: Reduced script dependencies by 40% and simplified the debugging of the scoring logic.</span>
        </div>
    </div>
        <div style="background: rgba(255, 255, 255, 0.03); padding: 1.75rem; border-radius: 12px; border: 1px solid rgba(255,255,255,0.1); display: flex; flex-direction: column; gap: 1rem;">
        <h4 style="color: #9bf1ff; margin: 0; font-size: 1.5rem; font-weight: 600; letter-spacing: -0.01em;">High-Speed Lane Navigation</h4>
        <div style="font-size: 1rem; line-height: 1.6; color: rgba(255,255,255,0.85);">
            <p style="margin: 0 0 0.75rem 0;">Translating a cart across three lanes based on thumbstick input requires precise snapping and low latency.</p>
            <p style="margin: 0;">A SwitchLaneController was implemented to map XR Input to localized lane coordinates on a spline-based track.</p>
        </div>
        <div style="margin-top: auto; padding-top: 1rem; border-top: 1px solid rgba(255,255,255,0.1); font-size: 0.95rem; color: #9bff9b; line-height: 1.5; display: flex; align-items: flex-start; gap: 0.6rem;">
            <span>✔ Result: Locked 90fps performance on Meta Quest 3 with sub-20ms input response time.</span>
        </div>
    </div>
</div>

<h3 style="display: flex; align-items: center; gap: 12px; color: #ffffff; margin-top: 3rem;">
    <span style="width: 30px; height: 2px; background: #9bf1ff; display: inline-block;"></span>
    <span style="letter-spacing: 1px; text-transform: uppercase; font-size: 0.9rem; color: #9bf1ff;">Engineering Deep-Dive</span>
</h3>
<h2 style="font-size: 2rem; margin-top: 0.5rem; color: #ffffff;">Core Engineering Challenges</h2>
### 🏗️ The Architecture: Event-Driven Architecture
<div class="table-wrapper">
    <table class="alt" style="font-size: 0.9rem;">
        <thead>
            <tr>
                <th>System Component</th>
                <th>Responsibility</th>
                <th>Implemented Pattern</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td><strong>MainManager</strong></td>
                <td>Orchestrates global game states and UI flow based on user progression.</td>
                <td>Singleton</td>
            </tr>
            <tr>
                <td><strong>SpawnManager</strong></td>
                <td>Manages procedural distribution of 2 obstacles and 1 safe spot across 3 spots per node.</td>
                <td>Randomization Factory</td>
            </tr>
            <tr>
                <td><strong>ResultManager</strong></td>
                <td>Aggregates session metrics: total spawns, specific obstacle hits, and successful safe spot captures.</td>
                <td>Observer Pattern</td>
            </tr>
              <tr>
                <td><strong>SwitchLaneController</strong></td>
                <td>Intercepts XR thumbstick data to execute smooth, localized lane-switching maneuvers.</td>
                <td>Input-to-Action Mapping</td>
            </tr>
              <tr>
                <td><strong>ObstacleController</strong></td>
                <td>Detects physical intersections and broadcasts collision payloads to the event bus.</td>
                <td>Event Broadcaster</td>
            </tr>
        </tbody>
    </table>
</div>


### 🧠 Architect’s Retrospective

<div style="background: rgba(155, 241, 255, 0.03); border: 1px solid rgba(155, 241, 255, 0.2); padding: 2rem; border-radius: 8px; margin: 2rem 0;">
    <h4 style="color: #9bf1ff; margin-top: 0;">Post-Mortem & Lessons Learned</h4>
    <p style="font-size: 0.95rem;">The system employs a Dichoptic Event-Driven Architecture to treat amblyopia by isolating visual stimuli. A procedural spawner generates 13 rows of obstacles, utilizing a 3-lane snap-movement system to minimize cognitive load and maximize focus on binocular integration. By decoupling the Spawner, Vision Manager, and Analytics via an event bus, the system ensures data integrity. Scene reloading is utilized as the primary lifecycle anchor to guarantee a stable, clean state for every  session.</p>
    <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 1.5rem; margin-top: 1.5rem;">
        <div>
            <h5 style="font-size: 0.7rem; letter-spacing: 1px; color: #ff9b9b; text-transform: uppercase;">Technical Debt</h5>
            <ul style="font-size: 0.85rem; padding-left: 1.2rem;">
                <li>Session Restart: Restarting a session utilizes a full scene reload. This is computationally expensive and introduces unnecessary latency and glitches. Refactoring to an Object Pooling and state-reset system</li>
            </ul>
            <ul style="font-size: 0.85rem; padding-left: 1.2rem;">
                <li>Hard-Coded Spawning: Spawn managers are currently static assignments. This limits track scalability. Transitioning to a dynamic, distance-based spawning system would allow for infinite or procedurally generated treatment tracks</li>
            </ul>
             <ul style="font-size: 0.85rem; padding-left: 1.2rem;">
                <li>Layer Dependency: The dichoptic effect relies on specific Unity Layer indices. This is brittle; moving to a Renderer Feature approach would provide more robust control over eye-specific culling.</li>
            </ul>
        </div>
        <div>
            <h5 style="font-size: 0.7rem; letter-spacing: 1px; color: #9bff9b; text-transform: uppercase;">Future Roadmap</h5>
            <ul style="font-size: 0.85rem; padding-left: 1.2rem;">
                <li>Dynamic Difficulty Adjustment (DDA): Implementation of an algorithm to adjust cart speed and obstacle frequency based on real-time hit/miss ratios.</li>
            </ul>
            <ul style="font-size: 0.85rem; padding-left: 1.2rem;">
                <li>Analytics Integration: Development of a secure local database to track player progress over multiple sessions for review.</li>
            </ul>
             <ul style="font-size: 0.85rem; padding-left: 1.2rem;">
                <li>Advanced Calibration: Addition of a pre-game UI to calibrate shader alpha levels, to cope for patients with different levels of suppression.</li>
            </ul>
        </div>
    </div>
</div>

---