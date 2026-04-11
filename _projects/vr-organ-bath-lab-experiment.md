---
layout: project-default
title: "VR Organ Bath Lab Experiement"
image: "/assets/images/pic04.jpg"
pillar: "virtual-reality"
genre: "education"
company: "Creatinno Tech"
company_url: "https://www.maitreehouse.com/"
hardware: "Meta Quest 2"
technologies: ["Tiltbrush", "Unity", "Oculus SDK"]
project_url: "https://papers.iafor.org/wp-content/uploads/papers/ace2023/ACE2023_76065.pdf?t=8"

#Project Achievements
achievements:
  - title: "Featured on Media"
    icon: "🖼️"
    url: "https://www.ceritalah.app/"
  - title: "Featured on Media"
    icon: "📰"
    url: "https://www.ceritalah.app/"
  - title: "XR Summit Malaysia Showcase"
    icon: "🎤"
    url: "https://www.ceritalah.app/"

# PROJECT DETAILS
project_role: "Technical Producer"
project_team_size: "2"
project_timeline: "2 Years"
project_timeline_detail: "R&D • Proto • Live"
project_platform: "60 FPS"

# PROJECT GALLERY
# VIDEO (COMMENT THIS OUT IF VIDEO IS NOT AVAILABLE)
# video_id: "KfWjFpPtnBU"
# video_type: "youtube"
# IMAGES (COMMENT THIS OUT IF IMAGES ARE NOT AVAILABLE)
project_images: 
  - "/assets/images/vrobl-ss1.png"
  - "/assets/images/vrobl-ss2.png"
  - "/assets/images/vrobl-ss3.png"
  - "/assets/images/vrobl-ss4.png"
  - "/assets/images/vrobl-ss5.png"
  - "/assets/images/vrobl-ss6.png"
  - "/assets/images/vrobl-ss7.png"
media_caption: "Heritage Storytelling with Augmented Reality (AR)"

# STRATEGIC INTENT
project_strategic_intent:
  title: "STRATEGIC INTENT"
  project_summary:
    heading: "PROJECT SUMMARY"
    content: "Ceritalah is a digital heritage platform using AR to bring local history and stories to life, connecting travelers with communities and cultural experiences across Malaysia."
  mission_impact:
    heading: "MISSION & IMPACT"
    content: "Led technical execution, coordinated workflows across teams, and ensured seamless integration of heritage storytelling with immersive technology."

# TECHNICAL LEADERSHIP
project_technical_leadership:
  title: "TECHNICAL LEADERSHIP"
  overview: "Coordinated a remote team of 3 developers and 1 software agency, conducting weekly code reviews and defining the CI/CD pipeline via GitHub Actions to ensure a 0% regression rate on new features."
  key_points:
    - title: "Weekly Syncs"
      description: "Sprint goals & blockers."
    - title: "QA Gatekeeper"
      description: "Code & asset reviews."
    - title: "CI/CD Workflow"
      description: "Enforced 0% regression."

# TECHNICAL ARCHITECTURE
project_technical_architecture:
  title: "TECHNICAL ARCHITECTURE"
  sections:
    - label: "Core Engine"
      tags: ["Unity 2022.3 LTS", "ARFoundation"]
    - label: "Infrastructure"
      tags: ["AWS S3", "Addressables", "Unity Cloud"]
    - label: "Production"
      tags: ["GitHub CI/CD", "Clickup", "Figma"]

# TECHNICAL CHALLENGES
project_challenges:
  title: "TECHNICAL DEEP-DIVE"
  challenges:
    - title: "The Drift Problem"
      description: "Standard GPS accuracy is insufficient for historical landmarks. I architected a Hybrid Localization system that uses GPS for geofencing and the Google Geospatial API for sub-centimeter visual anchoring."
      result: "Zero asset jittering in variable lighting."
      color: "#ff9b9b"
    - title: "Performance"
      description: "Outdoor AR causes rapid thermal throttling. I implemented <strong>Custom Frustum Culling</strong> and <strong>LZ4-compressed Addressables</strong> to reduce CPU overhead and storage footprint."
      result: "60FPS stability & 60% smaller APK size."
      color: "#9bf1ff"
    - title: "Strategic UX"
      description: "Solved User Placement friction."
      result: "Ghosting guide system."
      color: "#ffcc66"

# PROJECT RETROSPECTIVE
project_retrospective:
  title: "PROJECT RETROSPECTIVE"
  technical_debt:
    - "Network Edge Cases: Handling 5G to 3G handoffs during asset streaming."
    - "Device Fragmention: Optimizing depth-sensing for non-LiDAR Android devices."
  future_roadmap:
    - "Occlusion 2.0: Integrating depth-sensing for crowd integration."
    - "Light Estimation: Matching AR shadows with real-time solar data."
  verdict: "Building for the Wild (outdoor AR) proved that Environmental UX is as critical as the code. High-noon sunlight in Malaysia causes aggressive thermal throttling; our next iteration will move tracking logic to background threads more aggressively."
---

<!-- Main content goes here in markdown format -->