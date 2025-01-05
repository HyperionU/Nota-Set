---
marp: true
theme: uncover
class: invert
math: mathjax
style: |
  .columns {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1rem;
  }
---

# <!--fit--> Pre-Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2024-->

---

<!--paginate: true-->

# Lesson 3: Rational Functions and Transformations

---

## Rationals

A **Rational Function** is a function that can be represented as a fraction of polynomials. ($y = \frac{P(x)}{Q(x)}$)

Examples include:
* $y = \frac{3}{x}$ 
* $f(x) = \frac{4x^2 + 5}{x - 5}$ 
* $y = 5$ 
* $C(n) = \frac{100 + 2n}{n}$

---

## Basis Functions

![bg invert](https://s3-us-west-2.amazonaws.com/courses-images/wp-content/uploads/sites/896/2016/11/02213907/CNX_Precalc_Figure_03_07_0012.jpg)

There are two basis functions.

* $y = \frac{1}{x}$
* $y = \frac{1}{x^2}$

Common Characteristics of basis:
* Restriction: $x \neq 0$
* Domain: $x \neq 0$
* Range: $y \neq 0$
* Asymptotes: $x, y = 0$

---

## Transformations

Here's our toolkit:

$$
  y = \frac{a}{x - h} + k \text{ or }
  y = \frac{a}{(x - h)^2} + k
$$

* $a$: Vertical Stretch
* $h$: Horizontal Translation (x-coordinate of central point)
* $k$: Vertical Translation (y-coordinate of central point)

---

## Graphing Transformations

* Note the basis
* Note the central point.

Try sketching a graph of these:
1. $y = \frac{4}{x - 2} - 3$
2. $y = \frac{-2}{(x + 1)^2} + 4$

---

## Example 1

1. $y = \frac{4}{x - 2} - 3$

* Basis: $\frac{1}{x}$
* Central Point: $(2, -3)$
* Restriction: $x \neq 2$
* Behaviour near Restriction
  * Left: $y \to -\infty$
  * Right: $y \to -\infty$
* End Behaviour: $x \to \pm \infty, y \to -3$
* Asymptotes: $x = 2, y = -3$

---

## Example 2

2. $y = \frac{-2}{(x + 1)^2} + 4$

* Basis: $\frac{1}{x^2}$
* Central Point: $(-1, 4)$
* Restriction: $x \neq -1$
* Behaviour near Restriction: $y \to -\infty$
* End Behaviour: $y \to 4$
* Asymptotes: $x = -1, y = 4$

---

## Determining Equations

1. Note the basis
2. Determine the Central Point 
3. Determine $a$
  * Pick a point on the function
  * Plug in values.

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%204%20(Discontinuities).html)

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">