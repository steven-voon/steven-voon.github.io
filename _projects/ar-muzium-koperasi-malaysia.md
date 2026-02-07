---
layout: post
title: "Muzium Koperasi Malaysia"
image: "/assets/images/pic04.jpg"
pillar: "augmented-reality"
genre: "heritage"
company: "Creatinno Tech"
hardware: "Mobile"
technologies: ["Unity", "ARCore", "ARKit", "C#", "Blender"]
project_url: "https://www.ceritalah.com"
video_id: "https://www.youtube.com/watch?v=GIYklSH7qoA&list=PLfLzhRAcLiXRHTuJPkCSowJI48C6dzXj0&index=1"
---

<div class="project-specs" style="display: grid; grid-template-columns: repeat(auto-fit, minmax(180px, 1fr)); gap: 1rem; background: rgba(155, 241, 255, 0.05); padding: 1.5rem; border-left: 4px solid #9bf1ff; margin-top: -2.5rem; margin-bottom: 2rem; border-radius: 0 8px 8px 0;">
    <div><strong style="font-size: 0.7rem; letter-spacing: 1px;">ROLE</strong><br><span style="color: #9bf1ff; font-weight: 600;">Technical Lead</span></div>
    <div><strong style="font-size: 0.7rem; letter-spacing: 1px;">PLATFORM</strong><br>Unity 2022.3 (URP)</div>
    <div><strong style="font-size: 0.7rem; letter-spacing: 1px;">CORE TECH</strong><br>VPS & Cloud Assets</div>
    <div><strong style="font-size: 0.7rem; letter-spacing: 1px;">LIVE SITE</strong><br><a href="{{ page.project_url }}" target="_blank" class="button small primary">Visit Project ↗</a></div>
</div>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 2.5rem; align-items: start; margin-bottom: 3rem;">   
    <div>
        <h2 style="margin-top: 0;">The Vision</h2>
        <p><strong>Muzium Koperasi Malaysia</strong> is an interactive AR app showcasing historical moment of the organisation (ANGKASA) and showcase their batik collection.</p> 
        <p>As <strong>Technical Lead cum XR Engineer</strong>, my goal was to recreate the historical moment of one of the annual meeting and design a interactive photo session for their batik collectiont. </p>     
    </div>
    {% if page.video_id %}
    <div style="background: rgba(255,255,255,0.05); padding: 10px; border-radius: 12px; border: 1px solid rgba(255,255,255,0.1);">
        <div class="video-container" style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; border-radius: 8px;">
            <iframe src="https://www.youtube.com/embed/{{ page.video_id }}" 
                    style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
                    frameborder="0" allowfullscreen></iframe>
        </div>
        <p style="font-size: 0.7rem; text-align: center; margin: 0.5rem 0 0 0; color: #9bf1ff; letter-spacing: 1px; text-transform: uppercase;">
            Technical Demo: AR Portal Effect & Batik Photo Session
        </p>
    </div>
    {% endif %}
</div>


### 💻 Technical Stack & Expertise
<div class="tech-tags" style="display: flex; flex-wrap: wrap; gap: 0.5rem; margin-top: 1rem; margin-bottom: 3rem;">
    <span style="background: rgba(155, 241, 255, 0.1); color: #9bf1ff; padding: 0.2rem 0.8rem; border-radius: 20px; font-size: 0.8rem; border: 1px solid rgba(155, 241, 255, 0.3);">Unity 6.000 LTS</span>
    <span style="background: rgba(155, 241, 255, 0.1); color: #9bf1ff; padding: 0.2rem 0.8rem; border-radius: 20px; font-size: 0.8rem; border: 1px solid rgba(155, 241, 255, 0.3);">ARCore</span>
    <span style="background: rgba(155, 241, 255, 0.1); color: #9bf1ff; padding: 0.2rem 0.8rem; border-radius: 20px; font-size: 0.8rem; border: 1px solid rgba(155, 241, 255, 0.3);">ARKit</span>
    <span style="background: rgba(155, 241, 255, 0.1); color: #9bf1ff; padding: 0.2rem 0.8rem; border-radius: 20px; font-size: 0.8rem; border: 1px solid rgba(155, 241, 255, 0.3);">C#</span>
    <span style="background: rgba(155, 241, 255, 0.1); color: #9bf1ff; padding: 0.2rem 0.8rem; border-radius: 20px; font-size: 0.8rem; border: 1px solid rgba(155, 241, 255, 0.3);">Blender</span>
</div>

> **Leadership Note:** Perform technical feasibility study on requirement and advise appropriate tech stack. Identify technical limitation and advise workaround.

### 🛠️ Core Engineering Challenges

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 2rem; margin-bottom: 2rem;">
    <div style="background: rgba(255, 255, 255, 0.02); padding: 1.5rem; border-radius: 8px; border: 1px solid rgba(255,255,255,0.1);">
        <h4 style="color: #9bf1ff; margin-bottom: 0.5rem;">Recreating the historical site with crowds</h4>
        <p style="font-size: 0.9rem; line-height: 1.6;">Computational Heavy for crowd simulation. Techniques such as static batching, GPU instancing, occlusion culling is used for memory optimization.</p>
        <span style="font-size: 0.8rem; color: #9bff9b;">✔ Result: Fit in 100 crowds in the hall, running smooth on device with 50 FPS.</span>
    </div>
    <div style="background: rgba(255, 255, 255, 0.02); padding: 1.5rem; border-radius: 8px; border: 1px solid rgba(255,255,255,0.1);">
        <h4 style="color: #9bf1ff; margin-bottom: 0.5rem;">Stencil Shader Portal Optimization</h4>
        <p style="font-size: 0.9rem; line-height: 1.6;">Stencil Shader is used to create portal effect, however when user pass through the portal, there will be a short moment of visible glitches/flash. Create a dummy visual to be displayed  when user outside of the portal, then activate the real visual when user are inside the portal. </p>
        <span style="font-size: 0.8rem; color: #9bff9b;">✔ Result: Smooht transition when going in and out of the portal</span>
    </div>
</div>



---

### 🏗️ The Architecture: Service-Provider Pattern
To ensure the batik collection can be easily expand afterward, a data system using scriptable object is designed that make content maintenance easy.

<div class="table-wrapper">
    <table class="alt" style="font-size: 0.9rem;">
        <thead>
            <tr>
                <th>Aspect</th>
                <th>Concept/Design</th>
                <th>Implementation</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td><strong>Abstraction</strong></td>
                <td>Batik Data</td>
                <td>Design data structure for each batik collection, such as texture and release year. The customization parameter is also included, such as tudung color.</td>
            </tr>
            <tr>
                <td><strong>Data Class</strong></td>
                <td>Batik Collection Class</td>
                <td>Implement a class that stores batik collection with its own custom parameter.</td>
            </tr>
            <tr>
                <td><strong>Realtime Switching Batik</strong></td>
                <td>Batik Manager</td>
                <td>Batik weared by the model is switchable between gender and custom parameter like tudung color for female.</td>
            </tr>
        </tbody>
    </table>
</div>


---

### 🧠 Architect’s Retrospective

<div style="background: rgba(155, 241, 255, 0.03); border: 1px solid rgba(155, 241, 255, 0.2); padding: 2rem; border-radius: 8px; margin: 2rem 0;">
    <h4 style="color: #9bf1ff; margin-top: 0;">Post-Mortem & Lessons Learned</h4>
    <p style="font-size: 0.95rem;">Initially, batik session was planned to implement using ARKit Body Tracking, however the algorithm is not ready to production level as the tracking of the joint drift significant when user changing from pose and pose. Meanwhile, there is no way to map batik clothing onto user body perfectly as body shape and height differ from one to another.</p>
    
    <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 1.5rem; margin-top: 1.5rem;">
        <div>
            <h5 style="font-size: 0.7rem; letter-spacing: 1px; color: #ff9b9b; text-transform: uppercase;">Technical Debt</h5>
            <ul style="font-size: 0.85rem; padding-left: 1.2rem;">
                <li>Body Tracking: Mapping cloth onto user body regardless of body shape or height..</li>
            </ul>
        </div>
        <div>
            <h5 style="font-size: 0.7rem; letter-spacing: 1px; color: #9bff9b; text-transform: uppercase;">Future Roadmap</h5>
            <ul style="font-size: 0.85rem; padding-left: 1.2rem;">
                <li>AI Body Tracking: Using AI to process user body and map cloth onto user body regardless of body shape or height..</li>
            </ul>
        </div>
    </div>
</div>

---