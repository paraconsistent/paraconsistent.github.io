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

주어진 nonempty [preordered set](https://paraconsistent.github.io/logic/2024/02/15/preorder.html) ${ \left( J, \prec \right) }$이 주어졌을때, 조건

>모든 ${ \alpha,\beta \in J }$에 대해 어떤 ${ \gamma }$가 존재하여 ${ \alpha \prec \gamma }$이고 ${ \beta \prec \gamma }$

를 만족시키면 ${ (J,\prec) }$를 directed set이라고 부른다.

## 모티브

즉, ${ \alpha }$와 ${ \beta }$의 공통 상계 ${ \gamma }$가 항상 존재하는 것이다. 이 ${ \gamma }$는 ${ \alpha }$와 ${ \beta }$가 비교 불가능일때도 ${ \max(\alpha,\beta) }$와 유사한 역할을 한다 생각하면 된다.

## 함께보기

- [net](https://paraconsistent.github.io/logic/2024/02/26/net.html)