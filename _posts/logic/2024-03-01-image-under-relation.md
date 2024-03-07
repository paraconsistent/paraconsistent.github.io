---
layout: post
math: "true"
toc: "true"
title: binary relation의 image의 성질
categories: Logic
tags:
  - relation
---
## 성질

${ R }$이 ${ A }$ 위의 binary relation이라고 하자.

### Monotonicity

${ C \subseteq B\subseteq A }$에 대해,

$$ R[C] \subseteq R[B] $$

증명

${ c \in C \Rightarrow c \in B}$이므로,

$$ d \in R[C] \Leftrightarrow \exists c \in C,\,cRd \Rightarrow \exists c \in B,\, cRd  \Leftrightarrow d \in R[B] $$

### Intersection

${ B,C \subseteq A }$에 대해,

$$ R[B \cap C] \subseteq R[B] \cap R[C] $$

등호는 ${ R }$이 [injective](https://paraconsistent.github.io/logic/2024/02/26/relation.html#inj)일 때 성립한다.

증명

monotonicity에 의해,

${ R[B\cap C] \subseteq R[B] }$ 이고 ${ R[B \cap C] \subseteq R[C]}$. 따라서,

$$ R[B\cap C] \subseteq R[B] \cap R[C] $$

반대로,

${ y \in R[B] \cap R[C] }$라는 것은 적당한 ${ b \in B }$와 ${ c \in C }$가 존재하여,

$$ bRy \mbox{ and } cRy $$

라는 것이다. ${ R }$이 injective이면,

$$ bRy \mbox{ and } cRy \Rightarrow b=c $$

이므로 ${ b=c \in B \cap C  }$이므로

$$ y \in R[B \cap C] $$

따라서

$$ R[B] \cap R[C] \subseteq R[B \cap C] $$

### Union

${ (B\_{\alpha}: \alpha \in J) \subseteq \mathcal{P}(A)  }$에 대해,

$$ R[\bigcup_{\alpha \in J} B_{\alpha}] = \bigcup_{\alpha \in J} R[B_{\alpha}]  $$

증명

임의의 ${ \beta \in J }$에 대해,

$$ B_{\beta} \subseteq \bigcup_{\alpha \in J} B_{\alpha} $$

이므로 monotonicity에 의해,

$$ R[B_{\beta}] \subseteq R[\bigcup_{\alpha \in J}B_{\alpha}] $$

따라서

$$ \bigcup_{\alpha \in J} R[B_{\alpha}] \subseteq R[\bigcup_{\alpha \in J} B_{\alpha}] $$

반대로,

$$ y \in R[\bigcup_{\alpha \in J} B_{\alpha}] \Rightarrow \exists x \in \bigcup_{\alpha \in J } B_{\alpha},\, xRy$$

그런데

$$ x \in \bigcup_{\alpha \in J} B_{\alpha} \Leftrightarrow x \in B_{\beta} \mbox{ for some } \beta \in J$$

이므로 ${ y \in R[B_{\beta}] }$. 따라서

$$ R[\bigcup_{\alpha \in J}B_{\alpha}] \subseteq \bigcup_{\alpha \in J} R[B_{\alpha}] $$

### Difference

${ B,C \subseteq A }$에 대해

$$ R[B-C] \supseteq R[B] - R[C] $$

이고 등호는 ${ R }$이 [injective](https://paraconsistent.github.io/logic/2024/02/26/relation.html#inj)일 때 성립한다.

증명

$$ B = (B-C) \cup (B \cap C) \subseteq (B-C) \cup C$$

이므로 monotinicity에 의해

$$ R[B]\subseteq R[B-C] \cup R[C] $$

따라서 양변에 ${ R[C] }$를 빼주면,

$$ R[B]-R[C] \subseteq R[B-C] - R[C] \subseteq R[B-C]  $$

만약 ${ R }$이 injective이면,

$$ y \in R[B]-R[C] \Leftrightarrow y \in R[B] \mbox{ and } y \notin R[C] $$

${ xRy }$라고 하면, injective이므로

$$ x \in B \mbox{ and } x \notin C \Leftrightarrow x \in B-C $$

따라서

$$y \in R[B]-R[C] \Rightarrow y \in R[B-C] $$

따라서

$$ R[B] - R[C] \subseteq R[B-C] $$