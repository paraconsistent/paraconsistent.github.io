---
layout: post
math: "true"
toc: "true"
title: MONS and ONB
categories: Functional-Analysis
tags:
  - Hilbert-space
---
## Definitions

Given inner product space ${ (X,\langle \cdot,\cdot \rangle) }$,

**orthonormal system** is a subset ${S  }$ of ${ X }$ s.t.
- (orthogonality) ${ \langle x,y \rangle = 0 }$ for all distinct ${ x,y \in S }$
- (normality) ${ \langle x,x \rangle =1 }$ for all ${ x \in S }$

**maximal orthonormal system** (MONS) is a orthonormal system of maximal with inclusion ${ \subseteq }$

**orthonormal basis** (ONB) is a orthonormal system s.t.

$$ x = \sum_{y \in S} c_{y} y$$

for some sequence ${ \left\\{ c_{y} \right\\} }$ of scalars of ${ X }$.

## Gram-Schmidt process

Let

$$ \left \{ u_{1}, u_{2}, u_{3} \dots \right \} $$

be at most countable linearly independent susbset of inner product space ${ X }$. Define

$$ \begin{align} w_{1} &= u_{1} \\ w_{n+1} &= u_{n+1}-\sum_{j=1}^{n} \left( u_{n+1}, \frac{w_{j}}{\lVert w_{j} \rVert} \right) \frac{w_{j}}{\lVert w_{j} \rVert} \end{align} $$

and define

$$ v_{j}:= \frac{w_{j}}{\lVert w_{j} \rVert} $$

, then the set ${ \left\\{ v_{j} \right\\} }$ is orthornomal system such that

$$ \left\{ v_{j} \right\}_{j=1}^{n} \mbox{ spans the same subspace as } \left\{ u_{j} \right\}_{j=1}^{n}  $$

for all ${ n \in \mathbb{N} }$.

## Separable Hilbert space

We can prove every separable Hilbert space has an ONB without AC.

**Theorem** If ${ X }$ is a separable Hilbert space, then ${ X }$ has a ONB.

proof) Since ${ X }$ is separable, there exists a countable subset

$$ S = \left\{ x_{1},x_{2}, x_{3},\dots \right\} $$

such that ${ S }$ is dense in ${ X }$. Let ${ S' =S \setminus D }$ where

$$ D = \left\{ x_{k} \in S : x_{k} \mbox{ is a linear combination of } x_{i} \mbox{ for } i < k \right\} $$

Then ${ S' }$ is a linearly independent set of ${ X }$.

If apply Gram-Schmidt process on ${ S' }$, we get orthonormal system ${ S'' }$. Since ${ S'' }$ is dense in ${ X }$, ${ S'' }$ is the desired ONB.

## Hilbert space

**Theorem** Any Hilbert space has an ONB. Any MONS in a Hilbert space is an ONB.

pf) By the Zorn's lemma, any inner product space has at least one MONS.

Suppose ${ \{ x_{i} \}\_{i \in I} }$ is an arbitrary MONS in a Hilbert space ${ H }$. By the Bessel's inequality, there is at most a countable subset ${ I_{o} }$ of ${ I }$ s.t.

$$ \langle x_{i},x\rangle =0 \mbox{ for any } i \in I\setminus I_{0} $$

The completeness of ${ H }$ entails that

$$ x_{o} = \sum_{i \in I} \langle x,x_{i} \rangle x_{i} = \sum_{i \in I_{o} } \langle x,x_{i}\rangle x_{i}$$
On the other hand, ${ x=x_{o} }$ since

$$ \langle x_{o}-x,x_{i} \rangle = \langle x_{o},x_{i} \rangle-\langle x,x_{i} \rangle =0 $$

for any ${ i \in I }$ and the maximality of ${ \left\\{ x\_{i} \right\\} }$ gives ${ x\_{o} -x = 0}$

## References

1. [Anatolij Dvurečenskij. *Gleason's Theorem and Its Applications*, 1st ed. Springer Science+Business Media.](https://link.springer.com/book/10.1007/978-94-015-8222-3)