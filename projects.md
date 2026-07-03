---
layout: default
title: Projects
permalink: /projects/
---

# Projects

<div class="project-grid">
  {% for project in site.data.projects %}
  <div class="project-card" onclick="window.open('{{ project.url }}', '_blank')">
    <img src="{{ project.image }}" alt="{{ project.title }} screenshot" class="project-card-image">
    <div class="project-card-body">
      <h2>{{ project.title }}</h2>
      <span class="project-date">{{ project.year }}</span>
      <p>{{ project.description }}</p>
      <div class="project-tags">
        {% for tag in project.tags %}
        <span class="project-tag">{{ tag }}</span>
        {% endfor %}
      </div>
    </div>
  </div>
  {% endfor %}
</div>

<script>
document.querySelectorAll('.project-card-body a').forEach(function(link) {
  link.addEventListener('click', function(e) { e.stopPropagation(); });
});
</script>
