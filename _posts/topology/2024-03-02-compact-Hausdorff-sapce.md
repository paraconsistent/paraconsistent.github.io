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

## 모티브

${ X }$가 compact space이면 다음 성질이 성립한다.

1. 임의의 위상공간 ${ Y }$와 임의의 연속함수 ${ f:X \to Y }$에 대해, ${ f(X)}$는 ${ Y }$의 compact subset.
1. 임의의 closed subset ${ C \subseteq X}$에 대해, ${ C }$는 compact.

${ X }$가 Hausdorff space이면 다음 성질이 성립한다.

1. 임의의 subspace ${ Y \subseteq X }$에 대해, ${ Y }$는 Hausdorff space.
1. 임의의 compact subset ${ K \subseteq X}$에 대해, ${ K }$는 closed.

따라서 두 compact Hausdorff space ${ X }$와 ${ Y }$에 대해 다음 성질을 만족한다.

1. ${ K \subset X }$에 대해서, ${ K }$가 compact ${ \Leftrightarrow }$ ${ K }$가 closed.
2. 임의의 연속함수 ${ f: X \to Y }$는 closed map.