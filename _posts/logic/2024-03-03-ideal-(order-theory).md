---
layout: post
math: "true"
toc: "true"
title: Ideal (order theory)
categories: Logic
tags:
  - order
  - lattice
  - filter
---
## 정의

주어진 lattice ${ (L, \wedge, \vee) }$에 대해, 그 sublattice ${ (I,\wedge,\vee) }$가 다음 성질을 만족하면 ${ I }$는 ${ L }$의 **ideal**이라고 한다.

$$ a \in L \mbox{ and }  x \in I \Rightarrow a \wedge x \in I $$

meet ${ \wedge }$를 곱으로 봤을때 ${ }$대수학에서 ideal와 같다는 것을 알 수 있다.

## filter

**filter (또는 dual ideal)**은 ideal을 다음과 같이 [dualize](https://paraconsistent.github.io/logic/2024/03/03/duality-(order-theory).html)한 것이다.

$$ a \in L \mbox{ and } x \in F \Rightarrow a \vee x \in F $$

## 순서론적 관점


### lattice에서 정의된 poset에서

주어진 lattice ${ L=(L,\wedge,\vee) }$는 다음 순서로 poset ${ L=(L,\le) }$이다.

$$ a \le b \iff a \wedge b = a $$

이때 [lower set (또는 down-set)](https://paraconsistent.github.io/logic/2024/02/28/upper-set.html#%EC%A0%95%EC%9D%98) ${ I }$는 다음과 같이 정의된다.

$$ \forall   a \in L, \exists x \in I,\quad a \le x \Rightarrow a \in I $$

${ I }$가 ${ L }$의 ideal이라는 것은 다음 두 조건을 만족시키는 것과 동치이다.

$$ \begin{gather} \mbox{i.} & x \in I \mbox{ and } y \in I \Rightarrow x\vee y \in I \\ \mbox{ii.} & I \mbox{ is a lower set of } L \end{gather} $$

증명

${ I }$가 ideal이라고 하자.

${ I }$가 sublattice이므로 i을 만족.

${ I }$가 ideal이므로, 임의의 ${ a \in L }$과 ${ x \in I }$에 대해

$$ a \le x \iff a=a \wedge x \in I $$

따라서 ${ I }$는 lower set이므로 ii 만족.

반대로, ${ I }$가 i과 ii를 만족한다고 하자.

임의의 ${ x \in I }$에 대해, ${ x \wedge y \le x }$이므로 ii에 의해 ${ x \wedge y \in I }$. i과 결합하면, ${ I }$는 ${ L }$의 sublattice.

${ I }$가 lower set이므로 임의의 ${ a \in L }$과 임의의 ${ x \in I }$에 대해,

$$ a \wedge x \le x \Rightarrow a\wedge x \in I  $$

따라서 ${ I }$는 ideal.

위의 [dual statement](https://paraconsistent.github.io/logic/2024/03/03/duality-(order-theory).html)는 다음과 같다.

${ F }$가 ${ L }$의 filter라는 것은 다음 두 조건을 만족시키는 것과 동치이다.

$$ \begin{gather} \mbox{i.} & x \in F \mbox{ and } y \in F \Rightarrow x\wedge y \in F \\ \mbox{ii.} & F \mbox{ is an upper set of } L \end{gather} $$

여기서 [upper set](https://paraconsistent.github.io/logic/2024/02/28/upper-set.html) 조건은 lower set의 dual인 다음 조건이다.

$$ \forall a \in L, \exists x \in F, \quad a \ge x \Rightarrow a \in F  $$

### 일반적인 poset으로 확장

lattice에는 ${ x \wedge y = \inf \{ x,y \} }$ 와 ${ x \vee y = \sup \{ x,y \} }$에 닫혀있어야 한다는 조건이 필요했다. 일반적인 poset에서는 meet와 joint에 대해서 닫혀있을 필요가 없으므로 다음과 같이 조건을 약화한다.

poset ${ P=(P,\le) }$에 대해 ${ I }$가 ideal이라는 것은

$$ \begin{gather} \mbox{(upward directedness)} & \forall x,y \in I,\exists z \in I, \quad x \le z \mbox{ and } y \le z \\ \mbox{(downward closure)} & \forall p \in P, \exists x \in I,\quad p \le x \Rightarrow p \in I\end{gather} $$

upward directedness는 join에 대해 닫혀있다는 조건의 약화이고 ${ I }$가[join-semilattice](https://paraconsistent.github.io/logic/2024/02/27/lattice.html#semilattice)이면, lattice에서 ideal 동치조건 i과 같다.

downward closure는 ${ I }$가 lower set이라는 것과 동치

## 함께보기

- [filter](https://paraconsistent.github.io/logic/2024/02/27/filter.html)
- [lattice](https://paraconsistent.github.io/logic/2024/02/27/lattice.html)

## 참고문헌

1. Grätzer (2011). *Lattice Theory: Foundation*, Birkhäuser.