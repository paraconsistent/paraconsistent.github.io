---
layout: post
math: "true"
toc: "true"
title: Hölder's inequality
categories: Calculus
tags:
  - inequality
---
## Statement

Suppose ${ 1<p<\infty }$ and ${ p^{-1} + q^{-1} = 1 }$. If ${ f }$ and ${ g }$ are measureable functions on ${ X }$, then

$$ \lVert fg \rVert_{1} \le \lVert f \rVert_{p} \lVert g \rVert_{q} $$

In particular, if ${ f\in L^{p} }$ and ${ g \in L^{q} }$, then ${ fg \in L^{1} }$, and in this case equality holds iff

$$ \alpha \lvert f \rvert^{p}=\beta \lvert g \rvert^{q} $$

a.e. for some constant ${ (\alpha,\beta) \neq (0,0) }$.

### Lemma

If ${ a \ge 0, b \ge 0 }$, and ${ 0<\lambda<1 }$, then

$$ a^{\lambda}b^{1-\lambda} \le \lambda a + (1-\lambda)b $$

proof of the lemma) If ${ b=0 }$, obvious. Suppose ${ b \neq 0 }$, dviding both sides by ${ b }$ and setting ${ t=a / b }$,

$$ t^{\lambda} \le \lambda t + (1-\lambda) $$

Consider ${ f(t)=t^{\lambda} - \lambda t }$,

$$ f'(t) = \lambda t^{\lambda-1} - \lambda>0 $$

for ${ 0 \le t < 1 }$. Therefore ${ f(t) }$ has maximum value at ${ t=1 }$ and

$$ t^{\lambda}-\lambda t \le 1-\lambda $$

equality holds iff t=1.

### proof of the inequality

The result is trivial if ${ \lVert f \rVert_{p}=0 }$ or ${ \lVert g \rVert_{q} =0}$, or if ${ \lVert f \rVert_{p} = \infty }$ or ${ \lVert g \rVert_{q}=\infty }$.

Let ${ F=f / \lVert f \rVert_{p}, G =g / \lVert g \rVert_{q}  }$

Then,

$$ \lvert F(x)G(x) \rvert  \le p^{-1}\lvert F(x) \rvert^{p} + q^{-1} \lvert G(x) \rvert^{q}$$

for all ${ x \in X }$. Intergration of both sides yields,

$$ \lVert FG \rVert_{1} \le p^{-1}\lVert F \rVert_{p}^{p}+q^{-1} \lVert G \rVert_{q}^{q}=p^{-1}+q^{-1}=1$$

Equality holds iff

$$ \lvert F(x)G(x) \rvert =p^{-1}\lvert F(x) \rvert^{p} + q^{-1} \lvert G(x) \rvert^{q}$$

a.e. on ${ X }$, i.e.,

$$ \frac{\lvert f \rvert^{p}}{\lVert f \rVert_{p}^{p}} = \frac{\lvert g \rvert^{q}}{\lVert g \rVert_{q}^{q}} $$

a.e. on ${ X }$.

## References

1. Gerald B. Folland, *Real Analysis - Modern Techiques and Their Applications*, 2nd ed., 182p.
2. Walter Rudin, *Real and Complex Analysis*, 3rd ed., 63-65p.