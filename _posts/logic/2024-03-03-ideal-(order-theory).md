---
layout: post
math: "true"
toc: "true"
title: Ideal (order)
categories: Logic
tags:
  - order
  - lattice
  - filter
---
## 정의

주어진 lattice ${ (L, \wedge, \vee) }$에 대해, 그 sublattice ${ (I,\wedge,\vee) }$가 다음 성질을 만족하면 ${ I }$는 ${ L }$의 **ideal**이라고 한다.

$$ a \in L \mbox{ and }  x \in I \Rightarrow a \wedge x \in I $$

meet ${ \wedge }$를 곱으로 봤을때 ${ }$대수학에서 ideal와 같다는 것을 알 수 있다.

## filter

**filter (또는 dual ideal)**은 ideal을 다음과 같이 dualize한 것이다.

$$ a \in L \mbox{ and } x \in F \Rightarrow a \vee x \in F $$

## 참고문헌

1. Grätzer (2011). *Lattice Theory: Foundation*, Birkhäuser.