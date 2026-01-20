---
layout: default
title: "Projects"
permalink: /projects/
description: "Academic projects, research papers, and personal work"
---

<div class="container">
  <header class="page-header">
    <h1 class="page-title">Projects</h1>
    <p class="page-description">A collection of academic projects, research papers, and personal work spanning computer science, mathematics, and community involvement.</p>
  </header>

  <div class="grid grid-2">
    {% assign sorted_projects = site.projects | sort: 'date' | reverse %}
    {% for project in sorted_projects %}
      {% include project-card.html project=project %}
    {% endfor %}
  </div>
</div>
