---
marp: true
theme: uncover
class: invert
math: mathjax
---

$\newcommand\diff[1]{\mathcal{d}_{#1}}$

# <!--fit--> Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

$\newcommand\dd[2][]{\displaystyle\frac{d#1}{d#2}}$

<!--_footer: In partnership with Hyperion University, 2025-->

---

# Unit 3 Practice Quiz

---

## Differentiation Laws

All questions here use these laws:

1. Constant: $\diff{x} c = 0$
2. Power: $\diff{x} x^n = nx^{n - 1}$
3. Sum / Difference: $\diff{x} [f(x) \pm g(x)] = \diff{x} [f(x)] \pm \diff{x} [g(x)]$
4. Product: $\diff{x} f(x) = g(x) [\diff{x} h(x)] + h(x) [\diff{x} g(x)]$
5. Quotient: $\diff{x} f(x) = \frac{h(x) (\diff{x} g(x)) - g(x) (\diff{x} h(x))}{(h(x))^2}$
6. Chain: $\diff{x} f(x) = \diff{x} g(h(x)) [\diff{x} h(x)]$ or $\diff{x} y = \diff{u} y (\diff{x} u)$

---

<!--paginate: true-->

## Questions

Differentiate the following functions:
1. $y = 8x^4 - 6x^3 + x - 7$
2. $f(x) = \sqrt{x} (x^2 - 6)$
3. $y = \frac{3x^3}{x - 3}$
4. $f(x) = (x^3 + 4)^6$
5. $f(x) = \frac{x\sqrt{x - 1}}{x + 2}$
6. $y = x^2 (3x^2 - 7)^4$

---

## Question 1 Answer

1. Differentiate the following function: $y = 8x^4 - 6x^3 + x - 7$
    * $\diff{x} y = \diff{x} (8x^4) - \diff{x} (6x^3) + \diff{x} (x) - \diff{x} (7)$
    * $\dd[y]{x} = 4(8x^3) - 3(6x^2) + 1$
    * $\dd[y]{x} = 32x^3 - 18x^2 + 1$

---

## Question 2 Answer

2. Differentiate the following function: $f(x) = \sqrt{x} (x^2 - 6)$
    * $g(x) = x^\frac{1}{2}$
    * $h(x) = x^2 - 6$
    * $\diff{x} f(x) = (x^\frac{1}{2}) [\diff{x} (x^2 - 6)] + (x^2 - 6) [\diff{x} (x^\frac{1}{2})]$
    * $\diff{x} f(x) = (x^\frac{1}{2}) [\diff{x} (x^2) - \diff{x} (6)] + (x^2 - 6) [\diff{x} (x^\frac{1}{2})]$
    * $f'(x) = (x^\frac{1}{2})(2x) + (x^2 - 6) (\frac{1}{2} x^{-\frac{1}{2}})$
    * $f'(x) = 2x^\frac{3}{2} + \frac{1}{2} x^\frac{3}{2} - 3x^{-\frac{1}{2}}$
    * $f'(x) = \frac{5}{2} x^\frac{3}{2} - 3x^{-\frac{1}{2}}$

---

## Question 2 Answer, cont.

2. Differentiate the following function: $f(x) = \sqrt{x} (x^2 - 6)$
    * $f'(x) = \frac{5}{2} x^\frac{3}{2} - 3x^{-\frac{1}{2}}$
    * $f'(x) = \frac{5x^\frac{3}{2}}{2} - \frac{3}{x^\frac{1}{2}}$
    * $f'(x) = \frac{5x^\frac{3}{4} - 6}{2x^\frac{1}{2}}$
    * $f'(x) = \frac{5\sqrt[4]{x^3} - 6}{2\sqrt{x}}$

---

## Question 3 Answer

3. Differentiate the following function: $y = \frac{3x^3}{x - 3}$
    * $g(x) = 3x^3$
    * $h(x) = x - 3$
    * $\diff{x} y = \frac{(x - 3) (\diff{x} (3x^3)) - (3x^3) (\diff{x} (x - 3))}{(x - 3)^2}$
    * $\diff{x} y = \frac{(x - 3) (\diff{x} (3x^3)) - (3x^3) [\diff{x} (x) - \diff{x} (3)]}{(x - 3)^2}$
    * $\dd[y]{x} = \frac{(x - 3)(9x^2) - (3x^3)}{(x - 3)^2}$

---

## Question 3 Answer, cont.

3. Differentiate the following function: $y = \frac{3x^3}{x - 3}$
    * $\dd[y]{x} = \frac{9x^3 - 27x^2 - 3x^3}{(x - 3)^2}$
    * $\dd[y]{x} = \frac{6x^3 - 27x^2}{(x - 3)^2}$

---

## Question 4 Answer

4. Differentiate the following function: $f(x) = (x^3 + 4)^6$
    * $y = u^6$
    * $u = x^3 + 4$
    * $\diff{x} f(x) = \diff{u} (u^6) [\diff{x} (x^3 + 4)]$
    * $\diff{x} f(x) = \diff{u} (u^6) [\diff{x} (x^3) + \diff{x} (4)]$
    * $f'(x) = (6u^5)(3x^2)$
    * $f'(x) = 6(x^3 + 4)^5 (3x^2)$
    * $f'(x) = (18x^2)(x^3 + 4)^5$

---

## Question 5 Answer

5. Differentiate the following function: $f(x) = \frac{x\sqrt{x - 1}}{x + 2}$
    * $g(x) = x(x - 1)^\frac{1}{2}$
    * $u = x - 1$
    * $h(x) = x + 2$
    * $\diff{x} g(x) = (x) [\diff{u} (u^\frac{1}{2}) (\diff{x} (x - 1))] + (x - 1)^\frac{1}{2} [\diff{x} (x)]$
    * $\diff{x} g(x) = (x)(\frac{1}{2} (x - 1)^{-\frac{1}{2}}) + (x - 1)^\frac{1}{2}$
    * $\diff{x} g(x) = (x - 1)^{-\frac{1}{2}}[\frac{3}{2}x - 1]$
    * $\diff{x} f(x) = \frac{(x + 2) [(x - 1)^{-\frac{1}{2}}(\frac{3}{2}x - 1)] - (x(x - 1)^\frac{1}{2}) [\diff{x} (x + 2)]}{(x + 2)^2}$

---

## Question 5 Answer, cont.

5. Differentiate the following function: $f(x) = \frac{x\sqrt{x - 1}}{x + 2}$
    * $\diff{x} f(x) = \frac{(x + 2) [(x - 1)^{-\frac{1}{2}}(\frac{3}{2}x - 1)] - (x(x - 1)^\frac{1}{2}) [\diff{x} (x + 2)]}{(x + 2)^2}$
    * $\diff{x} f(x) = \frac{(x + 2) [(x - 1)^{-\frac{1}{2}}(\frac{3}{2}x - 1)] - (x(x - 1)^\frac{1}{2}) [\diff{x} (x) + \diff{x} (2)]}{(x + 2)^2}$
    * $f'(x) = \frac{(x + 2) [(x - 1)^{-\frac{1}{2}}(\frac{3}{2}x - 1)] - x(x - 1)^\frac{1}{2}}{(x + 2)^2}$
    * $f'(x) = \frac{(x + 2) (\frac{3}{2}x - 1) - x(x - 1)^\frac{1}{2}}{(x - 1)^\frac{1}{2} (x + 2)^2}$
    * $f'(x) = \frac{(\frac{3}{2}x^2 + 2x - 2) - x\sqrt{x - 1}}{\sqrt{x - 1} (x + 2)^2}$

---

## Question 6 Answer

6. Differentiate the following function: $y = x^2 (3x^2 - 7)^4$
    * $g(x) = x^2$
    * $h(x) = (3x^2 - 7)^4$
    * $v = u^4$
    * $u = 3x^2 - 7$
    * $\diff{x} y = g(x) [\diff{u} v (\diff{x} u)] + h(x) [\diff{x} g(x)]$
    * $\diff{x} y = (x^2) [\diff{u} (u^4)\diff{x} (3x^2 - 7)] + (3x^2 - 7)^4 [\diff{x} (x^2)]$
    * $\diff{x} y = (x^2) [\diff{u} (u^4)(\diff{x} (3x^2) - \diff{x} (7))] + (3x^2 - 7)^4 [\diff{x} (x^2)]$
    * $\dd[y]{x} = (x^2)(4u^3)(6x) + (2x)(3x^2 - 7)^4$

---

## Question 6 Answer, cont.

6. Differentiate the following function: $y = x^2 (3x^2 - 7)^4$
    * $u = 3x^2 - 7$
    * $\dd[y]{x} = (x^2)(4u^3)(6x) + (2x)(3x^2 - 7)^4$
    * $\dd[y]{x} = 4(6x^3)(3x^2 - 7)^3 + (2x)(3x^2 - 7)^4$
    * $\dd[y]{x} = (24x^3)(3x^2 - 7)^3 + (2x)(3x^2 - 7)^4$
    * $\dd[y]{x} = (2x)(3x^2 - 7)^3 [12x^3 + 3x^2 - 7]$

---

# [Next Lesson](Lesson%206)