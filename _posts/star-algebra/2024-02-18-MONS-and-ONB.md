---
layout: post
math: "true"
toc: "true"
title: MONS and ONB
categories: Functional-Analysis
tags:
  - Hilbert-space
---
## Definitions

Given inner product space ${ (X,\langle \cdot,\cdot \rangle) }$,

**orthonormal system** is a subset ${S  }$ of ${ X }$ s.t.
- (orthogonality) ${ \langle x,y \rangle = 0 }$ for all distinct ${ x,y \in S }$
- (normality) ${ \langle x,x \rangle =1 }$ for all ${ x \in S }$

**maximal orthonormal system** (ONB) is a orthonormal system of maximal with inclusion ${ \subseteq }$

**orthonormal basis** (ONB) is a orthonormal system s.t.

$$ x = \sum_{y \in S} c_{y} y$$

for some sequence ${ \left\{ c_{y} \right\} }$ of scalars of ${ X }$.

## Gram-Schmidt orthogonalization process

Let
$$ \left \\{ u_{1}, u_{2}, u_{3} \dots \right \\} $$

be at most countable linearly independent susbset of inner product space ${ X }$. Define

$$ \begin{align} w_{1} &= u_{1} \\ w_{n+1} &= u_{n+1}-\sum_{j=1}^{n} \left( u_{n+1}, \frac{w_{j}}{\lVert w_{j} \rVert} \right) \frac{w_{j}}{\lVert w_{j} \rVert} \end{align} $$

and define

$$ v_{j}:= \frac{w_{j}}{\lVert w_{j} \rVert} $$

, then the set ${ \left\{ v_{j} \right\} }$ is orthornomal system such that

$$ \left\{ v_{j} \right\}_{j=1}^{n} \mbox{ spans the same subspace as } \left\{ u_{j} \right\}_{j=1}^{n}  $$

for all ${ n \in \mathbb{N} }$.