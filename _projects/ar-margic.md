---
layout: post
title: "MARGIC"
image: "/assets/images/pic04.jpg"
pillar: "augmented-reality"
genre: "marketing"
company: "Creatinno Tech"
hardware: "Mobile"
technologies: ["AR", "Unity"]
project_url: "https://play.google.com/store/apps/details?id=com.creatinno.margic" # Referral link
# video_id: "https://www.youtube.com/watch?v=KfWjFpPtnBU"
---

<div class="project-specs" style="display: grid; grid-template-columns: repeat(auto-fit, minmax(180px, 1fr)); gap: 1rem; background: rgba(155, 241, 255, 0.05); padding: 1.5rem; border-left: 4px solid #9bf1ff; margin-top: -2.5rem; margin-bottom: 2rem; border-radius: 0 8px 8px 0;">
    <div><strong style="font-size: 0.7rem; letter-spacing: 1px;">ROLE</strong><br><span style="color: #9bf1ff; font-weight: 600;">Technical Lead</span></div>
    <div><strong style="font-size: 0.7rem; letter-spacing: 1px;">PLATFORM</strong><br>Unity 2022.3 (URP)</div>
    <div><strong style="font-size: 0.7rem; letter-spacing: 1px;">CORE TECH</strong><br>VPS & Cloud Assets</div>
    <div><strong style="font-size: 0.7rem; letter-spacing: 1px;">PROJECT SITE</strong><br><a href="{{ page.project_url }}" target="_blank" class="button small primary">Try it Now ↗</a></div>
</div>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 2.5rem; align-items: start; margin-bottom: 3rem;">   
    <div>
        <h2 style="margin-top: 0;">The Vision</h2>
        <p><strong>MARGIC</strong> is an AR platform that allows clients to host and share promotional AR content without needing to publish their own app.</p> 
        <p>As <strong>Unity XR Engineer</strong>,  led development and technical implementation of AR features, enabling clients to host, and share promotional AR content seamlessly.</p>     
    </div>
    {% if page.video_id %}
    <div style="background: rgba(255,255,255,0.05); padding: 10px; border-radius: 12px; border: 1px solid rgba(255,255,255,0.1);">
        <div class="video-container" style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; border-radius: 8px;">
            <iframe src="https://www.youtube.com/embed/{{ page.video_id }}" 
                    style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
                    frameborder="0" allowfullscreen></iframe>
        </div>
        <p style="font-size: 0.7rem; text-align: center; margin: 0.5rem 0 0 0; color: #9bf1ff; letter-spacing: 1px; text-transform: uppercase;">
            Technical Demo: VPS Localization
        </p>
    </div>
    {% endif %}
</div>


### 💻 Technical Stack & Expertise
<div class="tech-tags" style="display: flex; flex-wrap: wrap; gap: 0.5rem; margin-top: 1rem; margin-bottom: 3rem;">
    <span style="background: rgba(155, 241, 255, 0.1); color: #9bf1ff; padding: 0.2rem 0.8rem; border-radius: 20px; font-size: 0.8rem; border: 1px solid rgba(155, 241, 255, 0.3);">Unity 2022.3 LTS</span>
    <span style="background: rgba(155, 241, 255, 0.1); color: #9bf1ff; padding: 0.2rem 0.8rem; border-radius: 20px; font-size: 0.8rem; border: 1px solid rgba(155, 241, 255, 0.3);">ARFoundation</span>
    <span style="background: rgba(155, 241, 255, 0.1); color: #9bf1ff; padding: 0.2rem 0.8rem; border-radius: 20px; font-size: 0.8rem; border: 1px solid rgba(155, 241, 255, 0.3);">Google Geospatial API</span>
    <span style="background: rgba(155, 241, 255, 0.1); color: #9bf1ff; padding: 0.2rem 0.8rem; border-radius: 20px; font-size: 0.8rem; border: 1px solid rgba(155, 241, 255, 0.3);">AWS S3</span>
    <span style="background: rgba(155, 241, 255, 0.1); color: #9bf1ff; padding: 0.2rem 0.8rem; border-radius: 20px; font-size: 0.8rem; border: 1px solid rgba(155, 241, 255, 0.3);">Addressables</span>
</div>

> **Leadership Note:** Coordinated a remote team of 3 developers and 1 software agency, conducting weekly code reviews and defining the CI/CD pipeline via GitHub Actions to ensure a 0% regression rate on new features.


### 🛠️ Core Engineering Challenges

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 2rem; margin-bottom: 2rem;">
    <div style="background: rgba(255, 255, 255, 0.02); padding: 1.5rem; border-radius: 8px; border: 1px solid rgba(255,255,255,0.1);">
        <h4 style="color: #9bf1ff; margin-bottom: 0.5rem;">The "Drift" Problem</h4>
        <p style="font-size: 0.9rem; line-height: 1.6;">Standard GPS accuracy ($\pm$10m) is insufficient for historical landmarks. I architected a <strong>Hybrid Localization</strong> system that uses GPS for geofencing and the <strong>Google Geospatial API</strong> for sub-centimeter visual anchoring.</p>
        <span style="font-size: 0.8rem; color: #9bff9b;">✔ Result: Zero asset jittering in variable lighting.</span>
    </div>
    <div style="background: rgba(255, 255, 255, 0.02); padding: 1.5rem; border-radius: 8px; border: 1px solid rgba(255,255,255,0.1);">
        <h4 style="color: #9bf1ff; margin-bottom: 0.5rem;">Mobile Constraints</h4>
        <p style="font-size: 0.9rem; line-height: 1.6;">Outdoor AR causes rapid thermal throttling. I implemented <strong>Custom Frustum Culling</strong> and <strong>LZ4-compressed Addressables</strong> to reduce CPU overhead and storage footprint.</p>
        <span style="font-size: 0.8rem; color: #9bff9b;">✔ Result: 60FPS stability & 60% smaller APK size.</span>
    </div>
</div>



---

### 🏗️ The Architecture: Service-Provider Pattern
To ensure the app remained maintainable for a remote team, I implemented a decoupled system that separates core logic from third-party SDKs.

<div class="table-wrapper">
    <table class="alt" style="font-size: 0.9rem;">
        <thead>
            <tr>
                <th>Layer</th>
                <th>Responsibility</th>
                <th>Implementation</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td><strong>Abstraction</strong></td>
                <td>Location Service</td>
                <td>Interfaces for GPS, Heading, and VPS state.</td>
            </tr>
            <tr>
                <td><strong>Implementation</strong></td>
                <td>Provider Layer</td>
                <td>Swappable modules (Google Geospatial vs. Mapbox).</td>
            </tr>
            <tr>
                <td><strong>Lifecycle</strong></td>
                <td>State Machine</td>
                <td>Managed <em>Explore → Localize → Interact</em> flow.</td>
            </tr>
        </tbody>
    </table>
</div>



---

### 🧠 Architect’s Retrospective

<div style="background: rgba(155, 241, 255, 0.03); border: 1px solid rgba(155, 241, 255, 0.2); padding: 2rem; border-radius: 8px; margin: 2rem 0;">
    <h4 style="color: #9bf1ff; margin-top: 0;">Post-Mortem & Lessons Learned</h4>
    <p style="font-size: 0.95rem;">Building for the "Wild" (outdoor AR) proved that <strong>Environmental UX</strong> is as critical as the code. High-noon sunlight in Malaysia causes aggressive thermal throttling; our next iteration will move tracking logic to background threads more aggressively.</p>
    <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 1.5rem; margin-top: 1.5rem;">
        <div>
            <h5 style="font-size: 0.7rem; letter-spacing: 1px; color: #ff9b9b; text-transform: uppercase;">Technical Debt</h5>
            <ul style="font-size: 0.85rem; padding-left: 1.2rem;">
                <li>Network Edge Cases: Handling 5G to 3G handoffs during asset streaming.</li>
                <li>Device Fragmention: Optimizing depth-sensing for non-LiDAR Android devices.</li>
            </ul>
        </div>
        <div>
            <h5 style="font-size: 0.7rem; letter-spacing: 1px; color: #9bff9b; text-transform: uppercase;">Future Roadmap</h5>
            <ul style="font-size: 0.85rem; padding-left: 1.2rem;">
                <li>Occlusion 2.0: Integrating depth-sensing for crowd integration.</li>
                <li>Light Estimation: Matching AR shadows with real-time solar data.</li>
            </ul>
        </div>
    </div>
</div>

---


<script>
    const carousel = document.getElementById('case-study-carousel');
    const dots = document.querySelectorAll('.dot');
    
    // --- Dot Logic ---
    const updateDots = () => {
        const index = Math.round(carousel.scrollLeft / carousel.offsetWidth);
        dots.forEach((dot, i) => {
            dot.classList.toggle('active', i === index);
        });
    };
    carousel.addEventListener('scroll', updateDots);

    // --- Mouse Drag-to-Scroll Logic ---
    let isDown = false;
    let startX;
    let scrollLeft;

    carousel.addEventListener('mousedown', (e) => {
        isDown = true;
        carousel.style.cursor = 'grabbing';
        carousel.style.scrollSnapType = 'none'; // Temporarily disable snap to allow free drag
        startX = e.pageX - carousel.offsetLeft;
        scrollLeft = carousel.scrollLeft;
    });

    carousel.addEventListener('mouseleave', () => {
        isDown = false;
        carousel.style.cursor = 'grab';
    });

    carousel.addEventListener('mouseup', () => {
        isDown = false;
        carousel.style.cursor = 'grab';
        carousel.style.scrollSnapType = 'x mandatory'; // Re-enable snap
    });

    carousel.addEventListener('mousemove', (e) => {
        if (!isDown) return;
        e.preventDefault();
        const x = e.pageX - carousel.offsetLeft;
        const walk = (x - startX) * 2; // Scroll speed multiplier
        carousel.scrollLeft = scrollLeft - walk;
    });
</script>