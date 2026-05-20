---
layout: default
title: Projects
permalink: /projects/
---

<h1>Projects</h1>

{% assign published_projects = site.projects | where: "published", true %}

{% if published_projects.size > 0 %}
  <ul>
  {% for project in published_projects %}
    <li>
      <a href="{{ project.url | relative_url }}">{{ project.title }}</a> — {{ project.excerpt }}
    </li>
  {% endfor %}
  </ul>
{% else %}
  <p>No published projects yet. Here are placeholders:</p>
  <ul>
  {% for project in site.projects %}
    <li>
      <a href="{{ project.url | relative_url }}">{{ project.title }}</a> {% if project.published == false %}<em>(placeholder)</em>{% endif %}
    </li>
  {% endfor %}
  </ul>
{% endif %}
