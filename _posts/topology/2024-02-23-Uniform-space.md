---
layout: post
math: "true"
toc: "true"
title: Unifor space
categories: General-Topology
---
## filter definition

A filter ${ \mathfrak{U} \subset X \times X }$ is called *uniform structure* (*a uniformity*) if
- ${ (\forall V \in \mathfrak{U})\  V \supseteq \Delta }$
- ${ (\forall V \in \mathfrak{U}) \  V^{-1} \in \mathfrak{U}}$
- ${ (\forall V \in \mathfrak{U}, \exists W \in \mathfrak{U}  ) \ W\circ W \subseteq V }$

where
- ${ \Delta = \{ (x,x) : x \in X \} }$
- ${ V^{-1} = \{ (y,x) : (x,y) \in V \} }$
- ${ W \circ W = \{ (x,y) : (\exists z \in X)\  (x,z), (z,y) \in W \} }$

The elements of ${ \mathfrak{U} }$ are called *entourages* of the uniformity defined by ${ \mathfrak{U} }$.

## convering definition

A uniformity on a set ${ X }$ defined by the specification of a system of coverings ${ \mathfrak{C} }$ on ${ X }$ satisfying the following axioms:

- ${ \forall \alpha \in \mathfrak{C}}$, ${ \alpha }$ refines covering ${ \beta \Rightarrow \beta \in \mathfrak{C}}$
- ${ \forall \alpha_{1},\alpha_{2} \in \mathfrak{C} }$, ${ \exists \beta \in \mathfrak{C}}$ that star-refines both ${ \alpha_{1} }$ and ${ \alpha_{2} }$


## References

1. Uniform space. Encyclopedia of Mathematics. URL: http://encyclopediaofmath.org/index.php?title=Uniform_space&oldid=33601
