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


<h4>Model Categories</h4>
I am studying about model categories from Quillen's _Homotopical algebra_ . I am recording down the main ideas in this [note]({{site.url}}/modelcat.pdf){:target="_blank"} for my reference.
<hr>

<h4>
Serre Spectral Sequences
</h4>
A short note elaborating some examples from Hatcher's note on Serre spectral sequences. I have written few examples that help explain the basics of Serre specseq. They touch on the basic convergence and naturality properties.\\
[Serre spec seq]({{ site.url }}/serrespecseq.pdf){:target="_blank"}
<hr>



<h4>
Poincare Duality for Manifolds
</h4>
A [note]({{ site.url }}/pd.pdf){:target="_blank"} on Poincare Duality

<br>

<table style="width:100%"><tr><td><img src="http://math.jhu.edu/~savitt/GTM/maclane.jpg" width=500 height=140 alt=""></td><td><p>If I were a Springer-Verlag Graduate Text in Mathematics, I would be Saunders Mac Lane's <b><i>Categories for the Working Mathematician</i></b>.</p><p>I provide an array of general ideas useful in a wide variety of fields.  Starting from foundations, I illuminate the concepts of category, functor, natural transformation, and duality.  I then turn to adjoint functors, which provide a description of universal constructions, an analysis of the representation of functors by sets of morphisms, and a means of manipulating direct and inverse limits. </p><p>Which Springer GTM would <i>you</i> be? <a href="http://math.jhu.edu/~savitt/GTM.html">The Springer GTM Test</a></p></td></tr></table>