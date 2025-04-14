---
marp: true
theme: uncover
class: invert
math: mathjax
---

$\newcommand\diff[1]{\mathcal{d}_{#1}}$
$\newcommand\dd[2][]{\displaystyle\frac{d#1}{d#2}}$

# <!--fit--> Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2025-->

$\newcommand\limit[2]{\displaystyle\lim_{#1 \to #2}}$

---

# Lesson 5: The Chain Rule

---

<!--paginate: true-->

## Intro

* We can derive a few rules to differentiate quickly and efficiently.
* Previously, we derived the first five rules:
    * Constant: $\diff{x} c = 0$
    * Power: $\diff{x} x^n = nx^{n - 1}$
    * Sum / Difference: $\diff{x} (f(x) \pm g(x)) = \diff{x} f(x) \pm \diff{x} g(x)$
    * Product: $\diff{x} (f(x)g(x)) = f(x) (\diff{x} g(x)) + g(x) (\diff{x} f(x))$
    * Quotient: $\diff{x} f(x) = \frac{h(x) (\diff{x} g(x)) - g(x) (\diff{x} h(x))}{(h(x))^2}$
* From this, we can derive another rule: **The Chain Rule**

---

## The Chain Rule

* The Chain Rule is useful once we get to differentiating composite functions.
* Given that $f(x) = g(h(x))$:

$\diff{x} f(x) = \diff{x} g(h(x)) [\diff{x} h(x)]$

* Remember the quotient rule derivation? This is why it works.
* So, let's try this out, shall we?

---

## Example 1

1. Differentiate the following function: $f(x) = (x^2 - 2)^4$
    * Approach 1: $\diff{x} f(x) = \diff{x} g(h(x)) [\diff{x} h(x)]$
    * $g(x) = x^4$
    * $h(x) = x^2 - 2$
    * $\diff{x} f(x) = \diff{x} (x^2 - 2)^4 [\diff{x} (x^2 - 2)]$
    * $\diff{x} f(x) = \diff{x} (x^2 - 2)^4 [\diff{x} (x^2) - \diff{x} (2)]$
    * $f'(x) = 2x [4(x^2 - 2)^{4 - 1}]$
    * $f'(x) = 8x(x^2 - 2)^3$

---

## Example 1, cont.

1. Differentiate the following function: $f(x) = (x^2 - 2)^4$
    * Approach 2: $\diff{x} y = \diff{u} y (\diff{x} u)$
    * $y = u^4$
    * $u = x^2 - 2$
    * $\diff{x} y = \diff{u} u^4 [\diff{x} (x^2 - 2)]$
    * $\diff{x} y = \diff{u} u^4 [\diff{x} (x^2) - \diff{x} (2)]$
    * $\dd[y]{x} = 4u^3(2x)$
    * $\dd[y]{x} = 8x(x^2 - 2)^3$

---

## Example 2

2. Differentiate the following function: $f(x) = \sqrt{3x^4 - x}$
    * $f(x) = (3x^4 - x)^\frac{1}{2}$
    * $g(x) = x^\frac{1}{2}$
    * $h(x) = 3x^4 - x$
    * $\diff{x} f(x) = \diff{x} g(h(x)) [\diff{x} h(x)]$
    * $\diff{x} f(x) = \diff{x} (3x^4 - x)^\frac{1}{2} [\diff{x} (3x^4 - x)]$
    * $\diff{x} f(x) = \diff{x} (3x^4 - x)^\frac{1}{2} [\diff{x} (3x^4) - \diff{x} (x)]$
    * $f'(x) = \frac{1}{2}(3x^4 - x)^{-\frac{1}{2}} [4(3x^3) - 1]$
    * $f'(x) = \frac{1}{2}(3x^4 - x)^{-\frac{1}{2}} (12x^3 - 1)$

---

## Example 2, cont.

2. Differentiate the following function: $f(x) = \sqrt{3x^4 - x}$
    * $f'(x) = \frac{1}{2}(3x^4 - x)^{-\frac{1}{2}} (12x^3 - 1)$
    * $f'(x) = \frac{12x^3 - 1}{2(3x^4 - x)^\frac{1}{2}}$
    * $f'(x) = \frac{12x^3 - 1}{2 \sqrt{3x^4 - x}}$

---

## Product / Quotient Rule + Chain Rule

* When it comes to using Product / Quotient rule with the Chain rule, in most cases, the Chain rule would be incorporated into the steps for the Product / Quotient rule.

---

## Example 3

3. Differentiate the following function: $f(x) = 3x^2 (2 - x^2)^3$
    * $g(x) = 3x^2$
    * $u = 2 - x^2$
    * $y = u^3$
    * $h(x) = (2 - x^2)^3$
    * $\diff{x} f(x) = g(x) (\diff{x} h(x)) + h(x) (\diff{x} g(x))$
    * $\diff{x} f(x) = (3x^2) [\diff{x} h(x)] + (2 - x^2)^3 [\diff{x} (3x^2)]$
    * $\diff{x} f(x) = (3x^2) [\diff{u} y (\diff{x} u)] + (2 - x^2)^3 [\diff{x} (3x^2)]$

---

## Example 3, cont.

3. Differentiate the following function: $f(x) = 3x^2 (2 - x^2)^3$
    * $u = 2 - x^2$
    * $y = u^3$
    * $\diff{x} f(x) = (3x^2) [\diff{u} y (\diff{x} u)] + (2 - x^2)^3 [\diff{x} (3x^2)]$
    * $\diff{x} f(x) = (3x^2) [\diff{u} (u^3) \diff{x} (2 - x^2)] + (2 - x^2)^3 [\diff{x} (3x^2)]$
    * $\diff{x} f(x) = (3x^2) [\diff{u} (u^3) (\diff{x} (2) - \diff{x} (x^2))]$ 
    $+ (2 - x^2)^3 [\diff{x} (3x^2)]$
    * $f'(x) = (3x^2) [3(u^2) (-2x)] + (2 - x^2)^3 [2(3x)]$

---

## Example 3, cont.

3. Differentiate the following function: $f(x) = 3x^2 (2 - x^2)^3$
    * $u = 2 - x^2$
    * $f'(x) = (3x^2) [3(u^2) (-2x)] + (2 - x^2)^3 [2(3x)]$
    * $f'(x) = (3x^2) [3(2 - x^2)^2(-2x)] + (2 - x^2)^3 [2(3x)]$
    * $f'(x) = (3x^2)(-6x)(2 - x^2)^2 + (6x)(2 - x^2)^3$
    * $f'(x) = (6x)(2 - x^2)^3 - (18x^3)(2 - x^2)^2$
    * $f'(x) = 6x(2 - x^2)^2[(2 - x^2) - (3x^2)]$
    * $f'(x) = 6x(2 - x^2)^2(2 - 4x^2)$

---

## Example 4

4. Differentiate the following function: $f(x) = \frac{5x^4}{\sqrt{7x - 3}}$
    * $g(x) = 5x^4$
    * $u = 7x - 3$
    * $y = u^\frac{1}{2}$
    * $h(x) = (7x - 3)^\frac{1}{2}$
    * $\diff{x} f(x) = \frac{h(x) (\diff{x} g(x)) - g(x) (\diff{x} h(x))}{(h(x))^2}$
    * $\diff{x} f(x) = \frac{(7x - 3)^\frac{1}{2} [\diff{x} (5x^4)] - (5x^4) [\diff{x} h(x)]}{[(7x - 3)^\frac{1}{2}]^2}$

---

## Example 4

4. Differentiate the following function: $f(x) = \frac{5x^4}{\sqrt{7x - 3}}$
    * $u = 7x - 3$
    * $y = u^\frac{1}{2}$
    * $\diff{x} f(x) = \frac{(7x - 3)^\frac{1}{2} [\diff{x} (5x^4)] - (5x^4) [\diff{x} h(x)]}{[(7x - 3)^\frac{1}{2}]^2}$
    * $\diff{x} f(x) = \frac{(7x - 3)^\frac{1}{2} [\diff{x} (5x^4)] - (5x^4) [(\diff{u} y)(\diff{x} u)]}{[(7x - 3)^\frac{1}{2}]^2}$
    * $\diff{x} f(x) = \frac{(7x - 3)^\frac{1}{2} [\diff{x} (5x^4)] - (5x^4) [(\diff{u} u^\frac{1}{2})(\diff{x} (7x - 3))]}{[(7x - 3)^\frac{1}{2}]^2}$

---

## Example 4

4. Differentiate the following function: $f(x) = \frac{5x^4}{\sqrt{7x - 3}}$
    * $u = 7x - 3$
    * $y = u^\frac{1}{2}$
    * $\diff{x} f(x) = \frac{(7x - 3)^\frac{1}{2} [\diff{x} (5x^4)] - (5x^4) [(\diff{u} u^\frac{1}{2})(\diff{x} (7x - 3))]}{[(7x - 3)^\frac{1}{2}]^2}$
    * $\diff{x} f(x) = \frac{(7x - 3)^\frac{1}{2} [\diff{x} (5x^4)] - (5x^4) [(\diff{u} u^\frac{1}{2})[\diff{x} (7x) - \diff{x} (3)]]}{[(7x - 3)^\frac{1}{2}]^2}$
    * $f'(x) = \frac{(7x - 3)^\frac{1}{2} (20x^3) - (5x^4) [(\frac{7}{2} u^{-\frac{1}{2}})]}{7x - 3}$

---

## Example 4

4. Differentiate the following function: $f(x) = \frac{5x^4}{\sqrt{7x - 3}}$
    * $u = 7x - 3$
    * $y = u^\frac{1}{2}$
    * $f'(x) = \frac{(7x - 3)^\frac{1}{2} (20x^3) - (5x^4) [(\frac{7}{2} u^{-\frac{1}{2}})]}{7x - 3}$
    * $f'(x) = \frac{(7x - 3)^\frac{1}{2} (20x^3) - (5x^4) [\frac{7}{2} (7x - 3)^{-\frac{1}{2}}]}{7x - 3}$
    * $f'(x) = \frac{\frac{5}{2}x^3(7x - 3)^{-\frac{1}{2}} [(7x - 3)(8) - (7x)]}{7x - 3}$
    * $f'(x) = \frac{5x^3(56x - 24 - 7x)}{2(7x - 3)^\frac{3}{2}}$

---

## Example 4

4. Differentiate the following function: $f(x) = \frac{5x^4}{\sqrt{7x - 3}}$
    * $f'(x) = \frac{5x^3(56x - 24 - 7x)}{2(7x - 3)^\frac{3}{2}}$
    * $f'(x) = \frac{5x^3(49x - 24)}{2\sqrt{(7x - 3)^3}}$

---

## Differentiation Laws

1. Constant: $\diff{x} c = 0$
2. Power: $\diff{x} x^n = nx^{n - 1}$
3. Sum / Difference: $\diff{x} [f(x) \pm g(x)] = \diff{x} [f(x)] \pm \diff{x} [g(x)]$
4. Product: $\diff{x} [f(x)g(x)] = f(x) [\diff{x} g(x)] + g(x) [\diff{x} f(x)]$
5. Quotient: $\diff{x} f(x) = \frac{h(x) (\diff{x} g(x)) - g(x) (\diff{x} h(x))}{(h(x))^2}$
6. Chain: $\diff{x} f(x) = \diff{x} g(h(x)) [\diff{x} h(x)]$ or $\diff{x} y = \diff{u} y (\diff{x} u)$
7 - 10. Next Unit

---

## Exercises for Readers

* Differentiate the following functions:
    * $f(x) = (5x^3 - x)^9$
    * $y = \sqrt{x^2 - 2x}$
    * $f(x) = x^3(3x - 1)^2$

---

# [Practice Quiz](Quiz)

Or

# [Next Lesson](Lesson%206)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercise

* Differentiate the following function: $f(x) = (5x^3 - x)^9$
    * $g(x) = x^9$
    * $h(x) = 5x^3 - x$
    * $\diff{x} f(x) = \diff{x} g(h(x)) [\diff{x} h(x)]$
    * $\diff{x} f(x) = \diff{x} (5x^3 - x)^9 [\diff{x} (5x^3 - x)]$
    * $\diff{x} f(x) = \diff{x} (5x^3 - x)^9 [\diff{x} (5x^3) - \diff{x} (x)]$
    * $\diff{x} f(x) = 9(5x^3 - x)^8 [3(5x^2) - 1]$
    * $\diff{x} f(x) = 9(5x^3 - x)^8 (15x^2 - 1)$
    * $\diff{x} f(x) = 9(15x^2 - 1)(5x^3 - x)^8$


---

## Answers to Exercise, cont.

* Differentiate the following function: $y = \sqrt{x^2 - 2x}$
    * $g(x) = x^\frac{1}{2}$
    * $h(x) = x^2 - 2x$
    * $\diff{x} y = \diff{x} g(h(x)) [\diff{x} h(x)]$
    * $\diff{x} y = \diff{x} (x^2 - 2x)^\frac{1}{2} [\diff{x} (x^2 - 2x)]$
    * $\diff{x} y = \diff{x} (x^2 - 2x)^\frac{1}{2} [\diff{x} (x^2) - \diff{x} (2x)]$
    * $\dd[y]{x} = \frac{1}{2}(x^2 - 2x)^{-\frac{1}{2}} (2x - 2)$
    * $\dd[y]{x} = (x^2 - 2x)^{-\frac{1}{2}} (x - 1)$

---

## Answers to Exercise, cont.

* Differentiate the following function: $y = \sqrt{x^2 - 2x}$
    * $\dd[y]{x} = (x^2 - 2x)^{-\frac{1}{2}} (x - 1)$
    * $\dd[y]{x} = \frac{x - 1}{(x^2 - 2x)^\frac{1}{2}}$
    * $\dd[y]{x} = \frac{x - 1}{\sqrt{x^2 - 2x}}$

---

## Answers to Exercise, cont.

* Differentiate the following function: $f(x) = x^3(3x - 1)^2$
    * $g(x) = x^3$
    * $h(x) = (3x - 1)^2$
    * $y = u^2$
    * $u = 3x - 1$
    * $\diff{x} f(x) = g(x) [\diff{x} h(x)] + h(x) [\diff{x} g(x)]$
    * $\diff{x} f(x) = g(x) [\diff{u} y (\diff{x} u)] + h(x) [\diff{x} g(x)]$
    * $\diff{x} f(x) = (x^3) [\diff{u} (u^2) (\diff{x} (3x - 1))] + (3x - 1)^2 [\diff{x} (x^3)]$

---

## Answers to Exercise, cont.

* Differentiate the following function: $f(x) = x^3(3x - 1)^2$
    * $y = u^2$
    * $u = 3x - 1$
    * $\diff{x} f(x) = (x^3) [\diff{u} (u^2) (\diff{x} (3x - 1))] + (3x - 1)^2 [\diff{x} (x^3)]$
    * $f'(x) = (x^3) [\diff{u} (u^2) (\diff{x} (3x) - \diff{x} (1))] + (3x - 1)^2 [\diff{x} (x^3)]$
    * $f'(x) = (x^3) [(2u)(3)] + (3x - 1)^2 (3x^2)$
    * $f'(x) = (x^3)(6u) + (3x - 1)^2 (3x^2)$
    * $f'(x) = (6x^3)(3x - 1) + (3x - 1)^2 (3x^2)$
    * $f'(x) = (3x^2)(3x - 1)[2x + 3x - 1]$
    * $f'(x) = (3x^2)(3x - 1)(5x - 1)$

---


# [Practice Quiz](Quiz)

Or

# [Next Lesson](Lesson%206)
