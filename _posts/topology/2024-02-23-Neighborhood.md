---
layout: post
math: "true"
toc: "true"
title: Neighborhood
categories: General-Topology
tags:
  - filter
---
Let ${ (X,\mathcal{T}) }$ be a topological space, and let ${ N \subseteq X }$

## Neighborhood

We say that ${ N}$ is a **neighborhood** of a point ${ x }$ if

$$ x \in U \subseteq N $$

for some open set ${ U }$.

## Neighborhood Filter

For each ${ x \in X }$,

$$ \mathcal{N}(x) = \{ N \in \mathcal{T}: N \mbox{ is a neighborhood of } x \} $$

is a [proper filter](https://paraconsistent.github.io/logic/2024/02/23/Filters-and-Nets.html#filters-and-ideals) on ${ X }$, which we call the **neighborhood filter at ${ x }$** or **filter of neighborhoods of ${ x }$**.

## References

1. Eric Schechter. *Handbook of Analysis and Its foundations*, Academic Press, 110p.