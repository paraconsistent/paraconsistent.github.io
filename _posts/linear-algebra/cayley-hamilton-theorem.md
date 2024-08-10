---
layout: post
math: "true"
toc: "true"
title: 케일리-해밀턴 정리
categories: Linear-Algebra
tags:
  - determinant
  - cayley
  - hamilton
---
## 정의

${ A }$가 ${ n }$차 정사각행렬이고, ${ f(x) = \det(xI_{n}-A) }$일 때, ${ f(A)=0_{n} }$

## 증명

${ n }$차 정사각행렬 ${ B }$를 다음과 같이 정의하자.
$$ B = \mbox{adj}(xI_{n} - A)=\sum_{k=0}^{n-1} B_{k}x^{k} $$

수반행렬의 정의에 따라,

$$ \begin{eqnarray} f(x) &=& B(xI_{n}-A) \\ &=& \sum_{k=0}^{n-1} B_{k}x^{k+1} - \sum_{k=0}^{n-1}B_{k}Ax^{k} \end{eqnarray} $$

따라서

$$ f(A) = \sum^{n-1}_{k=0} B_{k}A^{k+1} - \sum_{k=0}^{n-1}B_{k}A^{k+1} =0_{n}$$