---
layout: post
math: "true"
toc: "true"
title: Compact Hausdorff space
categories: General-Topology
tags:
  - compact
---
## 정의

compact space이면서 동시에 Hausdorff space인 위상공간 ${ X }$를 compact Hausdorff space라고 한다.

### 모티브

${ X }$가 compact space이면 다음 성질이 성립한다.

1. 임의의 위상공간 ${ Y }$와 임의의 연속함수 ${ f:X \to Y }$에 대해, ${ f(X)}$는 ${ Y }$의 compact subset.
1. 임의의 closed subset ${ C \subseteq X}$에 대해, ${ C }$는 compact.

${ X }$가 Hausdorff space이면 다음 성질이 성립한다.

1. 임의의 subspace ${ Y \subseteq X }$에 대해, ${ Y }$는 Hausdorff space.
1. 임의의 compact subset ${ K \subseteq X}$에 대해, ${ K }$는 closed.

따라서 두 compact Hausdorff space ${ X }$와 ${ Y }$에 대해 다음 성질을 만족한다.

1. ${ K \subset X }$에 대해서, ${ K }$가 compact ${ \Leftrightarrow }$ ${ K }$가 closed.
1. 임의의 연속함수 ${ f: X \to Y }$는 closed map.

### closed map lemma

${ X }$가 compact space이고 ${ Y }$가 Hausdorff space이면, 임의의 연속함수 ${ f: X \to Y }$는 closed이고 proper[^1]이다.

증명

${ f }$는 closed
: compact space ${ X }$에서 ${ C }$가 closed면 compact이므로 ${ f(C) }$가 compact. 그런데 Hausdorff space ${ Y }$에서 compact이면 closed이므로 ${ f(C) }$는 closed.

${ f }$는 proper
: ${ K \subseteq Y }$가 compact ${ \Rightarrow }$ ${ K }$가 closed ${ \Rightarrow }$ ${ f^{-1}(K) }$가 closed ${ \Rightarrow }$ ${ f^{-1}(K) }$가 compact.

## 참고문헌

1. Munkres (2000). *Topology*, 2nd Edition.
1. [Wikipedia. *Open and closed maps*. (Retrieved: Mar 3, 2024)](https://en.wikipedia.org/wiki/Open_and_closed_maps)

---
[1]: K가 compact ⇒ K의 preimage under f가 compact.