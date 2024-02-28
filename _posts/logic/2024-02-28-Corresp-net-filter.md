---
layout: post
math: "true"
toc: "true"
title: Net과 Filter의 대응성
categories: Logic
tags:
  - net
  - filter
---
## 정의

### Eventuality filter

[net의 tail](https://paraconsistent.github.io/logic/2024/02/26/net.html#tail)을 정의할 때 우리는 다음 모임 또한 정의했다.

$$ \mathrm{Tails}((x_{\alpha})_{\alpha \in J})=\{ x_{\ge\beta} : \beta \in J\} $$

이 모임은 [filter base](https://paraconsistent.github.io/logic/2024/02/28/filter-base.html#filter-base)이고 이것이 생성하는 filter를  ${ (x\_{\alpha})\_{\alpha \in J} }$의 **eventuality filter**라고 한다.

**Exercise**. 주어진 ${ \mathrm{Tails}(x\_{\bullet}) }$이 filter base임을 증명하라.

Hint: ${ \alpha \le \beta \Rightarrow x_{\ge \beta} \subseteq x_{\ge \alpha} }$

## 참고문헌

1. Eric Schechter (1996). *Handbook of Analysis and Its Foundations*, Academic Press.