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
  <hr>
{% endfor %}

A [note]({{ site.url }}/pd.pdf) on Poincare Duality

<hr>

<!-- there was <h4>....</h4> and project url was inside it indented and <p>...</p> contained project description-->