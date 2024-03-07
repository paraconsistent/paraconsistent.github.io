---
layout: post
math: "true"
toc: "true"
title: Partial function
categories: Logic
tags:
  - relation
---
## 정의

[binary relation](https://paraconsistent.github.io/logic/2024/02/26/relation.html#binary-relation) ${ f }$가 **partial function**(또는 **partial map**) ${ f:X \rightharpoonup Y }$이라는 것은

$$ \begin{gather} \mathrm{dom}(f) \subseteq X \\ \mathrm{ran}(f) \subseteq Y  \end{gather} $$

이고 [Univalence](https://paraconsistent.github.io/logic/2024/02/26/relation.html#unival) 조건

$$ x_{1}fy = x_{2}fy \Rightarrow x_{1}=x_{2}  $$

을 만족한다는 것이다. 

### source와 target

partial function ${ f : X \rightharpoonup Y }$가 주어졌을때,

${ X }$를 ${ f }$의 **source**, ${ Y }$를 ${ f }$의 **target**이라고 한다.

### totality와 surjectivity

paritial function ${ f : X \rightharpoonup Y }$가 주어졌을때

#### totality {#total}

$$ \mathrm{dom}(f) = X$$

이면 ${ f }$를 **(total) function**이라 부르고

$$ f: X \to Y $$

로 표기한다.

#### surjectivity {#surj}

$$ \mathrm{ran}(f)=Y $$

이면 ${ f }$를 **surjective function**이라 부른다.

## 참고문헌

1. [Partial function - Wikipedia](https://en.wikipedia.org/wiki/Partial_function)
1. [partial function in nLab (ncatlab.org)](https://ncatlab.org/nlab/show/partial+function)