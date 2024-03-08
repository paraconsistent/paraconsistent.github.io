---
layout: post
math: "true"
toc: "true"
title: Associative algebra
categories: Algebra
tags:
  - algebraic-structure
---
## 정의

### Associative ${ R }$-algebra

${ R }$이 commutative ring이고 ring ${ A }$가 ${ R }$-module이라고 하자. 임의의 ${ r \in R }$과 임의의 ${ x,y \in A }$에 대해 scalar multiplication ${ \cdot R \times A \to A}$가

$$ r \cdot(xy)=(r\cdot x)y = x(r \cdot y) $$

을 만족시키면 ${ A }$를 **associative algebra over ${ R }$** 또는 **associative ${ R }$-algebra**라고 한다.

### ring homomorphism을 통한 정의

ring homomorphism ${ \varphi : R \to A }$가 주어져 있고 ${ \mathrm{ran}\, \varphi }$가 ${ A }$의 center에 들어갈 때 다음 ${ A }$에 ${ R }$-module structure를 줄 수 있다.

$$ \begin{eqnarray} R \times A &\to& A \\ (r,a) &\mapsto& \varphi(r)a \end{eqnarray} $$

이때 ${ \varphi }$를 **structure map**이라고 부른다.

### Algebra homomorphism

${ A }$와 ${ B }$가 associative ${ R }$-algebra일 때 ring homomorphism ${ f : A \to B }$가 ${ R }$-linear map이면 associative ${ R }$-algebra homomorphism이라고 한다.