---
layout: post
title:  Bockstein Homomorphism
date:   2022-11-01
categories: ALGTOP
---

I am fixing gaps in my knowledge of basic algebraic topology. This is basically me jotting down the definitions and theorems. 
This post will be focusing on Bockstein homomorphism. 

Consider the short exact sequence $0\to G\to H\to K\to 0$ and apply the functor, $\hom (C_n(X),-)$, we get an exact sequence \\[0\to C_n(X;G)\to C_n(X;H)\to C_n(X;K)\to 0\\] which is exact since $C_n(X)$ is free. We get an associated long exact sequence, 
\\[\cdots\to H^n(X;G)\to H^n(X;H)\to H^n(X;K)\to H^{n+1}(X;G)\to \cdots\\]

The boundary map $H^n(X;K)\to H^{n+1}(X;G)$ is called the Bockstein homomomorphism. 

We are mainly interested in the map $$\beta:H^n(X;\mathbb{Z}_m)\to H^{n+1}(X;\mathbb{Z}_m)$$ associated to the spectral sequence $$0\to \mathbb{Z}_m\xrightarrow{m} \mathbb{Z}_{m^2}\to \mathbb{Z}_m\to 0$$. Most of our focus will also be on $m$ prime.\\
Also look at the Bockstein map $$\tilde{\beta}: H^n(X;\mathbb{Z}_m)\to H^{n+1}(X;\mathbb{Z}_m)$$ associated to the sexseq $$0\to \mathbb{Z}\xrightarrow{m} \mathbb{Z}_{}\to \mathbb{Z}_m\to 0$$. From the natural map of latter sexseq to the former, we get the relation $\beta=\rho \tilde{\beta}$ where $$\rho:H^*(X;\mathbb{Z})\to H^*(X;\mathbb{Z}_m)$$ is the map induced by reducing coefficients mod $m$.
![text]({{site.url}}/1img.png){: width="500" }


 <script type="text/javascript"
  src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.0/MathJax.js?config=TeX-AMS_CHTML">
</script>
<script type="text/x-mathjax-config">
  MathJax.Hub.Config({
    tex2jax: {
      inlineMath: [['$','$'], ['\\(','\\)']],
      processEscapes: true},
      jax: ["input/TeX","input/MathML","input/AsciiMath","output/CommonHTML"],
      extensions: ["tex2jax.js","mml2jax.js","asciimath2jax.js","MathMenu.js","MathZoom.js","AssistiveMML.js", "[Contrib]/a11y/accessibility-menu.js"],
      TeX: {
      extensions: ["AMSmath.js","AMSsymbols.js","noErrors.js","noUndefined.js", "AMScd.js"],
      equationNumbers: {
      autoNumber: "AMS"
      }
    }
  });
</script>
