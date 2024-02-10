---
layout: post
math: "true"
toc: "true"
title: Fundamentials of Graph Theory
categories: combinatorics
tags:
  - graph
---
# Definitions

## graph

A graph ${ G }$ is an ordered pair of disjoint sets ${ (V,E) }$ s.t. ${ E \subset V^{(2)} }$ of unordered pairs of V. The set ${ V }$ is a set of *vertices* and ${ E }$ is the set of *edges*.

An edge ${ \{ x,y \} }$ is said to *join* the vertices ${ x }$ and ${ y }$ and is denoted by ${ xy }$.

## subgraph

${ G'=(V',E') }$ is a subgraph of ${ G = (V,E) }$ if ${ V' \subset V }$ and ${ E' \subset E }$. In this case we write ${ G' \subset G}$.

If ${ G' }$ contains all edges of ${ G }$ that joint two vertices in ${ V' }$, then ${ G' }$ is said to be the subgraph *induced* or *spanned by* ${ V' }$ and is denoted by ${ G[V'] }$.

If ${ V'=V }$, then ${ G' }$ is said to be a spanning subgraph of ${ G }$.

## order and size

the order of ${ G := \lvert V(G) \rvert }$, denoted by ${ \lvert G \rvert }$

the size of ${ G:= \lvert E(G) \rvert }$, denoted by ${ e(G) }$

## complement

${ \overline{G} = (V, V^{(2)}-E ) }$

## neighborhood

$${ \Gamma(x) = \left\{ y \in V : y \mbox{ is adjacent to x} \right\} }$$

is called open neighborhood of ${ x }$, and

$${ \Gamma(x) \cup \left\{ x \right\} }$$

is called closed neighborhood of ${ x }$.

# Paths, Cycles, and Trees

A path is a graph ${ P }$ of the form

$$ V(P) = \left\{ x\_{0},x\_{1},\dots,x\_{l} \right\}, \quad  E(P) = \left\{ x\_{0}x\_{1},x\_{1}x\_{2}, \dots, x\_{l-1}x\_{l} \right\} $$

This path ${ P }$ is usually denoted by ${ x\_{0}x\_{1},\cdots x\_{l} }$

A walk ${ W }$ in a  graph is an alternating sequence of vetrices and edges, say ${ x\_{0},e\_{1},x\_{1},e\_{2},\dots,e\_{l},x\_{l} }$ where ${ e\_{i}=x\_{i-1}x\_{i} }$.

This walk ${ W }$ is called a trail if all its edges are disticnt.

A trail whose endvertices coincide (a closed trail) is called a circuit.

If a walk ${ W = x\_{0}x\_{1}\cdots x\_{l} }$ is s.t. ${ l \ge 3, x\_{0}=x\_{l} }$, and vertices ${ x\_{i} }$, ${ 0<i<l }$ are distinct from each other and ${ x\_{0} }$, then ${ W }$ is said to be a cycle.

We frequently use the symbol ${ P\_{l} }$ to denote an arbitrary path of length ${ l }$, and ${ C\_{l} }$ to denote a cycle of length ${ l }$. We call ${ C\_{3} }$ a triangle, ${ C\_{4} }$ a quadrilateral, ${ C\_{5} }$ a pentagon, and so on. A cycle is even(ood) if its length is even(ood).


# References

 1. Béla Bollobás. *Modern Graph Theory*, Graduate Texts in Mathematics, Vol. 184, Springer-Verlag, New York, 1998.