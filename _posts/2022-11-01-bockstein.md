---
layout: post
title:  Steenrod Algebra
date:   2022-11-01
categories: ALGTOP
---
#### Bockstein Homomorphism
I am fixing gaps in my knowledge of basic algebraic topology. This is basically me jotting down the definitions and theorems. 
This post will be focusing on Bockstein homomorphism. 

Consider the short exact sequence $0\to G\to H\to K\to 0$ and apply the functor, $\hom (C_n(X),-)$, we get an exact sequence \\[0\to C_n(X;G)\to C_n(X;H)\to C_n(X;K)\to 0\\] which is exact since $C_n(X)$ is free. We get an associated long exact sequence, 
\\[\cdots\to H^n(X;G)\to H^n(X;H)\to H^n(X;K)\to H^{n+1}(X;G)\to \cdots\\]

The boundary map $H^n(X;K)\to H^{n+1}(X;G)$ is called the Bockstein homomomorphism. 

We are mainly interested in the map $$\beta:H^n(X;\mathbb{Z}_m)\to H^{n+1}(X;\mathbb{Z}_m)$$ associated to the spectral sequence $$0\to \mathbb{Z}_m\xrightarrow{m} \mathbb{Z}_{m^2}\to \mathbb{Z}_m\to 0$$. Most of our focus will also be on $m$ prime.\\
Also look at the Bockstein map $$\tilde{\beta}: H^n(X;\mathbb{Z}_m)\to H^{n+1}(X;\mathbb{Z}_m)$$ associated to the sexseq $$0\to \mathbb{Z}\xrightarrow{m} \mathbb{Z}_{}\to \mathbb{Z}_m\to 0$$. From the natural map of latter sexseq to the former, we get the relation $\beta=\rho \tilde{\beta}$ where $$\rho:H^*(X;\mathbb{Z})\to H^*(X;\mathbb{Z}_m)$$ is the map induced by reducing coefficients mod $m$.

![]({{site.url}}/1img.png){: width="500" }
<!-- <img align="left" width="500" src="{{site.url}}/1img.png"> -->

The Bockstein homomorphisms also satisfy the derivation property: \\[ \beta(a\smile b)=\beta(a)\smile b+(-1)^{\vert a\vert}a\smile \beta(b)\\]

Note that $\beta ^2=0$, so we have a chain complex with groups $$H^n(X;\mathbb{Z}_m)$$ and $\beta$ as boundary homomorphisms. The associated Bockstein cohomology groups are \\[\frac{ker(\beta)}{Im(\beta)}=BH^n(X;\mathbb{Z}_m)\\]

We record a proposition that helps us determine $BH^*$ before we proceed with discussion about Steenrod squares.

_If $$H_n(X;\mathbb{Z})$$ is finitely generatted for all $n$, then the Bockstein Cohomology groups $$BH^n(X;\mathbb{Z}_p)$$ are determined by the  following rules:_ 
<ol>
  <li><em>Each $\mathbb{Z}$ summand of $H^n(X ; \mathbb{Z})$ contributes a $\mathbb{Z}_p$ summand to $B H^n\left(X ; \mathbb{Z}_p\right)$. </em></li>
  <li><em>Each $\mathbb{Z}_{p^k}$ summand of $H^n(X ; \mathbb{Z})$ with $k>1$ contributes $\mathbb{Z}_p$ summands to both $B H^{n-1}\left(X ; \mathbb{Z}_p\right)$ and $B H^n\left(X ; \mathbb{Z}_p\right)$.</em></li>
  <li><em>$A \mathbb{Z}_p$ summand of $H^n(X ; \mathbb{Z})$ gives $\mathbb{Z}_p$ summands of $H^{n-1}\left(X ; \mathbb{Z}_p\right)$ and $H^n\left(X ; \mathbb{Z}_p\right)$ with $\beta$ an isomorphism between these two summands, hence there is no contribution to $B H^*\left(X ; \mathbb{Z}_p\right)$.</em></li>
</ol>

#### Steenrod Squares
A cohomology operation is a transformation $\Theta :H^m(X;G)\to H^n(X;H)$ defined for alls apces $X$, with a fixed choice of $m,n, G, H$ and satisfyuing the naturality property that for all maps $f:X\to Y$ there is a commuting diagram: 

  $$\begin{CD}
 H^m(Y;G)@>{\Theta_Y}>>H^n(Y;H)\\
@VV{f^*}V @VVV \\
H^m(X;G) @>{\Theta_X}>> H^n(X;H)
\end{CD}$$


<em> For fixed $m,n,G, H$ there is a bijection between the set of all cohomlogy operations $\Theta: H^m(X;G)\to H^n(X;H)$ and $H^n(K(G,m);H)$, ,defined by $\Theta\mapsto \Theta(\iota)$ where $\iota \in H^m(K(G,m);G)$ is a fundamental class.</em>

_will be continued_







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
