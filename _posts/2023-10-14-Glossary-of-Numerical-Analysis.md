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

## Rounding

Rounding means replaceing a number with an approximate value that has a shorter, simpler, or more explicit representation.

### Rounding to a specified multiple

Rounding a number ${ x }$ to a multiple of some specified positive value ${ m }$

$$ \mathrm{roundToMultiple}(x,m) = \mathrm{round}\left( \frac{x}{m} \right) \times m $$

### Logarithmic rounding


---
# References

1. [ISO 5725-1:2023(en), Accuracy (trueness and precision) of measurement methods and results — Part 1: General principles and definitions](https://www.iso.org/obp/ui/#iso:std:iso:5725:-1:ed-2:v1:en)