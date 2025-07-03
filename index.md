---
layout: default
title: Home
---

Welcome to my RL blog!

Here's an example LaTeX equation:

$$
\eta^{\hat{M}}(\pi) = \mathbb{E}_{(s, a) \sim \rho_{\pi}^{\hat{T}}} [G_{\pi}^{\hat{M}}(s, a)]
$$


<script>
  MathJax = {
    tex: {
      inlineMath: [['$', '$'], ['\\(', '\\)']],
      displayMath: [['$$', '$$'], ['\\[', '\\]']],
      processEscapes: true
    },
    options: {
      skipHtmlTags: ['script', 'noscript', 'style', 'textarea', 'pre'],
      ignoreHtmlClass: 'tex2jax_ignore',
      processHtmlClass: 'mathjax_process'
    }
  };
</script>
