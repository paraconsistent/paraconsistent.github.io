---
layout: post
math: "true"
toc: "true"
title: Quasi-metric
categories: General-Topology
---
Let ${ X \neq \emptyset }$. ${ d: X \times X \to [0,\infty) }$ called quasi-metric on ${ X }$ if
- ${ d(x,y)=0 \mbox{ iff } x=y }$
- ${ d(x,y) \le d(x,z) + d(z,y) }$ for all ${ x,y,z \in X }$

The difference between a metric and quasi-metric is that a quasi-metric does not possess the symmetry axiom:

$$ d(x,y) = d(y,x) $$

|  | identity axiom | symmetry axiom | triangle axiom |
| ---- | ---- | ---- | ---- |
| [metric](https://paraconsistent.github.io/general-topology/2023/02/23/metric.html) | O | O | O |
| [quasi-metric](https://paraconsistent.github.io/general-topology/2024/02/23/Quasi-metric.html) | O | X | O |
| [pseudo-metric](https://paraconsistent.github.io/general-topology/2024/02/23/Pseudo-metric.html) | △ | O | O |

## References

1. Quasi-metric. _Encyclopedia of Mathematics._ URL: http://encyclopediaofmath.org/index.php?title=Quasi-metric&oldid=37708