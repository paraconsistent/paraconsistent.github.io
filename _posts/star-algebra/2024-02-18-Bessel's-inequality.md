---
layout: post
math: "true"
toc: "true"
title: Bessel's inequality
categories: Functional-Analysis
tags:
  - hilbert-space
---
## Statement

Let ${ X }$ be an inner product space. If ${ \{ x\_{i} \}_{i \in I} }$ be an orthonormal family of vetors of ${ X }$, then

$$ \sum_{i \in I} \lvert \langle x,x_{i} \rangle \rvert^{2} \le \lVert x \rVert^{2} $$

where ${ \lVert x \rVert = \sqrt{\langle x,x \rangle} }$ .

### proof

For any finite subset ${ F }$ of ${ I }$, define

$$ x_{F} = \sum_{i \in F} \langle x,x_{i} \rangle x_{i} $$

Then,

$$ \begin{eqnarray} 0 \le \lVert x-x_{F} \rVert^{2} &=& \lVert x \rVert^{2}- \langle x,x_{F} \rangle - \langle x_{F},x \rangle + \lVert x_{F} \rVert^{2} \\ &=& \lVert x \rVert^{2} -\sum_{i \in F}\lvert\langle x,x_{i} \rangle\rvert^{2} \end{eqnarray}$$

Therefore,

$$\begin{eqnarray} \sum_{i \in I} \lvert \langle x,x_{i} \rangle \rvert^{2} &=& \sup \left\{ \sum_{i \in F} \lvert\langle x,x_{i} \rangle \rvert^{2} : F \mbox{ is a finite subset of } I \right\} \\ &\le& \lVert x \rVert^{2} \end{eqnarray}$$
