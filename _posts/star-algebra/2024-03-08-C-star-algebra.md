---
layout: post
math: "true"
toc: "true"
title: C-star-algebra
categories: Functional-Analysis
tags:
  - star-algebra
---
## 정의

### Complex ${ \ast }$-algebra

${ (A,+,\cdot,\ast) }$가 [associative complex algebra](https://paraconsistent.github.io/algebra/2024/03/08/associative-algebra.html)이면 [${ \ast }$-algebra](https://paraconsistent.github.io/functional-analysis/2024/02/09/star-algebra.html) 구조는 다음과 같이 자연스럽게 주어진다.

$$ \begin{gather} \mbox{(i)} & a^{\ast\ast}=a \\ \mbox{(ii)} & (a+b)^{\ast}=a^{\ast}+b^{\ast} \\ \mbox{(iii)} & (\lambda a)^{\ast}=\overline{\lambda} a^{\ast} \\ \mbox{(iv)} & (ab)^{\ast}=b^{\ast}a^{\ast} \end{gather} $$

### Abstract ${ C^{\ast} }$-algebra (${ B^{\ast} }$-algebra)

complex ${ \ast }$-algebra ${ (A,+,\cdot,\ast )}$가 norm ${ \lVert \cdot \rVert }$의 Banach algebra라고 하자. 이때 임의의 ${ a \in A }$에 대해,

$$ \lVert a^{\ast} \rVert = \lVert a \rVert $$

를 만족하면 **involutive Banach algebra**라고 한다.

involutive Banach algebra 중

$$ (C^{\ast}\mbox{-identity}) \quad \lVert a^{\ast}a \rVert= \lVert a \rVert^{2}$$

를 만족시키면 **(abstract) ${ C^{\ast} }$-algebra**라고 한다.

**Remark** Banach algebra가 ${ C^{\ast}}$-identity를 만족시키면 involutive Banach algebra가 된다. ${ a \neq 0 }$에 대해,

$$ \begin{gather} \lVert a \rVert^{2}=\lVert a^{\ast}a \rVert \le \lVert a^{\ast} \rVert \lVert a \rVert \\ \lVert a^{\ast} \rVert^{2}=\lVert a^{\ast\ast}a^{\ast} \rVert \le \lVert a^{\ast\ast} \rVert \lVert a^{\ast} \rVert\end{gather} $$

이므로 ${ \lVert a^{\ast} \rVert = \lVert a \rVert }$.

### Concrete ${ C^{\ast} }$-algebra

complex Hilbert space ${ \mathcal{H} }$가 주어졌을 때 ${ B(\mathcal{H}) }$의 ${ \ast }$-subalgebra 중 closed인 것을 **concrete ${ C^{\ast} }$-algebra**라고 한다.

## 여담

### 이름의 유래

본래 ${ C^{\ast} }$-algebra는 concrete ${ C^{\ast} }$-algebra를 의미하였고 C는 closed에서 따왔다. 나아가 abstract ${ C^{\ast} }$-algebra는 본래 ${ B^{\ast} }$-algebra로 불리었고 B는 Banach에서 따왔다. 하지만 근래에는 ${ C^{\ast} }$-algebra를 주로 abstract 의미로 많이 해석하여 ${ B^{\ast} }$-algebra는 잘 쓰이지 않게 되었다.

### 컴퓨터에서 표기

많은 시스템과 응용 프로그램에서 ${ \ast }$를 [와일드카드 문자](https://ko.wikipedia.org/wiki/%EC%99%80%EC%9D%BC%EB%93%9C%EC%B9%B4%EB%93%9C_%EB%AC%B8%EC%9E%90)로 사용하므로 문서 제목에는 C-star-algebra로 우회하는 것이 권장된다.

시스템에 따라 `Shift+8` 문자가 다르게 출력될 수 있으므로 TeX 문서에서 ${ \ast }$는 `\ast`로 쓰는 것이 권장된다.

## 참고문헌

1. [J. Hamhalter (2003). *Quantum Measure Theory*, Springer Dordrecht, p.12](https://link.springer.com/book/10.1007/978-94-017-0119-8)
1. [J. B. Conway (2007). *A Course in Functional Analysis*, 2nd ed., Springer New York, NY, p.232.](https://link.springer.com/book/10.1007/978-1-4757-4383-8)
1. W. Rudin (2005). *Functional Analysis*, International ed., McGraw-Hill, p.288.
1. [C-star-algebra in nLab (ncatlab.org)](https://ncatlab.org/nlab/show/C-star-algebra)