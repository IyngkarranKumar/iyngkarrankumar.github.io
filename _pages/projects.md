---
permalink: /Projects/
title: "Projects"
---
<style>
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 1.5em;
  padding: 0;
  list-style: none;
}
.project-card {
  border: 1px solid 
#e0e0e0;
  border-radius: 8px;
  padding: 1.5em;
  transition: box-shadow 0.3s ease;
}
.project-card:hover {
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}
.project-card a {
  font-size: 1.1em;
  font-weight: 500;
  text-decoration: none;
  color: 
#3383e2;
}
.project-card p {
  margin: 0.5em 0 0 0;
  font-size: 0.9em;
  color: #666;
}
</style>
<ul class="projects-grid">
  {% assign sorted_projects = site.projects | sort: 'order' %}
  {% for project in sorted_projects %}
    {% if project.show_in_list != false %}
      <li class="project-card">
        <a href="{{ project.url }}">{{ project.title }}</a>
        {% if project.excerpt %}
          <p>{{ project.excerpt | strip_html | truncate: 120 }}</p>
        {% endif %}
      </li>
    {% endif %}
  {% endfor %}
</ul>