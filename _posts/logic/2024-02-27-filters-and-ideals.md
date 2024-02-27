---
layout: post
math: "true"
toc: "true"
title: Filters and Ideals
categories: Logic
tags:
  - filter
  - order
---
## 집합론적 정의

### Filter

nonempty ${ \mathcal{F} \subseteq \mathcal{P}(X) }$가 다음 두 조건을 만족하면 **filter** on X라고 부른다.

1. ${ S \in \mathcal{F} }$ 이고 ${ S \subseteq T \subseteq X }$이면 ${ T \in \mathcal{F} }$
1. ${ S,T \in \mathcal{F} \Rightarrow S \cap T \in \mathcal{F}}$

이는 위상공간에서 근방(neighborhood)를 모방한 것이다.

${N}$이 ${ x }$의 근방이라는 것은 어떤 열린집합 ${ U }$가 존재해서,

$$ x \in U \subseteq N $$

이라는 것이므로  ${ U }$를 포함하는 모든 집합은 ${ x }$의 근방이다.

또 두 근방 ${ N\_{1}, N\_{2} }$이 있을 때,

$$ x \in U \subseteq N_{1} \cap N_{2}  $$ 
이므로 ${ N_{1} \cap N_{2} }$ 또한 ${ x }$의 근방임을 알 수 있다. 실제로 위상공간 ${ (X,\mathcal{T}) }$와 점 ${ x \in X }$ 주어졌을때,

$$ \mathcal{N}(x)=\{ N \in \mathcal{P}(X): x \in U \subseteq N \mbox{ for some } U \in \mathcal{T}\} $$

는 filter이다.

filter ${ \mathcal{F} }$가 공집합을 포함하면 조건 1에 의해

$$ \mathcal{F} = \mathcal{P}(X)$$

이 된다.

${ \mathcal{F} = \mathcal{P}(X) }$인 filter를 **improper filter**라고 하고 improper가 아닌 경우 **proper filter**라고 한다.

### Ideal

nonempty ${ \mathcal{J} \subseteq \mathcal{P}(X) }$가 다음 조건을 만족하면 **ideal** on X라고 부른다.

1. ${ S \in \mathcal{J} }$이고 ${ S \supseteq T }$이면 ${ T \in \mathcal{J} }$
1. ${ S,T \in \mathcal{J} \Rightarrow S \cup T}$

${ \mathcal{J}=\mathcal{P}(X) }$인 경우 **improper ideal**이라고 하고 improper가 아닌 경우 **proper ideal**이라고 한다.


### Filter ↔ Ideal duality

${ \mathcal{F} }$가 filter on ${ X }$일 때,

$$ \mathcal{J}=\{ X \setminus F: F\in \mathcal{F} \} $$

는 ideal이 되고 이 ${ \mathcal{J} }$를 ${ \mathcal{F} }$의 **dual**이라고 한다.

반대로 ${ \mathcal{J} }$가 ideal on ${ X }$일 때

$$ \mathcal{F}=\{ X \setminus J : J \in \mathcal{J} \} $$

는 filter가 되고 이 ${ \mathcal{F} }$를 ${ \mathcal{J} }$의 **dual**이라고 한다.

## 참고문헌

1. Eric Schechter (1996). *Handbook of Analysis and Its Applications*, Academic Press.