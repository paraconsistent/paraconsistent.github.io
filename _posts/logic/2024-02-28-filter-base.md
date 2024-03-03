---
layout: post
math: "true"
toc: "true"
title: Filter base and prefilter
categories: Logic
tags:
  - filter
---
## 정의

### Filter base

poset ${ P }$ 위의 [filter](https://paraconsistent.github.io/logic/2024/02/27/filters-and-ideals.html#filter) ${ F }$가 주어졌을 때 ${ B \subseteq F }$가 **filter base**라는 것은 ${ B }$로 생성되는 [upper set](https://paraconsistent.github.io/logic/2024/02/28/upper-set.html)이 ${ F }$인 경우를 의미한다.

$$ B^{\uparrow P} = \bigcup_{b \in B} \{ x \in P: b\le x \} =F $$

즉, ${ B }$라는 집합을 **upward closure** 시키면 ${ F }$가 된다는 것이다.

거꾸로, ${ B }$가 ${ F }$를 생성하려면 반드시 다음 조건을 만족해야 된다.

$$ \forall x \in F,\exists b \in B, \quad b \le x $$

### Prefilter

위의 filter base ${ B }$가 nonempty이고 downward directed이면 upper closure ${ B^{\uparrow P} }$가 항상 어떤 filter를 생성한다. 이런 ${ B }$를 prefilter라고 한다.

### Filter subbase

집합 ${ X }$에 대해 ${ \mathcal{S} \subseteq \mathcal{P}(X) }$가 주어졌을때 ${ \mathcal{S} }$를 포함하는 가장 작은 filter ${ \mathcal{F} }$를 생각해보자.

[집합론적 filter](https://paraconsistent.github.io/logic/2024/02/27/filter.html#%EC%A7%91%ED%95%A9%EB%A1%A0%EC%A0%81-%EC%A0%95%EC%9D%98)는 downward directedness와 finite intersection property가 동일하다. 따라서,

$$ \mathcal{B}= \mathcal{S} \cup \{ \mbox{all finite intersections in } \mathcal{S} \} $$

는 prefilter가 된다. 이 ${ \mathcal{B} }$가 filter ${ \mathcal{F} }$를 생성할 때, ${ \mathcal{S} }$를 ${ \mathcal{F} }$의 **subbase**라고 한다.


## 참고문헌

1. Eric Schechter (1996). *Handbook of Analysis and Its Foundations*, Academic Press.
1. Wikipeda. *Filter (mathematics)*, Retrieved: Feb 28, 2024, URL:https://en.wikipedia.org/wiki/Filter_(mathematics).