## 정의

### dual order

[poset](https://paraconsistent.github.io/logic/2024/02/15/Poset.html) ${ (P,\le) }$에 대해, 다음과 같이 주어진 역순서 ${ \ge }$를 생각해보자

$$ x\ge y \mbox{ iff } y\le x  $$

그러면 ${ (P,\ge) }$ 또한 poset이 되고 이것을 ${ (P,\le) }$의 **dual**이라고 하고 ${ P^{\delta} }$로 표기한다.

### dual stament

statement ${ \Phi }$가 주어졌을 때, ${ \Phi }$에 등장하는 ${ \le }$를 모두 그것의 역순서 ${ \ge }$로 치환한 statement를 ${ \Phi^{\delta} }$로 표기하고 ${ \Phi }$의 **dual statement**라고 한다.

### duality priciple

주어진 statement ${ \Phi }$에 대해,

>${ \Phi }$가 모든 poset에 대해서 성립한다 iff ${ \Phi^{\delta} }$가 모든 poset에 대해서 성립한다.

모든 poset에 대해서 성립하려면, poset ${ P }$ 마다 ${ P^{\delta} }$ 또한 성립하여야 하므로 자명하다.

## Lattice version

### meet-join duality

lattice ${ (L,\wedge,\vee) }$ 다음 poset ${ (L,\le) }$과 동등하다

$$ a \le b \iff a \wedge b = a $$

그런데 absorption에 의해,

$$ a \vee b = (a \wedge b) \vee b = b  $$

따라서

$$ a \ge b \iff a\vee b = b$$

우리는 poset으로서 lattice ${ L= (L,\wedge,\vee) }$마다 다음과 같은 dual lattice를 대응할 수 있다.

$$ L^{\delta}=(L,\vee,\wedge) $$
### dual statement for lattice

statement ${ \Phi }$가 주어졌을 때, ${ \Phi }$에 등장하는 모든 meet ${ \wedge }$와 join ${ \wedge }$를 서로 맞바꾼 statement ${ \Phi^{\delta} }$를 ${ \Phi }$의 dual statement라고 한다.

### duality principle for lattices

주어진 statement ${ \Phi }$에 대해,

> ${ \Phi }$가 모든 lattice에 대해서 성립한다 iff ${ \Phi^{\delta} }$가 모든 lattice에 대해서 성립한다.

## 참고문헌

1. Grätzer (2011). *Lattice Theory: Foundation*, Birkhäuser.