---
marp: true
theme: uncover
class: invert
math: mathjax
---

$\newcommand\diff[1][]{\mathcal{d}_{#1}}$
$\newcommand\dd[2][]{\displaystyle\frac{d#1}{d#2}}$

# <!--fit--> Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2025-->

$\newcommand\limit[2]{\displaystyle\lim_{#1 \to #2}}$

---

# Lesson 7: Implicit Differentiation

---

<!--paginate: true-->

## Intro

* Previously, we focused on simple derivatives: derivatives of functions such that $y = f(x)$.
* However, this may not always be the case. We may not strictly have one input and output.
* We may have interdependent values related by some equation. These form what are called 'implicit curves', and differentiating these is called 'implicit differentiation'.
* Here, let's look at an example:

---

## Example

* Consider this implicit curve: $2y = y^2 + 3x^3$
* This 'elliptic curve' is not a function. We can't easily isolate $y$.
* So, let's try a different technique:
    * $\diff (2y) = \diff (y^2 + 3x^3)$
    * $\diff (2y) = \diff (y^2) + \diff (3x^3)$
    * $2 dy = (2y)dy + 9x^2 dx$
    * $2 dy - (2y)dy = 9x^2 dx$

---

## Example, cont.

* $dy(2 - 2y) = 9x^2 dx$
* $\dd[y]{x} = \frac{9x^2}{2 - 2y}$
* And, that's our derivative for this implicit curve.
* This might not make much sense, but it works great when it comes to Applications of Differentiation (which we'll talk about in Unit 6).
* Let's look at more examples.

---

## Example 1

1. Differentiate $x^2 + y^2 = 15$
    * $\diff (x^2) + \diff (y^2) = \diff (15)$
    * $(2x)dx + (2y)dy = 0$
    * $(2y)dy = -(2x)dx$
    * $\dd[y]{x} = \frac{-2x}{2y}$
    * $\dd[y]{x} = \frac{-x}{y}$

---

## Example 2

2. Differentiate $3xy - 2y^2 = 5x$
    * $(3x)y - 2y^2 = 5x$
    * $\diff (3xy) - \diff (2y^2) = \diff (5x)$
    * $[3x (\diff (y)) + y (\diff (3x))] - \diff (2y^2) = \diff (5x)$
    * $[(3x)dy + y(3)dx] - 2(2y)dy = (5)dx$
    * $(3x)dy + (3y)dx - (4y)dy = (5)dx$
    * $(3x)dy - (4y)dy = (5)dx - (3y)dx$
    * $dy(3x - 4y) = dx(5 - 3y)$
    * $\dd[y]{x} = \frac{5 - 3y}{3x - 4y}$

---

## Example 3

3. Differentiate $2xy - 15 = -3x^2$ to find the slope at $P(1, 6)$
    * $(2x)y - 15 = -3x^2$
    * $\diff (2xy) - \diff (15) = \diff (-3x^2)$
    * $[2x \diff (y) + y \diff (2x)] - \diff (15) = \diff (-3x^2)$
    * $(2x)dy + y(2dx) = (-6x)dx$
    * $(2x)dy + (2y)dx = (-6x)dx$
    * $(2x)dy = (-6x)dx - (2y)dx$
    * $(2x)dy = dx(- 6x - 2y)$

---

## Example 3, cont.

3. Differentiate $2xy - 15 = -3x^2$ to find the slope at $P(1, 6)$
    * $(2x)dy = dx(- 6x - 2y)$
    * $\dd[y]{x} = -\frac{6x + 2y}{2x}$
    * $\dd[y]{x}_P = -\frac{6(1) + 2(6)}{2(1)}$
    * $\dd[y]{x}_P = -\frac{6 + 12}{2}$

---

## Example 3, cont.

3. Differentiate $2xy - 15 = -3x^2$ to find the slope at $P(1, 6)$
    * $\dd[y]{x}_P = -\frac{6 + 12}{2}$
    * $\dd[y]{x}_P = -\frac{18}{2}$
    * $\dd[y]{x}_P = -9$

---

## Exercises for Readers

* Differentiate the following:
    * $4x^2 + 4y^2 = 20$
    * $4xy^2 + 2y = 3x$
    * $3y - \frac{y^4}{x^2} = 2y$

---

# [Next Unit](../Trancendentals/Lesson%201)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Differentiate the following: $4x^2 + 4y^2 = 20$
    * $\diff (4x^2) + \diff (4y^2) = \diff (20)$
    * $2(4x)dx + 2(4y)dy = 0$
    * $(8x)dx + (8y)dy = 0$
    * $(8y)dy = -(8x)dx$
    * $\dd[y]{x} = \frac{-8x}{8y}$
    * $\dd[y]{x} = \frac{-x}{y}$

---

## Answers to Exercises, cont.

* Differentiate the following: $4xy^2 + 2y = 3x$
    * $\diff (4xy^2) + \diff (2y) = \diff (3x)$
    * $[4x \diff (y^2) + y^2 \diff (4x)] + \diff (2y) = \diff (3x)$
    * $4x(2y)dy + y^2(4)dx + (2)dy = (3)dx$
    * $(8xy)dy + (4y^2)dx + (2)dy = (3)dx$
    * $(8xy)dy + (2)dy = (3)dx - (4y^2)dx$
    * $dy(8xy + 2) = dx(3 - 4y^2)$
    * $\dd[y]{x} = \frac{3 - 4y^2}{8xy + 2}$

---

## Answers to Exercises, cont.

* Differentiate the following: $3y - \frac{y^4}{x^2} = 2y$
    * $\diff (3y) - \diff (\frac{y^4}{x^2}) = \diff (2y)$
    * $u = y^4$
    * $v = x^2$
    $\diff f(x) = \frac{v (\diff u) - u (\diff v)}{v^2}$
    * $\diff (3y) - \frac{(x^2) \diff (y^4) - (y^4) \diff (x^2)}{(x^2)^2} = \diff (2y)$
    * $(3y)dy - \frac{(x^2) 4(y^3)dy - (y^4) 2(x)dx}{(x^2)^2} = (2)dy$
    * $-\frac{(4x^2 y^3)dy - (2xy^4)dx}{(x^4)} = (2)dy - (3y)dy$

---

## Answers to Exercises, cont.

* Differentiate the following: $3y - \frac{y^4}{x^2} = 2y$
    * $-\frac{(4x^2 y^3)dy - (2xy^4)dx}{(x^4)} = (2)dy - (3y)dy$
    * $- \frac{2y^3[(2x)dy - (y)dx]}{(x^3)} = (2)dy - (3y)dy$
    * $- 2y^3[(2x)dy - (y)dx] = dy(2 - 3y)(x^3)$
    * $-(2x)dy - (y)dx = dy\frac{(2 - 3y)(x^3)}{2y^3}$
    * $(-y)dx = dy\frac{(2 - 3y)(x^3)}{2y^3} + 2x(dy)$
    * $(-y)dx = (dy)[\frac{2x^3 - 3yx^3}{2y^3} + 2x]$
    * $\frac{(-y)}{[\frac{2x^3 - 3yx^3}{2y^3} + 2x]} = \dd[y]{x}$

---

## Answers to Exercises, cont.

* Differentiate the following: $3y - \frac{y^4}{x^2} = 2y$
    * $(-y)dx = (dy)[\frac{2x^3 - 3yx^3}{2y^3} + 2x]$
    * $\dd[y]{x} = \frac{-y}{[\frac{2x^3 - 3yx^3 + 2x(2y^3)}{2y^3}]}$
    * $\dd[y]{x} = -y / \frac{2x^3 - 3yx^3 + 2x(2y^3)}{2y^3}$
    * $\dd[y]{x} = -y  (\frac{2y^3}{2x^3 - 3yx^3 + 2x(2y^3)})$

---

## Answers to Exercises, cont.

* Differentiate the following: $3y - \frac{y^4}{x^2} = 2y$
    * $\dd[y]{x} = -y  (\frac{2y^3}{2x^3 - 3yx^3 + 2x(2y^3)})$
    * $\dd[y]{x} = -\frac{2y^4}{2x^3 - 3yx^3 + 4xy^3}$

---

# [Next Unit](../Trancendentals/Lesson%201)