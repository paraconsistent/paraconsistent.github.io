---
layout: post
math: "true"
toc: "false"
title: 수렴하는 두 수열의 곱
categories: Calculus
tags:
  - sequence
---
## 정리

${ a\_{n} \to a }$ 이고 ${ b\_{n} \to b }$이라고 하자. 그러면

$$ a_{n} b_{n} \to ab $$

이다.

## 증명

충분히 작은 ${ \varepsilon >0  }$에 대해,

${ N\_{1}: n \ge N\_{1} \Rightarrow \left\lvert a\_{n} - a \right\rvert < \frac{\varepsilon}{2(\left\lvert b \right\rvert +1)} }$

${ N\_{2}: n \ge N\_{2} \Rightarrow \left\lvert b\_{n} -b \right\rvert < \frac{\varepsilon}{2(\left\lvert a \right\rvert+1)}<1 }$[^1]

${ N = \min(N\_{1},N\_{2}) }$ 이라고 하면,

${ n \ge N }$일 때,

$$ \begin{eqnarray}\left\lvert a_{n}b_{n} -ab \right\rvert &\le& \left\lvert a_{n} -a \right\rvert \left\lvert b_{n} \right\rvert + \left\lvert a \right\rvert \left\lvert b_{n} -b \right\rvert \\ &<& \frac{\varepsilon}{2(\left\lvert b \right\rvert +1)} (\left\lvert b\right\rvert+1) + \frac{\varepsilon\left\lvert a \right\rvert}{2(\left\lvert a \right\rvert+1)} \\ &<& \varepsilon\end{eqnarray} $$

## 주석

[^1]: 분모가 0이 되는 상황을 피하고자 1을 더해줬다.