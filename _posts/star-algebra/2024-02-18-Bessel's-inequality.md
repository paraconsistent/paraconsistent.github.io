---
layout: post
math: "true"
toc: "true"
title: Bessel's inequality
categories: Functional-Analysis
tags:
  - Hilbert-space
---
## Statement

Let ${ X }$ be an inner product space. If ${ \left\\{ x_{i} \right\\} }$ be an orthonormal family of vetors of ${ X }$, then

$$ \sum_{i \in I} \lvert \langle x,x_{i} \rangle \rvert^{2} \le \lVert x \rVert^{2} $$

where ${ \lVert x \rVert = \sqrt{\langle x,x \rangle} }$ .

### proof

By Schwartz inequality,

$$ \lvert \langle x,x_{i} \rangle \rvert^{2} \le \lVert x \rVert^{2}\lVert x_{i} \rVert^{2} $$

By orthonormal assumption, ${ \lVert x_{i} \rVert^{2}=1 }$.