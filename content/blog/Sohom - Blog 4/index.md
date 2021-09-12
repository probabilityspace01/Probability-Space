---
author: Soham Ghosh
#categories:
#- Theme Features
date: "2021-09-08"
draft: false
excerpt:
title: Some Classical Problems and Paradoxes in Geometric Probability
---

> *"Geometry is not true, it is advantageous."* - **Henri Poincare**

Yes , exactly... it's time to merge the two stalwarts together : *"Geometry"* and *"Probability"*.

### The Probability Measure of Geometrical Elements

In probability theory one is usually concerned with random variables which are quantities, or sets of quantities, taking values in some set of possibilities on which there is defined a non-negative measure, satisfying certain required conditions which enable us to interpret it as a probability. In the theory of geometrical probabilities the random elements are not quantities but geometrical objects such as points, lines and rotations. Since the ascription of a measure to such elements is not quite an obvious procedure, a number of "paradoxes" can be produced by failure to distinguish the reference set. These are all based on a simple confusion of ideas but may be useful in illustrating the way in which geometric probabilities should be defined.

### Bertrand's Paradox

We consider one paradox due to **J.Bertrand (1907)**.

The problem of interest is precisely : 

> *Determine the probability that a random chord of a circle of unit radius has a length greater than the square root of 3, the side of an inscribed equilateral triangle*.

### Context of the Problem

The development of the Theory of Probability has not been smooth at all. The first attempts to formalize the calculus of probability were due to Marquis De Laplace (1749-1827) who proposed to define the probability \\(\mathbb{P}(A)\\)

## Rendering mathematical equations

Examples from the [mathjax demo](https://www.mathjax.org/#demo).
But they work with `katex` as well.

### Rmarkdown

In `.Rmarkdown` documents, you can use either

```
$a \ne 0$
```

to get inline math: `\(a \ne 0\)`.
There is no conflict with using dollar symbols regularly, because `knitr` automatically escapes freestanding dollar symbols.

And you can use

```
$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$
```

to get a math paragraph:

$$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$

### md

In `.md` documents, you can **not** use the single dollar syntax.
The double dollar syntax still gives you a math paragraph.

```
$$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$
```

$$x = {-b \pm \sqrt{b^2-4ac} \over 2a}$$

In order to get inline equations, use:

```
`\(a \ne 0\)`
or
\\(a \ne 0\\)
```

to get: `\(a \ne 0\)`.



