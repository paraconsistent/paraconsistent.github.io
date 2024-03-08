---
layout: post
math: "true"
toc: "true"
title: Stereographic Projection
categories: Geometry
tags:
  - projection
---
![Stereographic Projection](https://raw.githubusercontent.com/paraconsistent/paraconsistent.github.io/master/_posts/calc/stereographic/stereographic.png)

## Stereogrphic Projection

Let

$$ \begin{dcases}\mathbf{x}=(x_{1},\dots,x_{n},0) \in \mathbb{R}^{n+1} \\ \mathbf{N}=(0,\dots,0,1) \in \mathbb{S}^{n} \subset \mathbb{R}^{n+1} \end{dcases} $$

Then

$$ \begin{eqnarray} \mathbf{u} &=& t\mathbf{x}+(1-t)\mathbf{N} \\ \Rightarrow 1&=& t^{2}\lVert \mathbf{x} \rVert^{2} +1-2t+t^{2}\\ \Rightarrow 0&=& ((1+\lVert \mathbf{x} \rVert^{2})t-2)t \\ &\therefore& t= \frac{2}{\lVert \mathbf{x} \rVert^{2}+1} \end{eqnarray} $$

and

$$ \therefore \mathbf{u}=\left( \frac{2\mathbf{x}}{\lVert \mathbf{x} \rVert^{2}+1} , \frac{\lVert \mathbf{x} \rVert^{2}-1}{\lVert \mathbf{x} \rVert^{2}+1} \right) $$

## Inverse of Stereogrphic Projection

Let

$$ \begin{dcases} \mathbf{N}=(0,\dots,0,1) \in  \mathbb{S}^{n} \subset \mathbb{R}^{n+1} \\ \mathbf{u}=(u_{0},\dots,u_{n}) \in \mathbb{S}^{n}\setminus\mathbf{N} \end{dcases} $$

Then

$$\begin{eqnarray} \mathbf{x} &=& t\mathbf{u}+(1-t)\mathbf{N} \\ &=& (tu_{0}, \dots,tu_{n-1},1+t(u_{n}-1)) \\ \Rightarrow 0 &=& 1+t(u_{n}-1) \\ \Rightarrow t &=& \frac{1}{1-u_{n}} \end{eqnarray}$$

and

$$ \mathbf{x} = \left( \frac{\mathbf{u}}{1-u_{n}}, 0 \right)$$

## South Pole Version

Let

$$ \begin{dcases}\mathbf{x}=(x_{1},\dots,x_{n},0) \in \mathbb{R}^{n+1} \\ \mathbf{S}=(0,\dots,0,-1) \in \mathbb{S}^{n} \subset \mathbb{R}^{n+1} \end{dcases} $$

Then

$$ \begin{eqnarray} \mathbf{u} &=& t\mathbf{x}+(1-t)\mathbf{S} \\ \Rightarrow 1&=& t^{2}\lVert \mathbf{x} \rVert^{2} +1-2t+t^{2}\\ \Rightarrow 0&=& ((1+\lVert \mathbf{x} \rVert^{2})t-2)t \\ &\therefore& t= \frac{2}{\lVert \mathbf{x} \rVert^{2}+1} \end{eqnarray} $$

$$ \therefore \mathbf{u}=\left( \frac{2\mathbf{x}}{\lVert \mathbf{x} \rVert^{2}+1} , \frac{1-\lVert \mathbf{x} \rVert^{2}}{\lVert \mathbf{x} \rVert^{2}+1} \right) $$

and its inversion is derived by

$$\begin{eqnarray} \mathbf{x} &=& t\mathbf{u}+(1-t)\mathbf{S} \\ &=& (tu_{0}, \dots,tu_{n-1},t(u_{n}+1)-1) \\ \Rightarrow 0 &=& t(u_{n}+1)-1 \\ \Rightarrow t &=& \frac{1}{1+u_{n}} \end{eqnarray}$$

$$ \therefore \mathbf{x} = \left( \frac{\mathbf{u}}{1+u_{n}}, 0 \right)$$