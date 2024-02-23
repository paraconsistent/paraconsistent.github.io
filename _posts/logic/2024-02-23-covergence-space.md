---
layout: post
math: "true"
toc: "true"
title: Convergence Spaces
categories: Logic
tags:
  - net
  - filter
  - convergence
  - limit
---
## convergence space

**convergence space** is a set ${ X }$ equipped with a function

$$ \lim : \{ \mbox{proper filters on X} \} \to \mathcal{P}(X)$$

Whenever ${ (X,\lim) }$ is a convergence space, then we shall extend the function lim in the following ways:

- If ${ \mathcal{B} }$ is a [filterbase](https://paraconsistent.github.io/logic/2024/02/23/Filters-and-Nets.html#filterbase-and-filtersubbase) on ${ X }$, then ${ \lim \mathcal{B} =\lim \mathcal{F}}$ where ${ \mathcal{F} }$ is the filter gen'd by ${ \mathcal{B} }$
- If ${ x_{\bullet} }$ is a [net](https://paraconsistent.github.io/logic/2024/02/23/Filters-and-Nets.html#nets) in ${ X }$, then ${ \lim x_{\bullet} = \lim \mathcal{F}}$ where ${ \mathcal{F} }$ is the [eventuality filter](https://paraconsistent.github.io/logic/2024/02/23/Filters-and-Nets.html#correspondence-between-nets-and-filters) of ${ x_{\bullet} }$

**Notations** If ${ \mathcal{F}  }$ is a proper filter or a net, the expression

$$ z \in \lim \mathcal{F} $$

will be read as

"${ z }$ is a **limit** of ${ \mathcal{F} }$."

It may also be writeen as

$$ \mathcal{F}\to z $$

and read as "${ \mathcal{F} }$ **converges** to ${ z }$."

**Definition** Let ${ p:X \to Y }$ be a mapping from one convergence space into another. We say that ${ p }$ is **convergence preserving** if

whenever ${ x_{\bullet} }$ is a net convergeing to a limit ${ x }$ in ${ X }$, then the net ${p(x_{\bullet})  }$ converges to ${ p(x) }$ in ${ Y }$

or, equivalently,

whenever ${ \mathcal{F} }$ is a filter converging to a limit ${ x }$ in ${ X }$, then the filter

$$ \{ S \subseteq Y : p^{-1}(S) \in \mathcal{F} \} $$

converges to ${ p(x) }$ in ${ Y }$.

## Refereces

1. Eric Schechter. *Handbook of Analysis and Its Foundations*, Academic Press.