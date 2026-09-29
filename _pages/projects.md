---
layout: page
title: projects
permalink: /projects/
description: Open-source systems work on efficient inference for diffusion language models.
nav: true
nav_order: 4
---

<div class="projects">
  {% if site.projects and site.projects.size > 0 %}
    {% assign sorted_projects = site.projects | sort: "importance" %}
    <div class="row row-cols-1 row-cols-md-3">
      {% for project in sorted_projects %}
        {% include projects.liquid %}
      {% endfor %}
    </div>
  {% else %}
    <p>No projects to show yet.</p>
  {% endif %}
</div>
