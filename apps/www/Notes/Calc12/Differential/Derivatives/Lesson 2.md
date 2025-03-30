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

# Lesson 2: The Power Rule

---

<!--paginate: true-->

## Intro

* From First Principles, we can derive a few rules to differentiate quickly and efficiently.
* We'll start by finding the derivative of a power function: $f(x) = x^n$.
    * $f'(x) = \limit{h}{0} \frac{f(x + h) - f(x)}{h}$
    * $f'(x) = \limit{h}{0} \frac{(x + h)^n - x^n}{h}$
    * Note: $\displaystyle(x + h)^n = \sum_{k = 0}^{n} \binom{n}{k} x^{n - k} h^k$

---

## Derivative of a Power Function

* For $f(x) = x^n$:
* $f'(x) = \limit{h}{0} \frac{(x + h)^n - x^n}{h}$
* Note: $\displaystyle(x + h)^n = \sum_{k = 0}^{n} \binom{n}{k} x^{n - k} h^k$
* $f'(x) = \limit{h}{0} \frac{C_1x^{n-1}h + C_2x^{n-2}h^2 + \cdots + C_{n - 1} xh^{n - 1} + h^n}{h}$
* $f'(x) = \limit{h}{0} C_1x^{n-1} + C_2x^{n-2}h + \cdots + C_{n - 1} xh^{n - 2} + h^{n - 1}$

---

## Derivative of a Power Function

* For $f(x) = x^n$:
* $f'(x) = \limit{h}{0} C_1x^{n-1} + C_2x^{n - 2} h + \cdots + C_{n - 1} xh^{n - 2} + h^{n - 1}$
* $f'(x) = C_1x^{n - 1}$ ($C_1 = n$)
* $f'(x) = nx^{n - 1}$
* This is the power rule, and it is one of nine important rules for differentiation.

---

## The Power Rule

$\displaystyle f(x) = x^n,\ f'(x) = nx^{n - 1}$
* Let's try this out, shall we?

---

## Example 1

1. Differentiate the following function: $f(x) = x^3$
    * $\diff{x} f(x) = \diff{x} x^3$
    * $f'(x) = 3x^{3 - 1}$
    * $f'(x) = 3x^2$

---

## Example 2

2. Differentiate the following function: $y = 3x^4$
    * $\diff{x} y = \diff{x} 3x^4$
    * $\dd[y]{x} = 12x^{4 - 1}$
    * $\dd[y]{x} = 12x^3$

* Differentiate the following function: $f(x) = 12x^5$ (ex. for reader)

---

## Sum and Difference

* These often contain constant terms, so let's understand how differentiating constants work:
* Let $f(x) = c$
    * $f'(x) = \limit{h}{0} \frac{f(x + h) - f(x)}{h}$
    * $f'(x) = \limit{h}{0} \frac{c - c}{h}$
    * $f'(x) = 0$
    * $\therefore \diff{x} c = 0$.

---

## Sum and Difference Rules

* These aren't one of the nine main derivative rules, but they do come up often.

$\diff{x} [f(x) \pm g(x)] = \diff{x} f(x) \pm \diff{x} g(x) = f'(x) \pm g'(x)$

* Let's test this out, shall we?

---

## Example 3

3. Find the derivative of the following function: $f(x) = 3x^4 - 2x^2 + 6$
    * $\diff{x} f(x) = \diff{x} (3x^4 - 2x^2 + 6)$
    * $f'(x) = \diff{x} (3x^4) - \diff{x} (2x^2) + \diff{x} (6)$
    * $f'(x) = 4(3x^{4 - 1}) - 2(2x^{2 - 1}) + 0$
    * $f'(x) = 12x^3 - 4x$

---

## Example 4

4. Differentiate the following function: $y = \frac{4}{x^2} + 3x$
    * Rewrite: $y = 4x^{-2} + 3x$
    * $\diff{x} y = \diff{x} (4x^{-2} + 3x)$
    * $\diff{x} y = \diff{x} (4x^{-2}) + \diff{x} (3x)$
    * $\dd[y]{x} = -2(4x^{-2 - 1}) + 3$
    * $\dd[y]{x} = -8x^{-3} + 3$
    * Rewrite: $\dd[y]{x} = 3 - \frac{8}{x^3}$

---

## Example 5

5. Differentiate the following function: $f(x) = 3\sqrt{x} - \sqrt[3]{x}$
    * Rewrite: $f(x) = 3x^\frac{1}{2} - x^\frac{1}{3}$
    * $\diff{x} f(x) = \diff{x} (3x^\frac{1}{2} - x^\frac{1}{3})$
    * $f'(x) = \diff{x} (3x^\frac{1}{2}) - \diff{x} (x^\frac{1}{3})$
    * $f'(x) = \frac{1}{2}(3x^{\frac{1}{2} - 1}) - \frac{1}{3} (x^{\frac{1}{3} - 1})$
    * $f'(x) = \frac{3}{2}(x^{-\frac{1}{2}}) - \frac{1}{3} x^{-\frac{2}{3}}$
    * Rewrite: $f'(x) = \frac{3}{2\sqrt{x}}- \frac{1}{3\sqrt[3]{x^2}}$

* Differentiate the following function: $y = \frac{2x + 3}{\sqrt{x}}$ (ex. for reader)

---

## Differentiation Laws

1. Constant: $\diff{x} c = 0$
2. Power: $\diff{x} x^n = nx^{n - 1}$
3. Sum / Difference: $\diff{x} [f(x) \pm g(x)] = \diff{x} [f(x)] \pm \diff{x} [g(x)]$
4. Product: Lesson 3
5. Quotient: Lesson 4 (special case of 3)
6. Chain: Lesson 5 
7. Sine: Next Unit
8. Cosine: Next Unit
9. Exponential: Next Unit
10. Logarithmic: Next Unit

---

## Exercises for Reader

* Differentiate the following functions:
    * $f(x) = 6x^3$
    * $y = \sqrt{x}$
    * $f(x) = \frac{1}{x^4}$
    * $y = 5 \sqrt[3]{x^4}$
    * $f(x) = 5x^3 - 2x$
    * $y = 4x^2 + x - 5$
    * $y = 2 \sqrt{x} - \frac{1}{2}$
    * $f(t) = \frac{4}{t} - \frac{1}{t^2}$

---

# [Next Lesson](Lesson%203)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Differentiate the following functions: 
    * $f(x) = 12x^5$
        * $\diff{x} f(x) = \diff{x} 12x^5$
        * $f'(x) = 5(12x^{5 - 1})$
        * $f'(x) = 60x^4$
    * $y = \frac{2x + 3}{\sqrt{x}}$
        * $y = \frac{2x}{\sqrt{x}} + \frac{3}{\sqrt{x}}$
        * $y = \frac{2x}{x^\frac{1}{2}} + \frac{3}{x^\frac{1}{2}}$

---

## Answers to Exercises, cont.

* Differentiate the following functions: 
    * $y = \frac{2x + 3}{\sqrt{x}}$
        * $y = \frac{2x}{x^\frac{1}{2}} + \frac{3}{x^\frac{1}{2}}$
        * $y = 2x^\frac{1}{2} + 3x^{-\frac{1}{2}}$
        * $\diff{x} y = \diff{x} [2x^\frac{1}{2} + 3x^{-\frac{1}{2}}]$
        * $\dd[y]{x} = \diff{x} (2x^\frac{1}{2}) + \diff{x} (3x^{-\frac{1}{2}})$
        * $\dd[y]{x} = \frac{1}{2}(2x^{\frac{1}{2} - 1}) - \frac{1}{2}(3x^{-\frac{1}{2} - 1})$

---

## Answers to Exercises, cont. 

* Differentiate the following functions: 
    * $y = \frac{2x + 3}{\sqrt{x}}$
        * $\dd[y]{x} = \frac{1}{2}(2x^{\frac{1}{2} - 1}) - \frac{1}{2}(3x^{-\frac{1}{2} - 1})$
        * $\dd[y]{x} = x^{-\frac{1}{2}} - \frac{3}{2} x^{-\frac{3}{2}}$
        * $\dd[y]{x} = \frac{1}{x^\frac{1}{2}} - \frac{3}{2x^{\frac{3}{2}}}$
        * $\dd[y]{x} = \frac{1}{\sqrt{x}} - \frac{3}{2\sqrt{x^3}}$

---

## Answers to Exercises, cont.

* Differentiate the following functions: 
    * $f(x) = 6x^3$
        * $\diff{x} f(x) = \diff{x} 6x^3$
        * $f'(x) = 3(6x^{3 - 1})$
        * $f'(x) = 18x^2$
    * $y = \sqrt{x}$
        * $y = x^\frac{1}{2}$
        * $\diff{x} y = \diff{x} x^\frac{1}{2}$
        * $\dd[y]{x} = \frac{1}{2} x^{\frac{1}{2} - 1}$

---

## Answers to Exercises, cont.

* Differentiate the following functions: 
    * $y = \sqrt{x}$
        * $\dd[y]{x} = \frac{1}{2} x^{\frac{1}{2} - 1}$
        * $\dd[y]{x} = \frac{1}{2} x^{-\frac{1}{2}}$
        * $\dd[y]{x} = \frac{1}{2x^\frac{1}{2}}$
        * $\dd[y]{x} = \frac{1}{2\sqrt{x}}$

---

## Answers to Exercises, cont.

* Differentiate the following functions: 
    * $f(x) = \frac{1}{x^4}$
        * $f(x) = x^{-4}$
        * $\diff{x} f(x) = \diff{x} x^{-4}$
        * $f'(x) = -4(x^{-4 - 1})$
        * $f'(x) = -4x^{-5}$
        * $f'(x) = \frac{-4}{x^5}$

---

## Answers to Exercises, cont.

* Differentiate the following functions: 
    * $y = 5 \sqrt[3]{x^4}$
        * $y = 5x^\frac{4}{3}$
        * $\diff{x} y = \diff{x} 5x^\frac{4}{3}$
        * $\dd[y]{x} = \frac{4}{3}(5x^{\frac{4}{3} - 1})$
        * $\dd[y]{x} = \frac{20}{3}x^\frac{1}{3}$
        * $\dd[y]{x} = \frac{20}{3\sqrt[3]{x}}$

---

## Answers to Exercises, cont.

* Differentiate the following functions: 
    * $f(x) = 5x^3 - 2x$
        * $\diff{x} f(x) = \diff{x} (5x^3 - 2x)$
        * $f'(x) = \diff{x} (5x^3) - \diff{x} (2x)$
        * $f'(x) = 3(5x^{3 - 1}) - 2$
        * $f'(x) = 15x^2 - 2$

---

## Answers to Exercises, cont.

* Differentiate the following functions: 
    * $y = 4x^2 + x - 5$
        * $\diff{x} y = \diff{x} (4x^2 + x - 5)$
        * $\dd[y]{x} = \diff{x} (4x^2) + \diff{x} (x) - \diff{x} (5)$
        * $\dd[y]{x} = 2(4x) + 1$
        * $\dd[y]{x} = 8x + 1$

---

## Answers to Exercises, cont.

* Differentiate the following functions: 
    * $y = 2 \sqrt{x} - \frac{1}{2}$
        * $y = 2x^\frac{1}{2} - \frac{1}{2}$
        * $\diff{x} y = \diff{x} (2x^\frac{1}{2} - \frac{1}{2})$
        * $\dd[y]{x} = \diff{x} (2x^\frac{1}{2}) - \diff{x} (\frac{1}{2})$
        * $\dd[y]{x} = \frac{1}{2}(2x^{\frac{1}{2} - 1})$
        * $\dd[y]{x} = x^{-\frac{1}{2}}$

---

## Answers to Exercises, cont.

* Differentiate the following functions: 
    * $y = 2 \sqrt{x} - \frac{1}{2}$
        * $\dd[y]{x} = x^{-\frac{1}{2}}$
        * $\dd[y]{x} = \frac{1}{x^\frac{1}{2}}$
        * $\dd[y]{x} = \frac{1}{\sqrt{x}}$

---

## Answers to Exercises, cont.

* Differentiate the following functions: 
    * $f(t) = \frac{4}{t} - \frac{1}{t^2}$
        * $f(t) = 4t^{-1} - t^{-2}$
        * $\diff{t} f(t) = \diff{t} (4t^{-1} - t^{-2})$
        * $f'(t) = \diff{t} (4t^{-1}) - \diff{t} (t^{-2})$
        * $f'(t) = -1(4t^{-1 - 1}) + 2(t^{-2 - 1})$
        * $f'(t) = 2t^{-3} - 4t^{-2} +$
        * $f'(t) = \frac{2}{t^3} - \frac{4}{t^2}$

---

# [Next Lesson](Lesson%203)