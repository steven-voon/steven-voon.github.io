---
layout: post
title: "Dulife Pocket"
image: "/assets/images/pic04.jpg"
pillar: "mobile-app"
genre: "productivity"
company: "Creatinno Tech"
hardware: "Mobile"
technologies: ["Flutter", "Unity", "FERN Stack"]
project_url: "https://www.ceritalah.com" # Referral link
carousel_images: 
  - "/assets/images/pic07.jpg"
  - "/assets/images/pic07.jpg"
  - "/assets/images/pic07.jpg"
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
        <p><strong>Ceritalah</strong> is a location-based AR platform designed to bridge Malaysian history with modern spatial computing.</p> 
        <p>As <strong>Technical Lead</strong>, my goal was to move beyond simple markers and create a "world-scale" AR experience.</p>     
    </div>
    <div style="background: rgba(255,255,255,0.05); padding: 10px; border-radius: 12px; border: 1px solid rgba(255,255,255,0.1); position: relative; overflow: hidden;">         
        <button onclick="document.getElementById('case-study-carousel').scrollBy({left: -document.getElementById('case-study-carousel').offsetWidth, behavior: 'smooth'})" 
            style="position: absolute; left: 25px; top: 50%; transform: translateY(-50%); z-index: 5; background: transparent !important; border: none !important; outline: none !important; box-shadow: none !important; color: white; font-size: 2.2rem; cursor: pointer; text-shadow: 0px 0px 15px rgba(0,0,0,0.9); transition: all 0.3s ease; padding: 10px; min-width: 44px; display: flex; align-items: center; justify-content: center;"
            onmouseover="this.style.opacity='0.6'; this.style.transform='translateY(-50%) scale(1.1)';" 
            onmouseout="this.style.opacity='1'; this.style.transform='translateY(-50%) scale(1)';">
            &#10094;
        </button>
        <button onclick="document.getElementById('case-study-carousel').scrollBy({left: document.getElementById('case-study-carousel').offsetWidth, behavior: 'smooth'})" 
            style="position: absolute; right: 25px; top: 50%; transform: translateY(-50%); z-index: 5; background: transparent !important; border: none !important; outline: none !important; box-shadow: none !important; color: white; font-size: 2.2rem; cursor: pointer; text-shadow: 0px 0px 15px rgba(0,0,0,0.9); transition: all 0.3s ease; padding: 10px; min-width: 44px; display: flex; align-items: center; justify-content: center;"
            onmouseover="this.style.opacity='0.6'; this.style.transform='translateY(-50%) scale(1.1)';" 
            onmouseout="this.style.opacity='1'; this.style.transform='translateY(-50%) scale(1)';">
            &#10095;
        </button>
        <div id="case-study-carousel" class="carousel-container" style="cursor: grab;">
            {% for img in page.carousel_images %}
            <div class="carousel-item">
                <img src="{{ img }}" alt="Project slide" style="pointer-events: none; -webkit-user-drag: none;">
            </div>
            {% endfor %}
        </div>
        <style>
            .dot { 
                width: 6px; height: 6px; border-radius: 50%; 
                background: rgba(155, 241, 255, 0.3); transition: all 0.3s ease; 
            }
            .dot.active { 
                background: #9bf1ff !important; 
                box-shadow: 0 0 8px #9bf1ff; transform: scale(1.3); 
            }
        </style>
        <div class="carousel-dots" style="display: flex; justify-content: center; gap: 8px; margin-top: 10px;">
            {% for img in page.carousel_images %}
            <div class="dot {% if forloop.first %}active{% endif %}"></div>
            {% endfor %}
        </div>                 
        <p style="font-size: 0.7rem; text-align: center; margin: 0.5rem 0 0 0; color: #9bf1ff; letter-spacing: 1px; text-transform: uppercase; opacity: 0.6;">
            Swipe or use arrows to view
        </p>
    </div>
</div>