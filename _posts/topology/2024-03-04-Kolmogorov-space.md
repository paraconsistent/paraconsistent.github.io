---
layout: post
math: "true"
toc: "true"
title: Kolmogorov space
categories: General-Topology
tags:
  - topology
---
## 정의

### topologically indistinguishable

topological space ${ (X,\mathcal{T}) }$의 두 점 ${ x,y }$가 **topologically indistinguishable**이라는 것은

$$ \forall U \in \mathcal{T}, \quad x \in U \iff y \in U $$

이다.

**Proposition** TFAE

1. ${ x }$와 ${ y }$는 topologically indistinguishable
1. ${ \mathrm{cl}(\\{x\\}) = \mathrm{cl}(\\{ y \\})}$ 
1. ${ \mathcal{N}(x) = \mathcal{N}(y) }$

### ${ T_{0} }$ space

다음 조건을 만족하는 topological space ${ (X,\mathcal{T}) }$를 **${ T_{0} }$ space** 또는 **Komogorov space**라고 한다.

 ${ x }$와 ${ y }$가 topologically indistinguishable ${ \Rightarrow }$ ${ x=y }$

동등하게, ${ \forall x,y \in X }$에 대해서 ${ x \neq y }$이면,

$$ \exists U \in \mathcal{T}, \quad x \in U \not\ni y \mbox{ or } x \notin U \ni y $$

## 참고문헌

1. Eric Schechter (1996). *Handbook of Analysis and Its Foundations*, p.436-437