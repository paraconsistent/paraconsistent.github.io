---
layout: post
math: "true"
toc: "true"
title: Alexandrov extension
categories: General-Topology
tags:
  - compact
  - extension
---
## 모티브

주어진 위상공간 ${ X  }$에 가상의 점 ${ \infty }$를 추가하여 ${ X^{\ast}=X \cup \\{ \infty \\} }$라는 더 큰 공간으로 키워서 compactification한다고 생각해보자. 그렇다면 embedding ${ c: X \to X^{\ast} }$ 다음 조건을 만족해야 한다.

1. ${ X }$의 모든 compact set ${ K }$에 대해, ${ c(K) }$가 ${ X^{\ast} }$에서 compact.
1. ${ X }$의 모든 closed subset ${ C }$에 대해, ${ c(C) }$가 ${ X^{\ast} }$에서 compact.

그렇다면 모든 compact 집합이 closed인 다음과 같은 위상을 주면 ${ X^{\ast} }$는 자연스럽게 compact space가 된다.

${ C }$가 ${ X^{\ast} }$에서 closed iff
1. closed이고 compact인 ${ K \subseteq X }$에 대해 ${ C=K \cup \\{ \infty \\}  }$ 또는
1. ${ C }$는 ${ X }$의 closed subset.

## Alexandrov extension

위에서 정의는 다음과 동등하다.

${ V }$가 ${ X^{\ast} }$에서 open iff
1. ${ V }$가 ${ X }$에서 open, 또는
1. closed이고 compact인 ${ K \subseteq X}$에 대해, ${ V = (X\setminus K) \cup \\{ \infty \\} }$

이때 ${ X^{\ast} }$를 ${ X }$의 **Alexandrov extension**이라고 한다.

## The one-point compactification

만약 Alexandrov extension ${ X^{\ast} }$에 Hausdorff 조건을 추가한다면,
1. ${ X }$는 ${ X^{\ast} }$의 subspace로써 Hausdorff space.
1. 위에 의해 ${ X }$의 모든 compact set은 closed.
1. 따라서 임의의 ${ x \in X }$와 그 점의 open neighborhood ${ U }$에 대해서 ${ c^{-1}(\overline{U}) }$는 ${ X }$에서 closed이므로 compact.

결론적으로,

$$ x \in U \subseteq c^{-1}(\overline{U})$$

이므로 ${ X }$는 locally compact.

반대로, ${ X }$가 locally compact Hausdorff라고 하자. ${ X^{\ast} }$가 Hausdorff임을 보이려고 하면 모든 ${ x \neq \infty }$에 대해 다음을 보이면 충분하다.

$$ \exists x \in U, \exists \infty \in V,\quad U \cap V = \emptyset $$

${ X }$가 locally compact space이므로 compact neighborhood ${ K }$가 존재하여, ${ x }$의 적당한 open neighborhood ${ U }$를 포함한다. 즉,

$$ x \in U \subseteq K $$

그런데 ${ \overline{U} }$가 closed이므로 ${ \overline{U} \cap K }$는 ${ K }$의 compact set이다. 그런데, ${ X }$가 Hausdorff이므로 ${ K }$에서 ${ X }$의 closed이므로, ${ K }$에서 ${ \overline{U} }$의 open covering은 모두 ${ X }$에서의 open covering이다.

따라서 ${ \overline{U} }$는 ${ X }$에서 closed이자 compact. 따라서 ${V:= X \setminus \overline{U} }$는 ${ \infty }$의 open neighborhood이고 ${ U \cap V = \emptyset }$. 따라서 ${ X^{\ast} }$는 Haudorff.

결론: ${ X }$가 locally compact Hausdorff ${ \Leftrightarrow X^{\ast} }$가 compact Hausdorff.

Alexandrov extension 중 Hausdorff인 것을 **one-point compactification**이라고 한다.

## 참고문헌

1. Munkres (1999). *Topology*, 2nd edition.
1. *Alexandrov extension*. In Wikipedia. Retrieved March 2, 2024, from [https://en.wikipedia.org/wiki/Alexandroff_extension](https://en.wikipedia.org/wiki/Alexandroff_extension)