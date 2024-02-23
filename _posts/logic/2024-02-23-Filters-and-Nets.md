---
layout: post
math: "true"
toc: "true"
title: Filters and Nets
categories: Logic
tags:
  - filter
  - net
  - order
---
## Filters and Ideals

Let ${ \mathcal{F} }$ be a nonempty collection of susbsets of a set ${ X }$. We say ${ \mathcal{F} }$ is a **filter** on ${ X }$ if

(1) ${\exists S \in \mathcal{F})\  S \subseteq T \subseteq X \Rightarrow T \in \mathcal{F} }$, and
 
(2) ${ S,T \in \mathcal{F} \Rightarrow S \cap T \in \mathcal{F} }$

**Example** ${ \mathcal{P}(X) }$ is a filter on ${ X }$ and it is called the **improper filter**. Any other filter on ${ X }$ will be called a **proper filter**.

A filter ${ \mathcal{F} }$ is proper iff

(3) ${ \emptyset \notin \mathcal{F} }$

A nonempty collection ${ \mathcal{J} }$ of subsets of a set ${ X }$ is an **ideal** on ${ X }$ if

(1) ${ (\exists S \in \mathcal{J}) \  S \supseteq T \Rightarrow T \in \mathcal{J}  }$, and

(2) ${ S,T \in  \mathcal{J} \Rightarrow S \cup T \in \mathcal{J}}$.

${ \mathcal{P}(X) }$ is called **improper ideal**. Any other ideal on ${ X }$ is called a **proper ideal**.

ideal ${ \mathcal{J} }$ is proper iff

(3) ${ X \notin \mathcal{J} }$

A ${ \sigma }$-idela is an ideal ${ \mathcal{J} }$ is closed under countable unions.

There is a simple correspondence between filters and ideals.

$$ \mathcal{F} \subseteq \mathcal{P}(X),\quad \mathcal{J} = \{ X \setminus S : S \in \mathcal{F} \} $$

Then,

$$ \mathcal{F} \mbox{ is a filter iff } \mathcal{J} \mbox{ is a ideal}  $$

We say that ${ \mathcal{F} }$ and ${ \mathcal{J} }$ are dual to each other.

Suppose ${\emptyset \neq \mathcal{J} \subseteq \mathcal{P}(X)}$, and ${ \mathcal{F} }$ is dual collection of ${ \mathcal{J} }$. Say that a set ${ S \subseteq X}$ is **small** if ${ S \in \mathcal{J} }$, or **large** if ${ S \in \mathcal{F} }$.

Then ${ \mathcal{J} }$ is an ideal and ${ \mathcal{F} }$ is a filter iff

(1) any subset of a small set is small, and

(2) the union of two small sets is small.

The ideal and filter are proper iff

(3) not every set is small.

Other words sometimes used in place of small are **negligible** and **null**.

Other words sometimes used in place of large are **residual** or **generic**. Also, a large subset of ${ X }$ is **almost all** of ${ X }$. We might also say that a condition ${ K }$ on pts ${ x \in X }$ is satisfied **almost everywhere** or **almost always**, or is **${ \mathcal{F} }$-true** or **almost ture**, if the set

$$ \{ x \in X : K \mbox{ is satisfied at } x \} $$

is a member of ${ \mathcal{F} }$.

Given any ${ \mathcal{G} \subseteq \mathcal{P}(X) }$, there exists a smallest filter (or ideal) that contatins ${ \mathcal{G} }$ - namely, the intersection of all the filters (or ideals) that contain ${ \mathcal{G} }$. We call it the filter (resp. the ideal) **generated** by ${ \mathcal{G} }$; we say that ${ \mathcal{G} }$ is generating set for it.

### filterbase and filtersubbase

**Definition** Let ${ \emptyset \neq \mathcal{G} \subseteq \mathcal{P}(X) }$.

1. ${ \mathcal{G} }$ is called a **filterbase** on ${ X }$ if each member of ${ \mathcal{G} }$ is nonempty, and for each pair of sets ${ A,B \in \mathcal{G} }$ there eixsts some ${ C \in \mathcal{G} }$ with ${ C \subseteq A \cap B }$.
1. We say that ${ \mathcal{G} }$ is a **filter subbase** on ${ X }$, or ${ \mathcal{G} }$ has the **finite intersection property** if the intersection of finitely many elements of ${ \mathcal{G} }$ is always nonempty.


**Definition** ${ \mathcal{F} }$ is a **superfilter** of ${ \mathcal{G} }$ whenever ${ \mathcal{F} }$ is a filter and ${ \mathcal{F} \supseteq \mathcal{G} }$.

**Definition** Let ${ \emptyset \neq \mathcal{F} \subseteq \mathcal{P}(X) }$. TFAE:

(i) ${ \mathcal{F} }$ is a proper filter on ${ X }$, and the ${ \mathcal{P}(X) \setminus \mathcal{F} }$ is an ideal

(ii) ${ \mathcal{F} }$ is a proper filter on ${ X }$ that also satisfies:

$$ (\forall K \subseteq X)\ K \in \mathcal{F} \mbox{ or } X \setminus K \in \mathcal{F} $$

(iii) ${ \mathcal{F} }$ is a **maximal filter** on ${ X }$. That is, ${ \mathcal{F} }$ is a proper filter on ${ X }$ and no other proper filter on ${ X }$ contains ${ \mathcal{F} }$.

(iv) ${ \mathcal{F} }$  is a maximal filter subbase on ${ X }$, i.e., ${ \mathcal{F} }$ is a filter subbase on ${ X }$, and no other filter subbase contains ${ \mathcal{F} }$.

(v) ${ \mathcal{F} }$ is a proper filter on ${ X }$,

$$ S_{1} \cup S_{2} \in \mathcal{F} \Rightarrow S_{1} \in \mathcal{F} \mbox{ or } S_{2} \in \mathcal{F} $$

If any of them are satisfied, we say ${ \mathcal{F} }$ is an **ultrafilter**.

## Nets

**Definition** A [preordered set](https://paraconsistent.github.io/logic/2024/02/15/preorder.html) ${ (J,\prec) }$ is called directed set if

$$ (\forall x,y \in J, \exists u \in J)\  x \prec u \mbox{ and } y \prec u$$

**Definition** Let ${ J }$ be a directed set. A **net** in a set ${ X }$ is any function ${ x_{\bullet} : J \to X }$.

- We usually write ${ x_{\bullet}(\alpha) }$ as ${ x_{\alpha} }$.
- ${ (x\_{\alpha})\_{\alpha \in J} }$ or ${ \\{x\_{\alpha}\\}\_{\alpha \in J} }$ are also notations for a net from ${ J }$.

nets are also sometimes called **generalized sequences** or **Moore-Smith sequences**.

**Definition** Let ${ x_{\bullet} : J \to X}$ be a net, and let ${ S \subseteq X }$. We say that

${ S }$ is a **tail set** of the net if ${ S }$ if ${ S }$ is of the form

$$ \{ x_{\alpha}: \alpha \succ \alpha_{0} \} $$

for some ${ \alpha_{0} \in J}$

${ S }$ is an **eventual** (or residual) set of the net if ${ S }$ contains some tail set. In this case we say that ${ x\_{\alpha} \in S}$ happens **eventually**, or that ${ x\_{\alpha} \in S }$ happens **for arbitrarily large values of** ${ \alpha }$.

${ S }$ is a **frequent** (or cofinal) set of the net if ${ S }$ meets every tail set, i.e., if for each ${ \alpha_{0} \in J }$ there is some ${ \alpha \succ \alpha_{0}}$ s.t. ${ x_{\alpha} \in S }$. In this case we say that ${ x_{\alpha} \in S }$ happens **frequently**, or that ${ x_{\alpha} \in S}$ happens **for arbitrary large values of** ${ \alpha }$.

${ S }$ is **infrequent** if it is not frequent.

## Correspondence between nets and filters

Let any net ${ x_{\bullet} }$ in a set ${ X }$ be given. Then

$$ \mathcal{B} = \{ \mbox{tail sets of the net } x_{\bullet} \} $$

is a filterbase on ${ X }$; the proper filter that it generates is

$$ \mathcal{F} = \{ \mbox{eventual sets of the net } x_{\bullet} \} $$

We call these the **filter base of the tails** and **eventuality filter** of ${ x\_{\bullet} }$, respectively. (Some mathematicians call ${ \mathcal{F} }$ the filter of tails of ${ x\_{\bullet} }$)

The proper ideal that is dual to filter ${ \mathcal{F} }$ is the collection of all infrequent subsets of ${ X }$.

## References

1. Eric Schechter. *Handbook of Analysis and Its Foundations*, Academic Press.
