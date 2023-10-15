---
layout: post
title: lifting property
category: Category Theory
tags:
  - lifting
  - algebraic-topology
  - homotopy
math: true
toc: true
---
## Formal definition
A pair of morphisms \\( (i,p) \\) has the **lifting property** iff there is a diagonal morphism h for each pair of morphisms \\( (f,g) \\) making the following diagram commutes.

<p align="middle"><iframe class="quiver-embed" src="https://q.uiver.app/#q=WzAsNCxbMCwwLCJBIl0sWzEsMSwiWSJdLFsxLDAsIlgiXSxbMCwxLCJCIl0sWzIsMSwicCJdLFswLDMsImkiLDJdLFswLDIsImYiXSxbMywxLCJnIiwyXSxbMywyLCJoIiwxLHsic3R5bGUiOnsiYm9keSI6eyJuYW1lIjoiZGFzaGVkIn19fV1d&embed" width="304" height="304" style="border-radius: 8px; border: none;"></iframe></p>

Then \( i \) has the left lifting property w.r.t. \( p \)and \( p \) has the right lifting property w.r.t. \( i \), denote those \( i \perp p \) or \( i \downarrow p \).

### Orthogonal with respect to a class

For a class ${ C }$ of morphisms in a category, the left orthogonal w.r.t. C is defined by

\\[ C^{\perp l} := \{ \, i \, \mid \, \forall p \in C, i\perp p \, \} \\]

and the right orthogonal w.r.t. \( C \)$ is defined by

\\[ C^{\perp r} := \{ \, i \, \mid \, \forall p \in C, i\perp p \, \} \\]

## homotopy lifting property

For any homotopy \\( f_{\bullet}:Y \times I \to B \\) and for any map \\( \tilde{f}_{0} : Y \to E\\) lifting \\( f_{0} = f_{\bullet} \rvert_{Y \times\left\{ 0 \right\}} \\), there exists a homotopy \\( \tilde{f}_{\bullet} : Y \times I \to E \\) lifting \\( f_{\bullet} \\)

<p align="middle"><iframe class="quiver-embed" src="https://q.uiver.app/#q=WzAsNCxbMCwwLCJZIl0sWzAsMSwiWSBcXHRpbWVzIEkiXSxbMSwxLCJCIl0sWzEsMCwiRSJdLFswLDEsIlxcaW90YV8wIiwyLHsic3R5bGUiOnsidGFpbCI6eyJuYW1lIjoiaG9vayIsInNpZGUiOiJ0b3AifX19XSxbMSwyLCJmX3tcXGJ1bGxldH0iLDJdLFszLDIsIlxccGkiLDAseyJzdHlsZSI6eyJoZWFkIjp7Im5hbWUiOiJlcGkifX19XSxbMCwzLCJcXH5mX3swfSJdLFsxLDMsIlxcfmZfe1xcYnVsbGV0fSIsMSx7InN0eWxlIjp7ImJvZHkiOnsibmFtZSI6ImRhc2hlZCJ9fX1dXQ==&embed" width="320" height="304" style="border-radius: 8px; border: none;"></iframe></p>

