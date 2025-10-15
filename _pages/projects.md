---
permalink: /Projects/
title: "Projects"
---

<div class="projects-list">
  <ul style="list-style: none; padding-left: 0;">
    {% assign sorted_projects = site.projects | sort: 'order' %}
    {% for project in sorted_projects %}
      <li style="margin-bottom: 1.5em;"> <!-- Increased spacing here -->
        <a href="{{ project.url }}" style="font-size: 1.1em; font-weight: 500; text-decoration: none; color: #3383e2;">
          {{ project.title }}
        </a>
        {% if project.excerpt %}
          <p style="margin: 0.3em 0 0 0; font-size: 0.9em; color: #888;">
            {{ project.excerpt | strip_html | truncate: 150 }}
          </p>
        {% endif %}
      </li>
    {% endfor %}
  </ul>
</div>