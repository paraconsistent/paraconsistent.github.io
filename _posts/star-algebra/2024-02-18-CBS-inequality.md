---
layout: post
math: "true"
toc: "true"
title: Cauchy-Schwarz inequality
categories: Calculus
tags:
  - inequality
---
## Statement

Let ${ (X,\langle \cdot,\cdot \rangle) }$ be a inner product space. Then,

$$ \lvert \langle x,y \rangle \rvert \le \lVert x \rVert  \lVert y \rVert$$
and the equality holds iff ${ \alpha x + \beta y = \mathbf{0} }$ for some scalars ${ \alpha,\beta }$ s.t. ${ \alpha \beta \neq 0 }$.

The inequality called Cauchy-Schwarz inequality or Cauchy-Bunyakovsky-Schwarz (CBS) inequality

### proof

If ${ y=\mathbf{0} }$,

$$ \lvert \langle x,0 \rangle \rvert = \lVert x \rVert \lVert \mathbf{0} \rVert $$
Suppose ${ y \neq \mathbf{0} }$, and let

$$ z = x - \frac{\langle x,y \rangle}{\langle y,y \rangle}y $$

Then,

$$ \langle z,y \rangle = \langle x,y \rangle - \langle x,y \rangle = 0$$

Therefore ${ z \perp y }$ and

$$ x= \frac{\langle x,y \rangle}{\langle y,y \rangle }y + z $$

which gives

$$ \lVert x \rVert^{2} = \left\lvert \frac{\langle x,y \rangle}{\langle y,y \rangle}\right\rvert^{2}\lVert y\rVert^{2} + \lVert z \rVert^{2} = \frac{\lvert \langle x,y \rangle\rvert^{2}}{\lVert y \rVert^{2}} + \lVert z \rVert^{2} \ge \frac{\lvert \langle x,y \rangle\rvert^{2}}{\lVert y \rVert^{2}} $$

Therefore,

$$ \lVert x \rVert^{2} \lVert y \rVert^{2} \ge \lvert\langle x,y \rangle\rvert^{2}  $$

The equality holds iff ${ z = \mathbf{0} }$ i.e.,

$$ \langle y,y \rangle x-\langle x,y \rangle y =0 $$
