---
layout: post
math: "true"
toc: "true"
title: Semicontinuity
categories: Analysis
---
## 정의

주어진 topological space ${ X }$에 대해 함수 ${ f: X \to [-\infty, + \infty] }$를 생각해보자. 

### Upper semicontinuity

$$ \limsup_{x \to x_{0}} f(x) \le f(x_{0}) $$

일 때, ${ f }$가 ${ x_{0} }$에서 **upper semicontinuous**라고 한다.

동등하게, ${ y>f(x_{0}) }$에 대해

$$ f^{-1}([-\infty,y)) \mbox{ is open in } X  $$

모든 ${ x_{0} \in X}$에 대해 위 조건을 만족하면, **${ f }$가 upper semicontinuous**라고 한다.

### Lower semicontinuity

$$ f(x_{0}) \le \liminf_{x \to x_{0}} f(x) $$

일 때, ${ f }$가 ${ x_{0} }$에서 **lower semicontinuous**라고 한다.

동등하게, 모든 ${ y<f(x_{0}) }$에 대해

$$ f^{-1}((y,+\infty]) \mbox{ is open in } X $$

모든 ${ x_{0} \in X }$에 대해 위 조건을 만족하면, **${ f }$가 lower semicontinuous**라고 한다.

## 도식

