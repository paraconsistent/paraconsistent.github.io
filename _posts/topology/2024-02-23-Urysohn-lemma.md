---
layout: post
math: "true"
toc: "true"
title: 우리손 보조정리
categories: General-Topology
---
## Lemma

${ X }$가 정규공간이고 ${ A,B }$가 ${ X }$의 닫힌 부분집합이라고 하자. 그러면 실수 폐구간 ${ [a,b] }$에 대해서 적당한 연속함수 ${ f: X \to [a,b]  }$가 존재하여,
- ${ f \rvert_{A}= a }$
- ${ f\rvert_{B} = b }$

를 만족한다.

### proof

${ f: X \to [0,1] }$에 대해서 보이면 충분하다. 왜냐하면, ${ a=b }$일 때는 상수함수 ${ f(x)=a }$가 조건을 만족하고, ${ a<b }$ 이면,

$$ \varphi(x) = \frac{x-a}{b-a},\quad \varphi \circ f : X \to [0,1] $$

이므로 충분하다.


#### Step 1

${ P = \mathbb{Q}\cap [0,1] }$이라고 하자. 가산집합이므로

$$ P=\{ r_{1},r_{2},r_{3}, \dots \} $$

으로 자연수 집합과 일대일 대응할 수 있다.

${ U_{1} = X-B}$로  두면,

$$ A \subset U_{1} $$

이므로 정규공간의 성질에 의해 다음을 만족하는 열린집합 ${ U_{0} }$가 존재한다.

$$ A \subset U_{0} \subset \overline{U}_{0} \subset U_{1} $$

${ P_{n}=\{ r\_{1},r\_{2},\dots,r\_{n} \} }$이라 하고 귀납가정

$$ r_{i} \le r_{j} \Rightarrow \overline{U}_{r_{i}} \subset  U_{r_{j}} $$

을 세우자. 그러면 ${ r_{n+1} }$은 ${ P }$에서 immediate predecessor ${ p }$와 immediate successor ${ q }$를 갖는다. (${ i<j \nRightarrow r_{i} < r_{j} }$임에 유의하라)

귀납가정에 의해, ${ \overline {U}_{p} \subset U_{q}  }$이므로 정규공간의 성질에 의해,

$$ \overline{U}_{p} \subset U_{r_{n+1}} \subset \overline{U}_{r_{n+1}} \subset U_{q}  $$

를 만족하는 열린집합 ${U_{n+1}  }$이 존재한다.

이제 ${ P_{n+1} }$이 우리가 원하는 성질

$$ r_{i} < r_{j} \Rightarrow \overline{U}_{r_{i}} \subset U_{r_{j}} $$

를 만족시킴을 보이자.

만약 ${ r_{i},r_{j} }$ 모두 ${ P_{n} }$의 원소인 경우 귀납가정에 의해 참이다. 따라서 ${ r_{n+1} }$과 ${ s \in P_{n} }$에 대해서만 보이면 된다. ${ p,q }$가 각각 immediate precessor, immediate successor이므로, ${ s\le p }$이거나 ${ s \ge q }$이다.

${ s \le p }$인 경우,

$$ \overline{U}_{s} \subset U_{p} \subset \overline{U}_{p} \subset U_{r_{n+1}} \Rightarrow \overline{U}_{s} \subset U_{r_{n+1}} $$

${ s \ge q }$인 경우,

$$ \overline{U}_{r_{n+1}} \subset U_{q} \subset \overline{U}_{q} \subset U_{s} \Rightarrow \overline{U}_{r_{n+1}} \subset U_{s}$$

따라서 임의의 ${ n\in \mathbb{N} }$에 대해서 성질이 만족하기 때문에 ${ P }$는 다음 성질을 만족한다.

$$ r<s \Rightarrow \overline{U}_{p} \subset U_{q} $$

#### Step 2

Step 1에서 ${ [0,1] }$에 존재하는 임의의 유리수 ${ r }$에 대해서 ${ U_{r} }$을 정의했다. 이제,

$$ \begin{dcases} U_{p}=\emptyset, & p<0\\ U_{p} = X, & p>1 \end{dcases} $$

로 정의하면, 모든 유리수 ${ r,s }$에 대해서 다음이 성립함을 알 수 있다.

$$ r<s \Rightarrow \overline{U}_{r} \subset U_{s} $$

#### Step 3

주어진 ${ x \in X }$에 대해서,

$$ \mathbb{Q}(x) = \{ r : x \in U_{r} \} $$

로 정의하면, Step 2에 따라 이 집합은 0 보다 작은 수는 포함하지 않고 1 보다 큰 모든 수를 포함함을 알 수 있다. 따라서 ${ \mathbb{Q}(x) }$는 아래로 유계이다. 따라서 실수의 최대 하계 성질에 의해,

$$ f(x) = \inf \mathbb{Q}(x) $$

는 ${ [0,1] }$에서 값을 가지는 함수로 잘 정의된다.

#### Step 4

이제 Step 3에서 정의한 ${ f }$가 우리가 원하는 함수임을 보이자. 만약 ${ x \in A }$이면 ${ A \subset U_{1} }$이었으므로, 모든 ${ r\ge 0 }$에 대해 ${ x \in U_{r} }$이다. 따라서

$$ \mathbb{Q}(x) = \mathbb{Q} \cap [0, \infty) $$
이므로 ${ f(x) = 0 }$.

같은 방식으로, ${ x \in B }$ 이면 ${ B \subset X\setminus U_{1} }$ 이므로

$$ \mathbb{Q}(x) = \mathbb{Q} \cap (1, \infty) $$

따라서 ${ f(x) = 1 }$.

마지막으로 ${ f }$가 연속임을 보이자.

우선 다음 두 성질을 증명하자.

$$ \begin{eqnarray} x \in \overline{U}_{r} &\Rightarrow& f(x) \le r \\ x \notin U_{r} &\Rightarrow& f(x) \ge r  \end{eqnarray} $$

${ x \in \overline{U}_{r} }$이면 임의의 ${ s>r }$에 대해, ${x \in U\_{s}  }$. 따라서 

$$ s>r \Rightarrow s \in \mathbb{Q}(x) $$

이므로 ${ f(x) \le r }$.

마찬가지로, ${ x \notin U_{r} }$이면 임의의 ${ s<r }$에 대해서 ${ x \notin U\_{s} }$. 따라서

 $$ s< r => s \notin \mathbb{Q}(x) $$

 이므로 ${ f(x) \ge r }$.

 이제 ${ f }$의 연속성을 증명해보자.

 점 ${ x_{0}\in X}$를 고정하고, ${ f(x\_{0}) }$를 포함하는 개구간 ${ (c,d) }$에 대해,

 $$ f(U) \subset (c,d) $$

 를 만족하는 ${ x_{0} }$의 열린근방 ${ U }$를 찾자.

 $$ c<p<f(x_{0})<q<d $$
 를 만족하는 유리수쌍 ${ p,q }$를 뽑으면

 $$ x_{0} \in U=U_{q}-\overline{U}_{p} $$

 이고

 $$ \begin{eqnarray} x\in U_{q} &\Rightarrow& f(x) \le q <d \\ x\notin \overline{U}_{q} &\Rightarrow& f(x) \ge p > c \end{eqnarray} $$

 이므로

 $$ f(U) \subset [p,q] \subset (c,d) $$

 따라서 ${ f }$는 연속이다.

## References

1. Munkres. *Topology*, 2nd International ed. 207-210p.