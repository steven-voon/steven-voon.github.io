---
layout: page
title: Project Archive
description: "A comprehensive index of XR architectures, R&D experiments, and technical leadership."
---

{% assign all_items = site.projects | concat: site.lab | sort: 'date' | reverse %}

<section id="main" class="wrapper">
    <div class="inner">
        <header class="major">
            <h1>The Full Index</h1>
        </header>
        <div class="archive-filters" style="margin-bottom: 2rem;">
            <button class="filter-btn active" data-filter="all">All</button>
            <button class="filter-btn" data-filter="virtual-reality">Virtual Reality</button>
            <button class="filter-btn" data-filter="augmented-reality">Augmented Reality</button>
            <button class="filter-btn" data-filter="others">App & Web & Games</button>
            <button class="filter-btn" data-filter="lab">Experimental</button>
        </div>
        <div class="table-wrapper">
            <table class="alt archive-table" style="font-size: 0.85rem;">
                <thead>
                    <tr>
                        <th style="padding: 0.7rem 0.5rem;">Year</th>
                        <th style="padding: 0.7rem 0.5rem;">Project Name</th>
                        <th style="padding: 0.7rem 0.5rem;">Company</th>
                        <th style="padding: 0.7rem 0.5rem;">Category</th>
                        <th style="padding: 0.7rem 0.5rem; text-align: center;">Link</th>
                        <th style="padding: 0.7rem 0.5rem; text-align: center;">Action</th>
                    </tr>
                </thead>
                <tbody>
                    {% for item in all_items %}
                    <tr class="archive-row {% if item.pillar %}{% for p in item.pillar %}{{ p | slugify }} {% endfor %}{% endif %}">
                        <td style="padding: 0.6rem 0.5rem; color: #9bf1ff; font-weight: 600;">{{ item.date | date: "%Y" }}</td>
                        <td style="padding: 0.6rem 0.5rem; font-size: 1.1rem;"><strong>{{ item.title }}</strong></td>
                        <td style="padding: 0.6rem 0.5rem; opacity: 0.8;">{{ item.company | default: "Freelance" }}</td>                   
                        <td style="padding: 0.6rem 0.5rem;">
                            {% if item.status %}
                                <div class="status-container">
                                    <span class="status-dot {{ item.status | slugify }}"></span>
                                    <span class="status-text" style="font-size: 0.7rem;">{{ item.status | replace: "-", " " }}</span>
                                </div>
                            {% else %}
                                <span style="opacity: 0.2;">—</span>
                            {% endif %}
                        </td>
                        <td style="padding: 0.6rem 0.5rem; text-transform: uppercase; font-size: 0.75rem; letter-spacing: 1px;">
                            {{ item.genre }}
                        </td>
                        <td style="padding: 0.6rem 0.5rem; text-align: center;">
                            {% if item.project_url %}
                                <a href="{{ item.project_url }}" target="_blank" style="border: none; color: #9bf1ff; font-size: 1.2rem;">↗</a>
                            {% else %}
                                <span style="opacity: 0.2;">—</span>
                            {% endif %}
                        </td>
                        <td style="padding: 0.6rem 0.5rem; text-align: center;">
                            <a href="{{ item.url | relative_url }}" class="button small" style="height: 2.1rem; line-height: 2.1rem; padding: 0 1.2rem; font-size: 0.75rem;">Learn More</a>
                        </td>                    
                    </tr>
                    {% endfor %}
                </tbody>
            </table>
        </div>
    </div>
</section>

<style>
    /* This is the line that actually hides the projects */
    .archive-row.hidden {
        display: none !important;
    }

    /* Optional: Style for the active filter button */
    .filter-btn.active {
        background-color: #9bf1ff !important;
        color: #1f1f1f !important;
    }

    .status-container {
        display: flex;
        align-items: center;
        gap: 8px; /* space between dot and text */
    }

    .status-dot {
        width: 8px;
        height: 8px;
        border-radius: 50%;
        display: inline-block;
    }

    .status-text {
        font-size: 0.75rem;
        text-transform: uppercase;
        letter-spacing: 1px;
        opacity: 0.9;
    }

    /* Animation Logic */
    @keyframes status-pulse {
        0% { opacity: 1; transform: scale(1); }
        50% { opacity: 0.3; transform: scale(0.9); }
        100% { opacity: 1; transform: scale(1); }
    }

    /* Color Assignments */
    /* Launched - Green */
    .status-dot.launched-active-development {
        background-color: #9bff9b;
        box-shadow: 0 0 8px #9bff9b;
        animation: status-pulse 1.5s infinite ease-in-out;
    }

    /* Completed - White/Grey */
    .status-dot.completed {
        background-color: #ffffff;
        box-shadow: 0 0 8px #ffffff;
    }

    /* In Progress - Yellow */
    .status-dot.in-progress {
        background-color: #ffe664;
        box-shadow: 0 0 8px #ffe664;
    }

    /* Maintained - Blue */
    .status-dot.launched-maintained {
        background-color: #9bf1ff;
        box-shadow: 0 0 8px #9bf1ff;
        animation: status-pulse 1.5s infinite ease-in-out;
    }
</style>


<script>
document.querySelectorAll('.filter-btn').forEach(button => {
    button.addEventListener('click', () => {
        // Update active button state
        document.querySelectorAll('.filter-btn').forEach(btn => btn.classList.remove('active'));
        button.classList.add('active');

        const filter = button.getAttribute('data-filter');
        const rows = document.querySelectorAll('.archive-row');

        rows.forEach(row => {
            // Check if collection class exists on row
            if (filter === 'all' || row.classList.contains(filter)) {
                row.classList.remove('hidden');
            } else {
                row.classList.add('hidden');
            }
        });
    });
});
</script>