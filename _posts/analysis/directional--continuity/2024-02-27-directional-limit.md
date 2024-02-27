---
layout: post
math: "true"
toc: "true"
title: Directional limit and continuity
categories: Analysis
---
## 정의

${ I }$이 ${ \mathbb{R} }$의 interval이라고 하자.

### Right-hand limit

함수 ${ f: I \to [-\infty,+\infty]  }$에 대해,

$$ \forall \varepsilon>0, \exists \delta >0, \quad a<x<a+\delta \Rightarrow \lvert f(x)-L \rvert  < \varepsilon $$

를 만족시키는 ${ L\in [-\infty,+\infty] }$을 ${ f }$의 **우극한(right-hand limit)**이라 하고 다음과 같이 표기한다.

$$ f(a+)=\lim_{x \to a+} f(x)=\lim_{x \searrow a} f(x) = \lim_{x \downarrow a} f(x)$$

### Left-hand limit

함수 ${ f: I \to [-\infty,+\infty] }$에 대해,

$$ \forall \varepsilon>0,\exists \delta>0, \quad a-\delta<x <a \Rightarrow \lvert f(x)-L \rvert < \varepsilon $$

를 만족시키는 ${ L \in [-\infty,+\infty]}$을 ${ f }$의 **좌극한(left-hand limit)**이라 하고 다음과 같이 표기한다.

$$ f(a-)=\lim_{x\to a-}f(x)= \lim_{x\nearrow a} f(x) = \lim_{x \uparrow a} f(x) $$

### directional continuity

$$ f(a+) = f(a) $$

이면 **${ f }$는 ${ a }$에서 right continuous**라고 하고, 만약 모든 ${ a\in I  }$에서 right continuous이면 ${ f }$는 (${ I }$에서) right continuous라고 한다.

$$ f(a-) = f(a) $$

이면  **${ f }$는 ${ a }$에서 left continuous**라고 하고, 만약 모든 ${ a \in I }$에서 left continuous이면 ${ f }$는 (${ I }$에서) left continuous라고 한다.

left continuous이면서 동시에 right continuous이면 continuous이다.

### 기하학적 관점

${ f: I\setminus \\{ x_{0} \\} \to \mathbb{R} }$의 그래프가 다음과 같이 주어져 있을 때,

![discontinuous](https://github.com/paraconsistent/paraconsistent.github.io/blob/master/_posts/analysis/semicontinuity/semiconti.png?raw=true)

$$ \begin{eqnarray} \lim_{x \searrow x_{0}} f(x) = b \\ \lim_{x \nearrow x_{0}} f(x) = a \end{eqnarray} $$

이므로 점 ${ (x\_{0},f(x\_{0}) )}$를 추가했을때,

${ f(x_{0})= b }$이면 right continuous,

${ f(x_{0}) = a }$이면 left continuous,

${ a=b=f(x_{0}) }$이면 continuous이다.

## 같이보기

- [Semicontinuity](https://paraconsistent.github.io/analysis/2024/02/27/semicontinuity.html)