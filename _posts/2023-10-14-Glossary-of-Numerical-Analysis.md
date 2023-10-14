---
layout: post
title: Glossary of Numerical Analysis
category: Numerical Analysis
tags:
  - precision
  - accuracy
  - significant-figure
  - rounding
math: true
toc: true
---
## Accuracy and precision

### ISO 5725

#### test result
value of a characteristic obtained by carrying out a specified test method

#### accuracy
closeness of agreement between a test result and the true value

#### precision
closeness of agreement between independent test results obtained under stipulated conditions

#### trueness
closeness of agreement between the expectation of test results and a true value

#### bias
difference between the expectation of the test results and a true value

## Floating-Point Arithmetic

### IEEE 754

#### floating formats
- a base(or radix) b, which is either 2 (binary) or 10 (decimal);
- a precision p;
- an exponent range from *emin* to *emax*, with ${ \mathrm{emin} = 1 - \mathrm{emax} }$

A format comprises
- Finite numbers: ${ (-1)^{s}\times c \times b^{q} }$, where a sign ${ s }$, a significand (or coefficient) ${ c }$, an exponent ${ q }$ s.t. ${ \mathrm{emin} \le q + p -1 \le \mathrm{emax} }$
- Two infinities: ${ +\infty }$ and ${ -\infty }$
- Two kinds of NaN: a quiet NaN (qNaN) and a signaling NaN (sNaN)

#### Basic and interchange formats

| Name       | Common name         | Radix (${ b }$) | Digits | Exponent                       | note        |
| ---------- | ------------------- | --------------- | ------ | ------------------------------ | ----------- |
| binary16   | Half precision      | 2               | 11     | ${ -14 \le q \le 15 }$         | Interchange |
| binary32   | Single precision    | 2               | 24     | ${ -126\le q \le 127 }$        | Basic       |
| binary64   | Double precision    | 2               | 53     | ${ -1022 \le q \le 1023 }$     | Basic       |
| binary128  | Quadruple precision | 2               | 113    | ${ -16382 \le q \le 16383 }$   | Basic       |
| binary256  | Octuple precision   | 2               | 237    | ${ -262142 \le q \le 262143 }$ | Interchange |
| decimal32  |                     | 10              | 7      | ${ -95 \le q \le 96 }$         | Interchange |
| decimal64  |                     | 10              | 16     | ${ -191 \le q \le 192 }$       | Basic       |
| decimal128 |                     | 10              | 34     | ${ -6143 \le q \le 6144}$      | Basic       |



---
# References

1. [ISO 5725-1:2023(en), Accuracy (trueness and precision) of measurement methods and results — Part 1: General principles and definitions](https://www.iso.org/obp/ui/#iso:std:iso:5725:-1:ed-2:v1:en)