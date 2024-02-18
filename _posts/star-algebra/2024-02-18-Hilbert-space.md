---
layout: post
math: "true"
toc: "true"
title: Hilbert space
categories: Functional-Analysis
tags:
  - Hilbert-space
---
## Pre-Hilbert space

A vector space ${ X }$ over the field ${ F=\mathbb{R}, \mathbb{C} }$ equipped with

$$ (\cdot,\cdot) : X \times X \to F $$

satisfying the following conditions:

- ${ (x+y,z) = (x,z) + (y,z), \quad (\lambda x,y) = \lambda(x,y) }$  for all ${ \lambda \in F, x,y,z \in X }$

-  ${ (y,x) = \overline{(x,y)} }$ for all ${ x,y \in X }$

- ${ (x,x) > 0 }$ for all nonzero ${ x \in X }$

**Remark** ${ (x,x) = 0 \mbox{ iff } x=0 }$

## Hilbert space

Hilbert space is a complete inner product space, i.e., the norm ${ \lVert x \rVert := \sqrt{(x,x)} }$ induces a metric

$$ d(x,y) = \lVert x-y \rVert $$

Then we say ${ X }$ is Hilbert space if complete with ${ d }$.