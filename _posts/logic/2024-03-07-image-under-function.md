---
layout: post
math: "true"
toc: "true"
title: 함수의 image 성질
categories: Logic
tags:
  - topology
---
## 성질

함수 ${ f: X\to Y}$와 대해서,

$$ \begin{gather} \mbox{(image)} &  f[A]=\{ f(x) : x\in A \} \\ \mbox{(inverse image)} & f^{-1}[B]=\{ x \in X: f(x) \in B \} \end{gather} $$

라고 하자. ${ f }$를 binary relation 관점에서 봤을때, inverse relation ${ f^{-1} }$도 binary relation이므로 그 성질들이 그대로 성립한다. 증명은 [binary relation의 image의 성질](https://paraconsistent.github.io/logic/2024/03/01/image-under-relation.html)을 참조하라.
### Monotonicity

${ A_{1} \subseteq A_{2} \subseteq X }$와 ${ B_{1} \subseteq B_{2} \subseteq Y }$에 대해

$$ \begin{gather} f[A_{1}] \subseteq f[A_{2}] \\ f^{-1}[B_{1}] \subseteq f^{-1}[B_{2}] \end{gather} $$

### Intersection

${ A_{1}, A_{2} \subseteq X }$에 대해,

$$ f[A_{1} \cap A_{2}] \subseteq f[A_{1}] \cap f[A_{2}] $$

inverse relation ${ f^{-1} }$는 [injective](https://paraconsistent.github.io/logic/2024/02/26/relation.html#inj)이므로 ${ B_{1},B_{2} \subseteq Y }$에 대해,

$$ f^{-1}[B_{1}\cap B_{2}]= f^{-1}[B_{1}] \cap f^{-1}[B_{2}] $$

### Union

${ (A_{\alpha}: \alpha \in I) \subseteq \mathcal{P}(X)}$에 대해,

$$ f[\bigcup_{\alpha \in I} A_{a}]=\bigcup_{\alpha \in I}f[A_{\alpha}] $$

${ (B_{\beta}:\beta \in J) \subseteq \mathcal{P}(Y)}$에 대해,

$$ f^{-1}[\bigcup_{\beta \in J} B_{\beta}] = \bigcup_{\beta \in J} f^{-1}[B_{\beta}]$$

### Difference

${ A_{1},A_{2} \subseteq X }$에 대해,

$$ f[A-B] \subseteq f[A]-f[B] $$

등호는 ${ f }$가 [injective](https://paraconsistent.github.io/logic/2024/02/26/relation.html#inj)일 때 성립한다.

${ f^{-1} }$는 injective relation이므로, ${ B_{1},B_{2} \subseteq Y }$에 대해,

$$ f^{-1}[B_{1}-B_{2}]=f^{-1}[B_{1}]-f^{-1}[B_{2}] $$

### Saturation

${ A \subseteq X }$에 대해,

$$ A \subseteq f^{-1}[f[A]] $$

등호는 ${ f }$가 [injective](https://paraconsistent.github.io/logic/2024/02/26/relation.html#inj)일 때 성립한다.

${ B \subseteq Y }$에 대해,

$$ f[f^{-1}[B]] \subseteq B$$

등호는 ${ f }$가 [surjective]일 때 성립한다.
