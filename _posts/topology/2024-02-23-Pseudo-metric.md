---
layout: post
math: "true"
toc: "true"
title: Pseudo-metric
categories: General-Topology
tags:
  - uniform
---
${ d: X \times X \to [0, \infty)}$ called pseudo-metric if
- ${ d(x,x) = 0}$ for all ${ x \in X }$
- ${ d(x,y) = d(y,x) }$ for all ${ x,y \in X }$
- ${ d(x,y) \le d(x,z) + d(z,y) }$ for all ${ x,y,z \in X }$

The difference between a metric and Pseudo-metric is the identity axiom:
$$ d(x,y) =0 \Rightarrow x =y $$

|  | identity axiom | symmetry axiom | triangle axiom |
| ---- | ---- | ---- | ---- |
| [metric](https://paraconsistent.github.io/general-topology/2023/02/23/metric.html) | O | O | O |
| [quasi-metric](https://paraconsistent.github.io/general-topology/2024/02/23/Quasi-metric.html) | O | X | O |
| [pseudo-metric](https://paraconsistent.github.io/general-topology/2024/02/23/Pseudo-metric.html) | △ | O | O |

## References

1. Pseudo-metric. Encyclopedia of Mathematics. URL: http://encyclopediaofmath.org/index.php?title=Pseudo-metric&oldid=54578
