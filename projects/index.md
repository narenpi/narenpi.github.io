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

<h4>
Poincare Duality for Manifolds
</h4>
A [note]({{ site.url }}/pd.pdf) on Poincare Duality

<hr>

<h4>
Serre Spectral Sequences
</h4>
A short note elaborating some examples from Hatcher's note on Serre spectral sequences. I have written few examples that help explain the basics of Serre specseq. They touch on the basic convergence and naturality properties.\\
[Serre spec seq]({{ site.url }}/serrespecseq.pdf)
<!-- there was <h4>....</h4> and project url was inside it indented and <p>...</p> contained project description-->