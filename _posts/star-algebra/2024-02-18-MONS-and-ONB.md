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