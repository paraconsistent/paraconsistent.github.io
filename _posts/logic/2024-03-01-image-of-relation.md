---
layout: post
math: "true"
toc: "true"
title: binary relation의 image의 성질
categories: Logic
tags:
  - relation
---
## 성질

${ R }$이 ${ A }$ 위의 binary relation이라고 하자.

### Monotonicity

${ C \subseteq B\subseteq A }$에 대해,

$$ R[C] \subseteq R[B] $$

### Intersection

${ B,C \subseteq A }$에 대해,

$$ R[B \cap C] \subseteq R[B] \cap R[C] $$

등호는 ${ R }$이 [injective](https://paraconsistent.github.io/logic/2024/02/26/relation.html#inj)일 때 성립한다.

### Union

${ (B\_{\alpha}: \alpha \in J) \subseteq \mathcal{P}(A)  }$에 대해,

$$ R[\bigcup_{\alpha \in J} B_{\alpha}] = \bigcup_{\alpha \in J} R[B_{\alpha}]  $$

### Difference

${ B,C \subseteq A }$에 대해

$$ R[B-C] \supseteq R[B] - R[C] $$

이고 등호는 ${ R }$이 [injective](https://paraconsistent.github.io/logic/2024/02/26/relation.html#inj)일 때 성립한다.