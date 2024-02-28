---
layout: post
math: "true"
toc: "true"
title: Filters and Ideals
categories: Logic
tags:
  - filter
  - order
---
## 집합론적 정의

### Filter

${ \mathcal{F} \subseteq \mathcal{P}(X) }$가 다음 세 조건을 만족하면 **filter** on X라고 부른다.

$$ \begin{gather} (\mbox{nontriviality}) &  \mathcal{F} \neq \emptyset \\ \mbox{(downard directed)} & A,B \in F \Rightarrow A \cap B \in F \\  \mbox{(upward closure)} & \exists A \in F, \quad A \subseteq B \subseteq X\Rightarrow B \in \mathcal{F}  \end{gather}$$

filter는 위상공간에서 근방(neighborhood)를 모방한 것이다.

${N}$이 ${ x }$의 근방이라는 것은 어떤 열린집합 ${ U }$가 존재해서,

$$ x \in U \subseteq N $$

이라는 것이므로  ${ U }$를 포함하는 모든 집합은 ${ x }$의 근방이다.

또 두 근방 ${ N\_{1}, N\_{2} }$이 있을 때,

$$ x \in U \subseteq N_{1} \cap N_{2}  $$ 
이므로 ${ N_{1} \cap N_{2} }$ 또한 ${ x }$의 근방임을 알 수 있다. 실제로 위상공간 ${ (X,\mathcal{T}) }$와 점 ${ x \in X }$ 주어졌을때,

$$ \mathcal{N}(x)=\{ N \in \mathcal{P}(X): x \in U \subseteq N \mbox{ for some } U \in \mathcal{T}\} $$

는 filter이다.

만약 filter ${ \mathcal{F} }$가 공집합을 포함하면 조건 1에 의해

$$ \mathcal{F} = \mathcal{P}(X)$$

이 된다.

${ \mathcal{F} = \mathcal{P}(X) }$인 filter를 **improper filter**라고 하고 improper가 아닌 경우 **proper filter**라고 한다.

### Ideal

nonempty ${ \mathcal{J} \subseteq \mathcal{P}(X) }$가 다음 조건을 만족하면 **ideal** on X라고 부른다.

1. ${ S \in \mathcal{J} }$이고 ${ S \supseteq T }$이면 ${ T \in \mathcal{J} }$
1. ${ S,T \in \mathcal{J} \Rightarrow S \cup T}$

${ \mathcal{J}=\mathcal{P}(X) }$인 경우 **improper ideal**이라고 하고 improper가 아닌 경우 **proper ideal**이라고 한다.


### Filter ↔ Ideal duality

${ \mathcal{F} }$가 filter on ${ X }$일 때,

$$ \mathcal{J}=\{ X \setminus F: F\in \mathcal{F} \} $$

는 ideal이 되고 이 ${ \mathcal{J} }$를 ${ \mathcal{F} }$의 **dual**이라고 한다.

반대로 ${ \mathcal{J} }$가 ideal on ${ X }$일 때

$$ \mathcal{F}=\{ X \setminus J : J \in \mathcal{J} \} $$

는 filter가 되고 이 ${ \mathcal{F} }$를 ${ \mathcal{J} }$의 **dual**이라고 한다.

## 순서론적 정의

위에서 ${ X }$ 위의 필터 ${ \mathcal{F} }$가 ${ \mathcal{P}(X) }$의 부분모임이므로 ${ (\mathcal{F},\subseteq) }$가 [poset](https://paraconsistent.github.io/logic/2024/02/15/Poset.html)임을 알 수 있다. 그러면 ${ \subseteq }$를 순서 ${ \le }$로 보면 poset 위에서 filter를 정의할 수 있지 않을까?

주어진 poset ${ (P,\le) }$의 부분집합 ${ F }$가 다음 세 조건을 만족시키면 filter라고 한다.

$$ \begin{gather} \mbox{(nontriviality)} & F \neq \emptyset \\ \mbox{(downward directed)} & \forall x,y \in F, \exists z \in F,\quad z \le x \mbox{ and } z \le y \\ \mbox{(upward closure)} &\forall x \in F,\exists  p \in P,\quad x \le p \Rightarrow p \in F \end{gather}$$

**Exercise** 1. ${ (\mathcal{P}(X),\subseteq) }$에서 ${ \mathcal{F} \subseteq \mathcal{P}(X)}$가 순서론적 filter이면 정확히 집합론적 filter임을 보여라.

풀이: (downard directed)만 보이면 충분하다.

${ A,B \in \mathcal{F} }$라고 하자 순서의 downard directed에 의해 ${ \exists C  \in \mathcal{F},\ C \subseteq A \cap B  }$ 다시 upward closure에 의해 ${ A \cap B  \in \mathcal{F}}$

만약 ${ (P,\le) }$가 [meet-semilattice](https://paraconsistent.github.io/logic/2024/02/27/lattice.html#semilattice)이면, 다시말해,

$$ a,b \in P \Rightarrow a \wedge b =\inf \{ a,b \} \in P $$

이면, upward closure에 의해 ${ a \wedge b \in \mathcal{F} }$임을 쉽게 알 수 있다. 집합론적 정의가 정확히 meet-semilattice의 경우이다.

반대로 말하자면 순서론적 정의는 meet-semilattice가 아닌 경우로 집합론적 정의를 확장한 것이다.

## 함께보기

- [Lattice](https://paraconsistent.github.io/logic/2024/02/27/lattice.html)
- upper set
- net

## 참고문헌

1. Eric Schechter (1996). *Handbook of Analysis and Its Applications*, Academic Press.