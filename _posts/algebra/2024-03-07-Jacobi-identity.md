---
layout: post
math: "true"
toc: "true"
title: Jacobi identity
categories: Algebra
tags:
  - lie-algebra
---
## Jacobi idenitity

$$ [X_{1},[X_{2},X_{3}]] + [X_{2},[X_{3},X_{1}] ]+ [X_{3},[X_{1},X_{2}]] =0$$

### 증명

$$ [X_{1},[X_{2},X_{3}]]= X_{1}X_{2}X_{3}-X_{2}X_{3}X_{1}-X_{1}X_{3}X_{2}+X_{3}X_{2}X_{1} $$

3-cycle ${ \sigma = (1\,2\,3) }$에 대해서 다음과 같이 치환해보자.

$$ \sigma(X_{i}X_{j}X_{k}):=X_{\sigma(i)}X_{\sigma(j)}X_{\sigma(k)} $$

그러면

$$ \begin{gather} \sum_{j=0}^{2} \sigma^{j}(X_{2}X_{3}X_{1}) = \sum_{j=0}^{2} \sigma^{j+1} (X_{1}X_{2}X_{3})=\sum_{j=0}^{2}\sigma^{j}(X_{1}X_{2}X_{3}) \\ \sum_{j=0}^{2} \sigma^{j}(X_{3}X_{2}X_{1}) = \sum_{j=0}^{2} \sigma^{j+2} (X_{1}X_{3}X_{2})=\sum_{j=0}^{2}\sigma^{j}(X_{1}X_{3}X_{2})\end{gather}$$

따라서

$$ \sum_{j=0}^{2} [X_{\sigma^{j}(1)},[X_{\sigma^{j}(2)},X_{\sigma^{j}(3)}]]=0$$
