---
layout: page
title: Math 
permalink: /math/
---

{% for project in site.projects %}
  <h4>
    <a href="{{ project.url }}">
      {{ project.title }}
      </a>
  </h4>
  <p>{{ project.description }}</p>
{% endfor %}