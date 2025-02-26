---
marp: true
theme: uncover
class: invert
math: mathjax
---

# <!--fit--> Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2025-->

---

# Lesson 1: Factoring

---

<!--paginate: true-->

## Intro

* The ability to simplify expressions is essential when working with what we'll be evaluating in future chapters.
* I'm assuming you're familiar with factoring, as well as several factoring methods.
* In this lesson, you'll be presented with three methods for factoring.

---

## Sum / Difference of Cubes

* Say we have these two cubic polynomials:
    * $a^3 + b^3$
    * $a^3 - b^3$
    * *How would we factor these?*
* First, we need to determine $a$ and $b$:
    * $a = \sqrt[3]{a^3}, b = \sqrt[3]{b^3}$
* Now, all we need is to determine how they're factored.

---

## How to Factor Cubes

* We know what $a$ and $b$ are.
* We have these two cubic polynomials:
    * $a^3 + b^3$
    * $a^3 - b^3$
* Let's factor them:
    * $a^3 + b^3 = (a + b)(a^2 - ab + b^2)$
    * $a^3 - b^3 = (a - b)(a^2 + ab + b^2)$

---

## Example 1

1. Factor $x^3 + 27$
    * $a^3 = x^3 \therefore a = x$
    * $\not\sqrt[3]{b^{\not3}} = \sqrt[3]{27}$
    * $b = 3$
    * Substitute: $x^3 + 3^3 = (x + 3)(x^2 - 3x + (3^2))$
    * $x^3 + 27 = (x + 3)(x^2 - 3x + 9)$

---

## Example 2

2. Factor the expression $8x^3 - y^3$
    * We know that $a^3 - b^3 = (a - b)(a^2 + ab + b^2)$
    * $(2x)^3 - y^3 = (2x - y)[(2x)^2 + 2xy + y^2]$
    * $8x^3 - y^3 = (2x - y)(4x^2 + 2xy + y^2)$

* Factor $8x^3 - 125y^3$ (ex. for reader)
* Factor $64x^3 + 1$ (ex. for reader)

---

## Rational Exponents

* Put simply, the variable with the smallest exponents should be factored out. 
* *Wait, what? How does that work?*
* Like this: $x^\frac{5}{2} + 3x^\frac{3}{2} + 2x^\frac{1}{2}$
    * $x^\frac{5}{2} + 3x^\frac{3}{2} + 2x^\frac{1}{2} = x^\frac{1}{2}(x^\frac{5-1}{2} + 3x^\frac{3-1}{2} + 2)$
    * $x^\frac{5}{2} + 3x^\frac{3}{2} + 2x^\frac{1}{2} = x^\frac{1}{2}(x^\frac{4}{2} + 3x^\frac{2}{2} + 2)$
    * $x^\frac{5}{2} + 3x^\frac{3}{2} + 2x^\frac{1}{2} = x^\frac{1}{2}(x^2 + 3x + 2)$
    * $x^\frac{5}{2} + 3x^\frac{3}{2} + 2x^\frac{1}{2} = x^\frac{1}{2}(x + 2)(x + 1)$

---

## Rational Example

3. Factor $x^\frac{1}{2} + 7x^\frac{-1}{2} + 12x^\frac{-3}{2}$
    * $x^\frac{1}{2} + 7x^\frac{-1}{2} + 12x^\frac{-3}{2} = x^\frac{-3}{2}(x^\frac{4}{2} + 7x^\frac{2}{2} + 12)$
    * $x^\frac{-3}{2}(x^2 + 7x + 12)$
    $x^\frac{-3}{2}(x + 3)(x + 4)$

* Factor $a^\frac{-1}{2} - 2a^\frac{-3}{2} - 35a^\frac{-5}{2}$ (ex. for reader)
* Factor $(x + 1)^\frac{3}{2} - 2(x + 1)^\frac{1}{2}$ (ex. for reader)
* Factor $5a^\frac{3}{2} - 20a^\frac{-1}{2}$ (ex. for reader)

---

## Difference of 'Squares'

* Recall that $x^2 - y^2 = (x + y)(x - y)$
* You may recognise this when $y \in \mathbb{Z}$ ($y$ is an integer):
    * $x^2 - 9 = (x + 3)(x - 3)$
* This also works when $y \not\in \mathbb{Z}$:
    * $x^2 - 3$
    * Since $x^2 - y^2 = (\sqrt{x^2} + \sqrt{y^2})(\sqrt{x^2} - \sqrt{y^2})$
    * We get that $x^2 - 3 = (x + \sqrt{3})(x - \sqrt{3})$
* Now, let's try this.

---

## 'Squares' Examples

4. Factor $x^2 - 5$
    * $x^2 - 5 = (x^2 + \sqrt{5})(x^2 - \sqrt{5})$
5. Factor $25x^2 - 8$
    * $25x^2 - 8 = (5x - \sqrt{8})(5x + \sqrt{8})$
    * $(5x - 2\sqrt{2})(5x + 2\sqrt{2})$

* Factor $x^2 - 20$. (ex. for reader)

---

# [Next Lesson](Lesson%202)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercise

* Factor $8x^3 - 125y^3$ 
    * $(2x - 5y)(4x62 + 10xy + 25x^2)$
* Factor $64x^3 + 1$
    * $(4x + 1)(16x^2 - 4x + 1)$
* Factor $a^\frac{-1}{2} - 2a^\frac{-3}{2} - 35a^\frac{-5}{2}$
    * $a^\frac{-5}{2}(a^2 - 2a - 35)$
    * $a^\frac{-5}{2}(a - 7)(a + 5)$

---

## Answers to Exercise (cont.)

* Factor $(x + 1)^\frac{3}{2} - 2(x + 1)^\frac{1}{2}$
    * $(x + 1)^\frac{1}{2}((x + 1) - 2)$
    * $(x + 1)^\frac{1}{2}(x - 1)$
* Factor $5a^\frac{3}{2} - 20a^\frac{-1}{2}$
    * $5a^\frac{-1}{2}(a^2 - 4)$
    * $5a^\frac{-1}{2}(a - 2)(a + 2)$
* Factor $x^2 - 20$
    * $(x + 2\sqrt{5})(x - 2\sqrt{5})$

---

# [Next Lesson](Lesson%202)