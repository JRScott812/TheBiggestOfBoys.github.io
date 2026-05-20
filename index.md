---
layout: default
title: Home
permalink: /
---

<h1>My Amazing Website</h1>

<section class="about">
  <h1>About Me:</h1>
  <h2>
    I'm a student interested in software development and technology in general.
    During an internship I had over the summer, I worked with <a href="https://clovernook.org/">Clovernook Center
    for the Blind & Visually Impaired</a> in developing an AR (Augmented Reality) navigation app for the
    Microsoft HoloLens. That was a great opportunity to learn new programming skills and tools, like Unity.
    It was great to see technology have such a direct impact on improving peoples' lives.
  </h2>
</section>

<section class="latest-projects">
  <h2>Projects (placeholders)</h2>
  <ul>
    {% for project in site.projects %}
      <li>
        <a href="{{ project.url | relative_url }}">{{ project.title }}</a>
        {% if project.excerpt %} — {{ project.excerpt }}{% endif %}
        {% if project.published == false %} <em>(placeholder)</em>{% endif %}
      </li>
    {% endfor %}
  </ul>
</section>
