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
라고 할 수 있다.

모든 ${ x_{0} \in X}$에 대해 위 조건을 만족하면, **${ f }$가 upper semicontinuous**라고 한다.

### Lower semicontinuity

$$ f(x_{0}) \le \liminf_{x \to x_{0}} f(x) $$

일 때, ${ f }$가 ${ x_{0} }$에서 **lower semicontinuous**라고 한다.

동등하게, 모든 ${ y<f(x_{0}) }$에 대해

$$ f^{-1}((y,+\infty]) \mbox{ is open in } X $$

라고 할 수 있다.

모든 ${ x_{0} \in X }$에 대해 위 조건을 만족하면, **${ f }$가 lower semicontinuous**라고 한다.

## 기하학적 관점

${ f: X\setminus \\{ x_{0} \\} \to [-\infty,+\infty] }$의 그래프가 다음과 같이 주어졌다고 하자.

![semicontinuity](https://github.com/paraconsistent/paraconsistent.github.io/blob/master/_posts/analysis/semicontinuity/semiconti.png?raw=true)

이때,

$$ \begin{eqnarray} \liminf_{x \to x_{0}} f(x) = a \\ \limsup_{x \to x_{0}} f(x) = b \end{eqnarray} $$

이기 때문에 만약 ${ (x\_{0},f(x\_{0})) }$라는 점을 추가했을 때

${ f(x_{0}) \ge b }$인 경우, upper semicontinuous

${ f(x_{0}) \le a }$인 경우, lower semicontinuous

가 된다.[^1]

## 같이보기

- [Directional limit and continuity](https://paraconsistent.github.io/analysis/2024/02/27/directional-continuity.html)

---
[^1]: 이 경우에 등호가 조건인 one-sided continuity와 헷갈리면 안된다.