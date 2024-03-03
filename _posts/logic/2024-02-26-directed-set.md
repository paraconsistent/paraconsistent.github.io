---
layout: post
math: "true"
toc: "true"
title: Directed set
categories: Logic
tags:
  - order
---
## 정의

주어진 nonempty [preordered set](https://paraconsistent.github.io/logic/2024/02/15/preorder.html) ${ \left( J, \preceq \right) }$이 주어졌을때, 조건

$$ \begin{gather} \mbox{(downward directedness)} & \forall x,y \in J, \exists z \in J, \quad z \preceq x \mbox{ and } z \preceq y \end{gather} $$

를 만족시키면 ${ (J,\preceq) }$를 **(downward) directed set**이라고 부른다.

[dual](https://paraconsistent.github.io/logic/2024/03/03/duality-(order-theory).html) 개념으로 **upward directed set**을 다음과 같이 정의한다.

$$ \begin{gather} \mbox{(upward directedness)} & \forall x,y \in J,\exists z \in J, \quad x \preceq z \mbox{ and } y \preceq z  \end{gather}$$

## 모티브

즉, ${ \alpha }$와 ${ \beta }$의 공통 상계 ${ \gamma }$가 항상 존재하는 것이다. 이 ${ \gamma }$는 ${ \alpha }$와 ${ \beta }$가 비교 불가능일때도 ${ \max(\alpha,\beta) }$와 유사한 역할을 한다 생각하면 된다.

## 함께보기

- [Net](https://paraconsistent.github.io/logic/2024/02/26/net.html): directed set에서 나가는 함수 = net
- [Filter](https://paraconsistent.github.io/logic/2024/02/27/filter.html) = downward directed + upper set
- [Ideal (order theory)](https://paraconsistent.github.io/logic/2024/03/03/ideal-(order-theory).html) = upward directed + lower set
