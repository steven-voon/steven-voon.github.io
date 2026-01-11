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
            <button class="filter-btn" data-filter="projects">Strategic Pillars</button>
            <button class="filter-btn" data-filter="lab">R&D Lab</button>
        </div>
        <div class="table-wrapper">
            <table class="alt archive-table">
                <thead>
                    <tr>
                        <th>Year</th>
                        <th>Project Name</th>
                        <th>Category</th>
                        <th>Action</th>
                    </tr>
                </thead>
                <tbody>
                    {% for item in all_items %}
                    <tr>
                        <td style="color: #9bf1ff; font-weight: 600;">{{ item.date | date: "%Y" }}</td>
                        <td><strong>{{ item.title }}</strong></td>
                        <td style="text-transform: uppercase; font-size: 0.7rem; letter-spacing: 1px;">
                            {{ item.collection }}
                        </td>
                        <td><a href="{{ item.url | relative_url }}" class="button small">View Specs</a></td>
                    </tr>
                    {% endfor %}
                </tbody>
            </table>
        </div>
    </div>
</section>


<script>
document.querySelectorAll('.filter-btn').forEach(button => {
    button.addEventListener('click', () => {
        // Update active button state
        document.querySelectorAll('.filter-btn').forEach(btn => btn.classList.remove('active'));
        button.classList.add('active');

        const filter = button.getAttribute('data-filter');
        const rows = document.querySelectorAll('.archive-row');

        rows.forEach(row => {
            if (filter === 'all' || row.classList.contains(filter)) {
                row.classList.remove('hidden');
            } else {
                row.classList.add('hidden');
            }
        });
    });
});
</script>