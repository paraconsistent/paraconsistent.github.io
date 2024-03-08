---
layout: post
title: Antihomomorphism
math: "true"
categories: Category-Theory
tags:
  - star-algebra
toc: "true"
---
## 정의

### Antihomomorphism

${ f:X \to Y }$가 **antihomomorphism**이라는 것은 ${ f: X \to Y^{\mathrm{op}} }$로 봤을 때 **homomorphism**인 것을 말한다.

구체적으로,

$$ f(xy) = f(y)f(x) $$

를 만족하는 함수이다.

homo-를 endo-, auto-, mono-, epi-, iso- 등으로 치환하면 homomorphism의 그 의미와 똑같이 둔다.

### Involution

**involution**은 ${ f^{2}=\mathrm{id} }$를 만족하는 antiautomorphism ${ f }$를 지칭한다.

## 예시

### Inverse

group ${ G }$에 대해 antiautomorphism ${ g \mapsto g^{-1}}$는 involution이다.

$$\begin{gather} (g^{-1})^{-1}=g \\ (gh)^{-1}=h^{-1}g^{-1} \end{gather}  $$

### Transpose

matrix의 transpose ${ A \mapsto A^{t} }$는 involution이다.

$$ \begin{gather} (A^{t})^{t}= A \\ (AB)^{t}=B^{t}A^{t} \end{gather} $$

### Adjoint

inner product space ${ V }$ 위의 linear operator의 adjoint ${ A \mapsto A^{\dagger} }$는 involution이다.

$$ \begin{gather} (A^{\dagger})^{\dagger} = A \\ (AB)^{\dagger} =B^{\dagger}A^{\dagger} \end{gather} $$

### Quaternion conjugation

quarternion ${ \mathbb{H} }$에 대해 quaternion conjugation ${ q \mapsto q^{\ast} }$는 involution이다.

$$ \begin{gather} (q^{\ast})^{\ast}=q \\ (pq)^{\ast}=q^{\ast}p^{\ast} \end{gather} $$

## References

1. Involution. _Encyclopedia of Mathematics._ URL: [http://encyclopediaofmath.org/index.php?title=Involution&oldid=47428](http://encyclopediaofmath.org/index.php?title=Involution&oldid=47428)
