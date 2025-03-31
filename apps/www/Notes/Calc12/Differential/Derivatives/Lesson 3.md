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

# Lesson 3: The Product Rule

---

<!--paginate: true-->

## Intro

* We can derive a few rules to differentiate quickly and efficiently.
* Previously, we derived the first three rules:
    * Constant: $\diff{x} c = 0$
    * Power: $\diff{x} x^n = nx^{n - 1}$
    * Sum / Difference: $\diff{x} (f(x) \pm g(x)) = \diff{x} f(x) \pm \diff{x} g(x)$
* Now, we can derive another rule: **The Product Rule**

---

## The Product Rule

$\diff{x} [f(x)g(x)] = f(x) [\diff{x} g(x)] + g(x) [\diff{x} f(x)]$
* For this, determining the derivative of each of the constituent functions is helpful.
* Then, we could substitute into this.
* So, let's try this out, shall we?

---

## Example 1

1. Differentiate the following function: $f(x) = x^3 (x^2 + 2x)$
    * $g(x) = x^3$
    * $h(x) = x^2 + 2x$
    * $\diff{x} f(x) = g(x) [\diff{x} h(x)] + h(x) [\diff{x} g(x)]$
    * $f'(x) = x^3 [\diff{x} (x^2 + 2x)] + (x^2 + 2x) [\diff{x} (x^3)]$
    * $f'(x) = x^3 [\diff{x} (x^2) + \diff{x} (2x)] + (x^2 + 2x) [\diff{x} (x^3)]$
    * $f'(x) = x^3 (2x + 2) + (x^2 + 2x) [3(x^{3 - 1})]$
    * $f'(x) = x^3 (2x + 2) + (x^2 + 2x) (3x^2)$
    * $f'(x) = (2x^4 + 2x^3) + (3x^4 + 6x^3)$
    * $f'(x) = 5x^4 + 8x^3$

---

## Example 2

2. Differentiate the following function: $f(x) = \sqrt{x} (5x^4)$
    * $g(x) = x^\frac{1}{2}$
    * $h(x) = 5x^4$
    * $\diff{x} f(x) = g(x) [\diff{x} h(x)] + h(x) [\diff{x} g(x)]$
    * $f'(x) = (x^\frac{1}{2}) [\diff{x} (5x^4)] + (5x^4) [\diff{x} (x^\frac{1}{2})]$
    * $f'(x) = (x^\frac{1}{2}) [4(5x^{4 - 1})] + (5x^4) [\frac{1}{2} (x^{\frac{1}{2} - 1})]$
    * $f'(x) = (x^\frac{1}{2})(20x^3) + (5x^4) (\frac{1}{2} x^{-\frac{1}{2}})$
    * $f'(x) = (\frac{1}{2} x^{-\frac{1}{2}}) [(2x)(20x^3) + 5x^4]$
    * $f'(x) = (\frac{1}{2} x^{-\frac{1}{2}}) (45x^4)$

---

## Example 2, cont.

2. Differentiate the following function: $f(x) = \sqrt{x} (5x^4)$
    * $f'(x) = (\frac{1}{2} x^{-\frac{1}{2}}) (45x^4)$
    * $f'(x) = \frac{45x^4}{2x^\frac{1}{2}}$
    * $f'(x) = \frac{45x^4}{2\sqrt{x}}$

* Differentiate the following function: $f(x) = (x^2 - 7x)(x^3 + 2x - 8)$ (ex. for reader)
* Differentiate the following function: $y = x^3 (15x^4)$ (ex. for reader)

---

## Differentiation Laws

1. Constant: $\diff{x} c = 0$
2. Power: $\diff{x} x^n = nx^{n - 1}$
3. Sum / Difference: $\diff{x} [f(x) \pm g(x)] = \diff{x} [f(x)] \pm \diff{x} [g(x)]$
4. Product: $\diff{x} [f(x)g(x)] = f(x) [\diff{x} g(x)] + g(x) [\diff{x} f(x)]$
5. Quotient: Next Lesson (special case of 4)
6. Chain: Lesson 5 
7. Sine: Next Unit
8. Cosine: Next Unit
9. Exponential: Next Unit
10. Logarithmic: Next Unit

---

## Exercises for Reader

* Differentiate the following functions:
    * $f(x) = 5x^7 (\frac{6}{x})$ (ex. for reader)
    * $y = (5\sqrt{x^3})(9x^4)$ (ex. for reader)
    * $f(x) = (7 - x^2)(\sqrt{x})$ (ex. for reader)
    * $y = (5x^3 - x)(\frac{1}{2\sqrt{x}})$ (ex. for reader)
    * $f(x) = (3x^2 - x + 18)(2x^3 - x)$ (ex. for reader)

---

# [Next Lesson](Lesson%204)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Differentiate the following function $f(x) = (x^2 - 7x)(x^3 + 2x - 8)$
    * $g(x) = x^2 - 7x$
    * $h(x) = x^3 - 2x - 8$
    * $\diff{x} f(x) = g(x) [\diff{x} h(x)] + h(x) [\diff{x} g(x)]$
    * $f'(x) = (x^2 - 7x) [\diff{x} (x^3 - 2x - 8)] +$
    $(x^3 - 2x - 8) [\diff{x} (x^2 - 7x)]$
    * $f'(x) = (x^2 - 7x) [\diff{x} (x^3 - \diff{x} (2x) - \diff{x} (8)] +$ 
    $(x^3 - 2x - 8) [\diff{x} (x^2) - \diff{x} (7x)]$

---

## Answers to Exercises, cont.

* Differentiate the following function $f(x) = (x^2 - 7x)(x^3 + 2x - 8)$
    * $f'(x) = (x^2 - 7x) [\diff{x} (x^3 - \diff{x} (2x) - \diff{x} (8)] +$ 
    $(x^3 - 2x - 8) [\diff{x} (x^2) - \diff{x} (7x)]$
    * $f'(x) = (x^2 - 7x) [3(x^{3 - 1}) - 2] + (x^3 - 2x - 8)(2x - 7)$
    * $f'(x) = (x^2 - 7x)(3x^2 - 2) + (x^3 - 2x - 8)(2x - 7)$
    * $f'(x) = (3x^4 - 21x^3 - 2x^2 + 14x) +$
    $(2x^4 - 7x^3 - 4x^2 - 2x + 56)$
    * $f'(x) = 5x^4 - 28x^3 - 6x^2 + 12x + 56$

---

## Answers to Exercises, cont.

* Differentiate the following function: $y = x^3 (15x^4)$
    * $g(x) = x^3$
    * $h(x) = 15x^4$
    * $\diff{x} y = g(x) [\diff{x} h(x)] + h(x) [\diff{x} g(x)]$
    * $\dd[y]{x} = (x^3) [\diff{x} (15x^4)] + (15x^4) [\diff{x} (x^3)]$
    * $\dd[y]{x} = (x^3)[4(15x^{4 - 1})] + (15x^4)[3(x^{3 - 1})]$
    * $\dd[y]{x} = (x^3)(60x^3) + (15x^4)(3x^2)$

---

## Answers to Exercises, cont.

* Differentiate the following function: $y = x^3 (15x^4)$
    * $\dd[y]{x} = (x^3)(60x^3) + (15x^4)(3x^2)$
    * $\dd[y]{x} = 60x^6 + 45x^6$
    * $\dd[y]{x} = 105x^6$

---

## Answers to Exercises, cont.

* Differentiate the following function: $f(x) = 5x^7 (\frac{6}{x})$
    * $g(x) = 5x^7$
    * $h(x) = \frac{6}{x}$
    * $\diff{x} f(x) = g(x) [\diff{x} h(x)] + h(x) [\diff{x} g(x)]$
    * $\diff{x} f(x) = (5x^7) [\diff{x} \frac{6}{x}] + \frac{6}{x} [\diff{x} (5x^7)]$
    * $f'(x) = (5x^7) [\diff{x} (6x^{-1})] + \frac{6}{x} [7(5x^{7 - 1})]$
    * $f'(x) = (5x^7) [-1(6x^{-1 - 1})] + \frac{6}{x} [35x^6)]$
    * $f'(x) = (5x^7) (-6x^{-2}) + \frac{6}{x} (35x^6)$
    * $f'(x) = 210x^5 - 30x^5$
    * $f'(x) = 180x^5$

---

## Answers to Exercises, cont.

* Differentiate the following function: $f(x) = 5x^7 (\frac{6}{x})$
    * $f'(x) = 210x^5 - 30x^5$
    * $f'(x) = 180x^5$

---

## Answers to Exercises, cont.

* Differentiate the following function: $y = (5\sqrt{x^3})(9x^4)$
    * $g(x) = 5\sqrt{x^3}$
    * $h(x) = 9x^4$
    * $\diff{x} y = g(x) [\diff{x} h(x)] + h(x) [\diff{x} g(x)]$
    * $\diff{x} y = (5\sqrt{x^3})[\diff{x} 9x^4] + (9x^4)[\diff{x} 5\sqrt{x^3}]$
    * $\dd[y]{x} = (5x^\frac{3}{2})[\diff{x} 9x^4] + (9x^4)[\diff{x} 5x^\frac{3}{2}]$
    * $\dd[y]{x} = (5x^\frac{3}{2})[4(9x^{4 - 1})] + (9x^4)[\frac{3}{2} (5x^{\frac{3}{2} - 1})]$

---

## Answers to Exercises, cont.

* Differentiate the following function: $y = (5\sqrt{x^3})(9x^4)$
    * $\dd[y]{x} = (5x^\frac{3}{2})[4(9x^{4 - 1})] + (9x^4)[\frac{3}{2} (5x^{\frac{3}{2} - 1})]$
    * $\dd[y]{x} = (5x^\frac{3}{2})[4(9x^3)] + (9x^4)[\frac{3}{2} (5x^\frac{1}{2})]$
    * $\dd[y]{x} = (5x^\frac{3}{2})(36x^3) + (9x^4)(\frac{15}{2}x^\frac{1}{2})$
    * $\dd[y]{x} = 180x^\frac{9}{2} + \frac{135}{2}x^\frac{9}{2}$
    * $\dd[y]{x} = \frac{495}{2}x^\frac{9}{2}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $y = (5\sqrt{x^3})(9x^4)$
    * $\dd[y]{x} = \frac{495}{2}x^\frac{9}{2}$
    * $\dd[y]{x} = \frac{495\sqrt{x^9}}{2}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $f(x) = (7 - x^2)(\sqrt{x})$
    * $g(x) = 7 - x^2$
    * $h(x) = \sqrt{x}$
    * $\diff{x} f(x) = g(x) [\diff{x} h(x)] + h(x) [\diff{x} g(x)]$
    * $\diff{x} f(x) = (7 - x^2) [\diff{x} \sqrt{x}] + \sqrt{x} [\diff{x} (7 - x^2)]$
    * $f'(x) = (7 - x^2) [\diff{x} x^\frac{1}{2}] + x^\frac{1}{2} [\diff{x} (7) - \diff{x} (x^2)]$
    * $f'(x) = (7 - x^2) (\frac{1}{2} x^{-\frac{1}{2}}) + x^\frac{1}{2} (- 2x)$
    * $f'(x) = \frac{7}{2} x^{-\frac{1}{2}} - \frac{1}{2} x^\frac{3}{2} - 2x^\frac{3}{2}$


---

## Answers to Exercises, cont.

* Differentiate the following function: $f(x) = (7 - x^2)(\sqrt{x})$
    * $f'(x) = \frac{7}{2} x^{-\frac{1}{2}} - \frac{1}{2} x^\frac{3}{2} - 2x^\frac{3}{2}$
    * $f'(x) = \frac{7}{2} x^{-\frac{1}{2}} - \frac{3}{2} x^\frac{3}{2}$
    * $f'(x) = x^{-\frac{1}{2}} (\frac{7}{2} - \frac{3}{2} x^2)$
    * $f'(x) = \frac{7 - 3x^2}{2x^{\frac{1}{2}}}$
    * $f'(x) = \frac{7 - 3x^2}{2\sqrt{x}}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $y = (5x^3 - x)(\frac{1}{2\sqrt{x}})$
    * $g(x) = 5x^3 - x$
    * $h(x) = \frac{1}{2\sqrt{x}}$
    * $\diff{x} y = g(x) [\diff{x} h(x)] + h(x) [\diff{x} g(x)]$
    * $\diff{x} y = (5x^3 - x) [\diff{x} \frac{1}{2\sqrt{x}}] + \frac{1}{2\sqrt{x}} [\diff{x} (5x^3 - x)]$
    * $\dd[y]{x} = (5x^3 - x) [\diff{x} \frac{1}{2}x^{-\frac{1}{2}}] + \frac{1}{2}x^{-\frac{1}{2}} [\diff{x} (5x^3) - \diff{x} (x)]$

---

## Answers to Exercises, cont.

* Differentiate the following function: $y = (5x^3 - x)(\frac{1}{2\sqrt{x}})$
    * $\dd[y]{x} = (5x^3 - x) [\diff{x} \frac{1}{2}x^{-\frac{1}{2}}] + \frac{1}{2}x^{-\frac{1}{2}} [\diff{x} (5x^3) - \diff{x} (x)]$
    * $\dd[y]{x} = (5x^3 - x) [-\frac{1}{2} (\frac{1}{2}x^{-\frac{1}{2} - 1})] + \frac{1}{2}x^{-\frac{1}{2}} [3(5x^{3 - 1}) - 1]$
    * $\dd[y]{x} = (5x^3 - x) [-\frac{1}{4}x^{-\frac{3}{2}})] + \frac{1}{2}x^{-\frac{1}{2}} (15x^2 - 1)$
    * $\dd[y]{x} = [-\frac{5}{4}x^{3 - \frac{3}{2}} + \frac{1}{4}x^{1 - \frac{3}{2}}] + [\frac{15}{2}x^{2 - \frac{1}{2}} - \frac{1}{2}x^{-\frac{1}{2}}]$

---

## Answers to Exercises, cont.

* Differentiate the following function: $y = (5x^3 - x)(\frac{1}{2\sqrt{x}})$
    * $\dd[y]{x} = [-\frac{5}{4}x^{3 - \frac{3}{2}} + \frac{1}{4}x^{1 - \frac{3}{2}}] + [\frac{15}{2}x^{2 - \frac{1}{2}} - \frac{1}{2}x^{-\frac{1}{2}}]$
    * $\dd[y]{x} = [\frac{1}{4}x^{-\frac{1}{2}} - \frac{5}{4}x^\frac{3}{2}] + [\frac{15}{2}x^\frac{3}{2} - \frac{1}{2}x^{-\frac{1}{2}}]$
    * $\dd[y]{x} = [\frac{1}{4}x^{-\frac{1}{2}} - \frac{5}{4}x^\frac{3}{2}] + [\frac{15}{2}x^\frac{3}{2} - \frac{1}{2}x^{-\frac{1}{2}}]$
    * $\dd[y]{x} = \frac{25x^2 - 1}{4\sqrt{x}}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $f(x) = (3x^2 - x + 18)(2x^3 - x)$
    * $g(x) = 3x^2 - x + 18$
    * $h(x) = 2x^3 - x$
    * $\diff{x} f(x) = g(x) [\diff{x} h(x)] + h(x) [\diff{x} g(x)]$
    * $\diff{x} f(x) = (3x^2 - x + 18) [\diff{x} (2x^3 - x)] +$ 
    $(2x^3 - x) [\diff{x} (3x^2 - x + 18)]$
    * $f'(x) = (3x^2 - x + 18) [\diff{x} (2x^3) - \diff{x} (x)] +$ 
    $(2x^3 - x) [\diff{x} (3x^2) - \diff{x} (x) + \diff{x} (18)]$

---

## Answers to Exercises, cont.

* Differentiate the following function: $f(x) = (3x^2 - x + 18)(2x^3 - x)$
    * $f'(x) = (3x^2 - x + 18) [\diff{x} (2x^3) - \diff{x} (x)] +$ 
    $(2x^3 - x) [\diff{x} (3x^2) - \diff{x} (x) + \diff{x} (18)]$
    * $f'(x) = (3x^2 - x + 18)(6x^2 - 1) + (2x^3 - x)(6x - 1)$
    * $f'(x) = (18x^4 - 6x^3 + 105x^2 + x - 18)$ 
    $+ (12x^4 - 2x^3 - 6x^2 + x)$
    * $f'(x) = 30x^4 - 4x^3 + 99x^2 + 2x - 18$ 

---

# [Next Lesson](Lesson%203)