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

# Lesson 4: The Quotient Rule

---

<!--paginate: true-->

## Intro

* We can derive a few rules to differentiate quickly and efficiently.
* Previously, we derived the first four rules:
    * Constant: $\diff{x} c = 0$
    * Power: $\diff{x} x^n = nx^{n - 1}$
    * Sum / Difference: $\diff{x} (f(x) \pm g(x)) = \diff{x} f(x) \pm \diff{x} g(x)$
    * Product: $\diff{x} (f(x)g(x)) = f(x) (\diff{x} g(x)) + g(x) (\diff{x} f(x))$
* From this, we can derive another rule: **The Quotient Rule**

---

## Deriving the Quotient Rule

* $f(x) = \frac{g(x)}{h(x)}$
* $f(x) = g(x)[h(x)]^{-1}$
* $\diff{x} f(x) = g(x) [\diff{x} (h(x)^{-1})] + [h(x)]^{-1} [\diff{x} g(x)]$
* $f'(x) = g(x) [-1(h(x)^{-1 - 1}) \diff{x} h'(x)] + [h(x)]^{-1} [g'(x)]$
* $f'(x) = g(x) [-(h(x)^{-2}) h'(x)] + [h(x)]^{-1} [g'(x)]$
* $f'(x) = [h(x)]^{-1} g'(x) - g(x)h(x)^{-2}h'(x)$
* $f'(x) = (h(x))^{-2} [h(x)g'(x) - g(x)h'(x)]$
* $f'(x) = \frac{h(x)g'(x) - g(x)h'(x)}{(h(x))^2}$
* *I'll explain the differentiation of $h(x)^{-1}$ later.*

---

## The Quotient Rule

$\diff{x} f(x) = \frac{h(x) (\diff{x} g(x)) - g(x) (\diff{x} h(x))}{(h(x))^2}$

* Similar to the product rule, determining the derivative of each of the constituent functions is helpful.
* Then, we could substitute into this.
* Now, let's test this, shall we?

---

## Example 1

1. Differentiate the following function: $f(x) = \frac{13x^3}{5x - 1}$
    * $g(x) = 13x^3$
    * $h(x) = 5x - 1$
    * $\diff{x} f(x) = \frac{h(x) (\diff{x} g(x)) - g(x) (\diff{x} h(x))}{(h(x))^2}$
    * $f'(x) = \frac{(5x - 1)[\diff{x} (13x^3)] - (13x^3)[\diff{x} (5x - 1)]}{(5x - 1)^2}$
    * $f'(x) = \frac{(5x - 1)[3(13x^{3 - 1})] - (13x^3)[\diff{x} (5x) - \diff{x} (1)]}{(5x - 1)^2}$
    * $f'(x) = \frac{(5x - 1)(39x^2) - 5(13x^3)}{(5x - 1)^2}$

---

## Example 1, cont.

1. Differentiate the following function: $f(x) = \frac{13x^3}{5x - 1}$
    * $f'(x) = \frac{(5x - 1)(39x^2) - 5(13x^3)}{(5x - 1)^2}$
    * $f'(x) = \frac{195x^3 - 39x^2 - 65x^3}{(5x - 1)^2}$
    * $f'(x) = \frac{130x^3 - 39x^2}{(5x - 1)^2}$

* Differentiate the following function: $y = \frac{7x^2 - 3x}{2x^5}$ (ex. for reader)
* Differentiate the following function: $f(x) = \frac{7\sqrt{x}}{x^2 - 4x}$ (ex. for reader)

---

## Example 2

2. Differentiate the following function: $y = \frac{1 + x}{3x^2}$
    * $g(x) = 1 + x$
    * $h(x) = 3x^2$
    * $\diff{x} y = \frac{h(x) (\diff{x} g(x)) - g(x) (\diff{x} h(x))}{(h(x))^2}$
    * $\dd[y]{x} = \frac{(3x^2)[\diff{x} (1 + x)] - (1 + x)[\diff{x} (3x^2)]}{(3x^2)^2}$
    * $\dd[y]{x} = \frac{(3x^2)[\diff{x} (1) + \diff{x} (x)] - (1 + x)[2(3x^{2 - 1})]}{(3x^2)^2}$

---

## Example 2, cont.

2. Differentiate the following function: $y = \frac{1 + x}{3x^2}$
    * $\dd[y]{x} = \frac{(3x^2)[\diff{x} (1) + \diff{x} (x)] - (1 + x)[2(3x^{2 - 1})]}{(3x^2)^2}$
    * $\dd[y]{x} = \frac{3x^2 - [(1 + x)(6x)]}{(3x^2)^2}$
    * $\dd[y]{x} = \frac{3x^2 - (6x + 6x^2)}{(3x^2)^2}$
    * $\dd[y]{x} = \frac{- 6x - 3x^2}{(3x^2)^2}$

---

## Example 2, cont.

2. Differentiate the following function: $y = \frac{1 + x}{3x^2}$
    * $\dd[y]{x} = \frac{- 6x - 3x^2}{(3x^2)^2}$
    * $\dd[y]{x} = \frac{-3x(2 - x)}{(3x^2)^2}$
    * $\dd[y]{x} = \frac{-3x(2 - x)}{9x^4}$
    * $\dd[y]{x} = \frac{-(2 - x)}{3x^3}$

---

## Differentiation Laws

1. Constant: $\diff{x} c = 0$
2. Power: $\diff{x} x^n = nx^{n - 1}$
3. Sum / Difference: $\diff{x} [f(x) \pm g(x)] = \diff{x} [f(x)] \pm \diff{x} [g(x)]$
4. Product: $\diff{x} [f(x)g(x)] = f(x) [\diff{x} g(x)] + g(x) [\diff{x} f(x)]$
5. Quotient: $\diff{x} f(x) = \frac{h(x) (\diff{x} g(x)) - g(x) (\diff{x} h(x))}{(h(x))^2}$
6. Chain: Next Lesson
7 - 10. Next Unit

---

## Exercises for Reader

* Differentiate the following functions:
    * $f(x) = \frac{5x^2 - 1}{2x + 4}$ (ex. for reader)
    * $y = \frac{\sqrt[3]{x^2}}{2\sqrt{x}}$ (ex. for reader)
    * $f(x) = \frac{7\sqrt{x}}{x^2 - 4x}$ (ex. for reader)
    * $f(x) = \frac{2x^3}{x - 5}$ (ex. for reader, bonus: use product rule)
    * $y = \frac{(x^4)(2x - 1)}{4x^3}$ (ex. for reader)
    * $f(x) = \frac{3x^3 - 12x}{(x + 3)(2x - 7)}$ (ex. for reader)

---

# [Next Lesson](Lesson%205)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Differentiate the following function:  $y = \frac{7x^2 - 3x}{2x^5}$
    * $g(x) = 7x^2 - 3x$
    * $h(x) = 2x^5$
    * $\diff{x} y = \frac{h(x) (\diff{x} g(x)) - g(x) (\diff{x} h(x))}{(h(x))^2}$
    * $\diff{x} y = \frac{(2x^5) [\diff{x} (7x^2 - 3x)] - (7x^2 - 3x) [\diff{x} (2x^5)]}{(2x^5)^2}$
    * $\dd[y]{x} = \frac{(2x^5) [\diff{x} (7x^2) - \diff{x} (3x)] - (7x^2 - 3x) [\diff{x} (2x^5)]}{(2x^5)^2}$
    * $\dd[y]{x} = \frac{(2x^5)(14x - 3) - (7x^2 - 3x)[5(2x^{5 - 1})]}{(2x^5)^2}$

---

## Answers to Exercises, cont.

* Differentiate the following function:  $y = \frac{7x^2 - 3x}{2x^5}$
    * $\dd[y]{x} = \frac{(2x^5)(14x - 3) - (7x^2 - 3x)[5(2x^{5 - 1})]}{(2x^5)^2}$
    * $\dd[y]{x} = \frac{(2x^5)(14x - 3) - (7x^2 - 3x)(10x^4)}{(2x^5)^2}$
    * $\dd[y]{x} = \frac{28x^6 - 6x^5 - (70x^6 - 30x^5)}{(2x^5)^2}$
    * $\dd[y]{x} = \frac{24x^5 - 42x^6}{(2x^5)^2}$

---

## Answers to Exercises, cont.

* Differentiate the following function:  $y = \frac{7x^2 - 3x}{2x^5}$
    * $\dd[y]{x} = \frac{24x^5 - 42x^6}{(2x^5)^2}$
    * $\dd[y]{x} = \frac{2x^5(12 - 21x)}{(2x^5)^2}$
    * $\dd[y]{x} = \frac{(12 - 21x)}{2x^5}$
    * $\dd[y]{x} = \frac{3(4 - 7x)}{2x^5}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $f(x) = \frac{7\sqrt{x}}{x^2 - 4x}$
    * $g(x) = 7\sqrt{x}$
    * $h(x) = x^2 - 4x$
    * $\diff{x} f(x) = \frac{h(x) (\diff{x} g(x)) - g(x) (\diff{x} h(x))}{(h(x))^2}$
    * $\diff{x} f(x) = \frac{(x^2 - 4x) [\diff{x} (7\sqrt{x})] - (7\sqrt{x}) [\diff{x} (x^2 - 4x)]}{(x^2 - 4x)^2}$
    * $f'(x) = \frac{(x^2 - 4x) [\diff{x} (7x^\frac{1}{2})] - (7x^\frac{1}{2}) [\diff{x} (x^2) - \diff{x} (4x)]}{(x^2 - 4x)^2}$
    * $f'(x) = \frac{(x^2 - 4x)(\frac{7}{2} x^{\frac{1}{2} - 1}) - (7x^\frac{1}{2}) (2x - 4)}{(x^2 - 4x)^2}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $f(x) = \frac{7\sqrt{x}}{x^2 - 4x}$
    * $f'(x) = \frac{(x^2 - 4x)(\frac{7}{2} x^{\frac{1}{2} - 1}) - (7x^\frac{1}{2}) (2x - 4)}{(x^2 - 4x)^2}$
    * $f'(x) = \frac{(x^2 - 4x)(\frac{7}{2} x^{-\frac{1}{2}}) - (7x^\frac{1}{2}) (2x - 4)}{(x^2 - 4x)^2}$
    * $f'(x) = \frac{\frac{7}{2}x^\frac{3}{2} - \frac{28}{2}x^\frac{1}{2} - (14x^\frac{3}{2} - 28x^\frac{1}{2})}{(x^2 - 4x)^2}$
    * $f'(x) = \frac{\frac{7}{2}x^\frac{3}{2} - \frac{28}{2}x^\frac{1}{2} - 14x^\frac{3}{2} + 28x^\frac{1}{2}}{(x^2 - 4x)^2}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $f(x) = \frac{7\sqrt{x}}{x^2 - 4x}$
    * $f'(x) = \frac{\frac{7}{2}x^\frac{3}{2} - \frac{28}{2}x^\frac{1}{2} - 14x^\frac{3}{2} + 28x^\frac{1}{2}}{(x^2 - 4x)^2}$
    * $f'(x) = \frac{\frac{-21}{2}x^\frac{3}{2} + 14x^\frac{1}{2}}{(x^2 - 4x)^2}$
    * $f'(x) = \frac{-21x^\frac{3}{2} + 28x^\frac{1}{2}}{2(x^2 - 4x)^2}$
    * $f'(x) = \frac{7x^\frac{1}{2}(4 - 3x)}{2(x^2 - 4x)^2}$
    * $f'(x) = \frac{7(4 - 3x)}{2\sqrt{x^3}(x^2 + 8x + 4)}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $f(x) = \frac{5x^2 - 1}{2x + 4}$
    * $g(x) = 5x^2 - 1$
    * $h(x) = 2x + 4$
    * $\diff{x} f(x) = \frac{h(x) (\diff{x} g(x)) - g(x) (\diff{x} h(x))}{(h(x))^2}$
    * $\diff{x} f(x) = \frac{(2x + 4) [\diff{x} (5x^2 - 1)] - (5x^2 - 1) [\diff{x} (2x + 4)]}{(2x + 4)^2}$
    * $f'(x) = \frac{(2x + 4) [\diff{x} (5x^2) - \diff{x} (1)] - (5x^2 - 1) [\diff{x} (2x) + \diff{x} (4)]}{(2x + 4)^2}$
    * $f'(x) = \frac{(2x + 4) (10x) - (5x^2 - 1) (2)}{(2x + 4)^2}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $f(x) = \frac{5x^2 - 1}{2x + 4}$
    * $f'(x) = \frac{(2x + 4) (10x) - (5x^2 - 1) (2)}{(2x + 4)^2}$
    * $f'(x) = \frac{(20x^2 + 40x) - (10x^2 - 2)}{(2x + 4)^2}$
    * $f'(x) = \frac{20x^2 + 40x - 10x^2 + 2)}{(2x + 4)^2}$
    * $f'(x) = \frac{10x^2 + 40x + 2}{(2x + 4)^2}$
    * $f'(x) = \frac{10x^2 + 40x + 2}{(4x^2 + 16x + 16)}$
    * $f'(x) = \frac{2(5x^2 + 20x + 1)}{4(x^2 + 4x + 4)}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $f(x) = \frac{5x^2 - 1}{2x + 4}$
    * $f'(x) = \frac{2(5x^2 + 20x + 1)}{4(x^2 + 4x + 4)}$
    * $f'(x) = \frac{5x^2 + 20x + 1}{2(x^2 + 4x + 4)}$
    * $f'(x) = \frac{5x^2 + 20x + 1}{2(x + 2)^2}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $y = \frac{\sqrt[3]{x^2}}{2\sqrt{x}}$
    * $g(x) = \sqrt[3]{x^2}$
    * $h(x) = 2\sqrt{x}$
    * $\diff{x} y = \frac{h(x) (\diff{x} g(x)) - g(x) (\diff{x} h(x))}{(h(x))^2}$
    * $\diff{x} y = \frac{(2\sqrt{x}) [\diff{x} (\sqrt[3]{x^2})] - (\sqrt[3]{x^2}) [\diff{x} (2\sqrt{x})]}{(2\sqrt{x})^2}$
    * $\dd[y]{x} = \frac{(2x^\frac{1}{2}) [\diff{x} (x^\frac{2}{3})] - (x^\frac{2}{3}) [\diff{x} (2x^\frac{1}{2})]}{(2x^\frac{1}{2})^2}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $y = \frac{\sqrt[3]{x^2}}{2\sqrt{x}}$
    * $\dd[y]{x} = \frac{(2x^\frac{1}{2}) [\diff{x} (x^\frac{2}{3})] - (x^\frac{2}{3}) [\diff{x} (2x^\frac{1}{2})]}{(2x^\frac{1}{2})^2}$
    * $\dd[y]{x} = \frac{(2x^\frac{1}{2}) [\frac{2}{3}(x^{\frac{2}{3} - 1})] - (x^\frac{2}{3}) [\frac{1}{2}(2x^{\frac{1}{2} - 1})]}{(2x^\frac{1}{2})^2}$
    * $\dd[y]{x} = \frac{(2x^\frac{1}{2}) (\frac{2}{3}x^{-\frac{1}{3}}) - (x^\frac{2}{3}) (x^{-\frac{1}{2}})}{(2x^\frac{1}{2})^2}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $y = \frac{\sqrt[3]{x^2}}{2\sqrt{x}}$
    * $\dd[y]{x} = \frac{(2x^\frac{1}{2}) (\frac{2}{3}x^{-\frac{1}{3}}) - (x^\frac{2}{3})) (x^{-\frac{1}{2}})}{(2x^\frac{1}{2})^2}$
    * $\dd[y]{x} = \frac{\frac{4}{3}x^{\frac{1}{6}} - x^\frac{1}{6}}{(2x^\frac{1}{2})^2}$
    * $\dd[y]{x} = \frac{\frac{1}{3}x^{\frac{1}{6}}}{4x}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $y = \frac{\sqrt[3]{x^2}}{2\sqrt{x}}$
    * $\dd[y]{x} = \frac{\frac{1}{3}x^{\frac{1}{6}}}{4x}$
    * $\dd[y]{x} = \frac{x^{\frac{1}{6}}}{3(4x)}$
    * $\dd[y]{x} = \frac{x^{\frac{1}{6}}}{12x}$
    * $\dd[y]{x} = \frac{x^{\frac{-5}{6}}}{12}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $y = \frac{\sqrt[3]{x^2}}{2\sqrt{x}}$
    * $\dd[y]{x} = \frac{x^{\frac{-5}{6}}}{12}$

    * $\dd[y]{x} = \frac{1}{12x^{\frac{5}{6}}}$
    
    * $\dd[y]{x} = \frac{1}{12\sqrt[6]{x^5}}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $f(x) = \frac{2x^3}{x - 5}$
    * $g(x) = 2x^3$
    * $h(x) = x - 5$
    * $\diff{x} f(x) = \frac{h(x) (\diff{x} g(x)) - g(x) (\diff{x} h(x))}{(h(x))^2}$
    * $\diff{x} f(x) = \frac{(x - 5)[\diff{x} (2x^3)] - (2x^3)[\diff{x} (x - 5)]}{(x - 5)^2}$
    * $f'(x) = \frac{(x - 5)[\diff{x} (2x^3)] - (2x^3)[\diff{x} (x) - \diff{x} (5)]}{(x - 5)^2}$
    * $f'(x) = \frac{(x - 5)(6x^2) - (2x^3)}{(x - 5)^2}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $f(x) = \frac{2x^3}{x - 5}$   
    * $f'(x) = \frac{(x - 5)(6x^2) - (2x^3)}{(x - 5)^2}$
    * $f'(x) = \frac{6x^3 - 30x^2 - 2x^3}{(x - 5)^2}$
    * $f'(x) = \frac{4x^3 - 30x^2}{(x - 5)^2}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $y = \frac{(x^4)(2x - 1)}{4x^3}$
    * $f(x) = x^4$
    * $g(x) = 2x - 1$
    * $h(x) = 4x^3$
    * $\diff{x} y = \frac{h(x) (\diff{x} f(x)g(x)) - f(x)g(x) (\diff{x} h(x))}{(h(x))^2}$
    * $\diff{x} f(x)g(x) = f(x) \diff{x} [g(x)] + g(x) \diff{x} [f(x)]$
    * $\diff{x} y = \frac{h(x) (f(x) \diff{x} [g(x)] + g(x) \diff{x} [f(x)]) - f(x)g(x) (\diff{x} h(x))}{(h(x))^2}$
    * $\diff{x} y = \frac{(4x^3) [(x^4) \diff{x} (2x - 1) + (2x - 1) \diff{x} (x^4)] - (x^4)(2x - 1) (\diff{x} (4x^3))}{(4x^3)^2}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $y = \frac{(x^4)(2x - 1)}{4x^3}$
    * $\diff{x} y = \frac{(4x^3) [(x^4) \diff{x} (2x - 1) + (2x - 1) \diff{x} (x^4)] - (x^4)(2x - 1) (\diff{x} (4x^3))}{(4x^3)^2}$
    * $\diff{x} y = \frac{(4x^3) [(x^4) \diff{x} (2x) - \diff{x} (1) + (2x - 1) \diff{x} (x^4)] - (x^4)(2x - 1) (\diff{x} (4x^3))}{(4x^3)^2}$
    * $\dd[y]{x} = \frac{(4x^3) [(2x^4) + (2x - 1)(4x^3)] - (x^4)(2x - 1)(12x^2)}{(4x^3)^2}$
    * $\dd[y]{x} = \frac{(40x^7 - 16x^6) - (24x^7 - 12x^6)}{(4x^3)^2}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $y = \frac{(x^4)(2x - 1)}{4x^3}$
    * $\dd[y]{x} = \frac{(40x^7 - 16x^6) - (24x^7 - 12x^6)}{(4x^3)^2}$
    * $\dd[y]{x} = \frac{40x^7 - 16x^6 - 24x^7 + 12x^6}{(4x^3)^2}$
    * $\dd[y]{x} = \frac{16x^7 - 4x^6}{(4x^3)^2}$
    * $\dd[y]{x} = \frac{(4x^3)[4x^4 - x^3]}{(4x^3)^2}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $y = \frac{(x^4)(2x - 1)}{4x^3}$
    * $\dd[y]{x} = \frac{(4x^3)[4x^4 - x^3]}{(4x^3)^2}$
    * $\dd[y]{x} = \frac{4x^4 - x^3}{4x^3}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $f(x) = \frac{3x^3 - 12x}{(x + 3)(2x - 7)}$
    * $a(x) = 3x^3 - 12x$
    * $b(x) = x + 3$
    * $c(x) = 2x - 7$
    * $\diff{x} f(x) = \frac{b(x)c(x) (\diff{x} a(x)) - a(x) (\diff{x} b(x)c(x))}{(b(x)c(x))^2}$
    * $\diff{x} b(x)c(x) = b(x) (\diff{x} [c(x)]) + c(x) (\diff{x} [b(x)])$
    * $\diff{x} f(x) = \frac{b(x)c(x) (\diff{x} a(x)) - a(x) (b(x) (\diff{x} [c(x)]) + c(x) (\diff{x} [b(x)]))}{(b(x)c(x))^2}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $f(x) = \frac{3x^3 - 12x}{(x + 3)(2x - 7)}$
    * $a(x) = 3x^3 - 12x$
    * $b(x) = x + 3$
    * $c(x) = 2x - 7$
    * $\diff{x} f(x) = \frac{b(x)c(x) (\diff{x} a(x)) - a(x) (b(x) (\diff{x} [c(x)]) + c(x) (\diff{x} [b(x)]))}{(b(x)c(x))^2}$
    * $\diff{x} f(x) =$ 
    $\frac{(x + 3)(2x - 7) [\diff{x} (3x^3 - 12x)] - (3x^3 - 12x) ((x + 3)(\diff{x} [2x - 7]) + (2x - 7)(\diff{x} [(x + 3)]))}{((x + 3)(2x - 7))^2}$

---

## Answers to Exercises, cont.

* Differentiate the following function: $f(x) = \frac{3x^3 - 12x}{(x + 3)(2x - 7)}$
    * $\diff{x} f(x) =$ 
    $\frac{(x + 3)(2x - 7) [\diff{x} (3x^3 - 12x)] - (3x^3 - 12x) ((x + 3)(\diff{x} [2x - 7]) + (2x - 7)(\diff{x} [(x + 3)]))}{((x + 3)(2x - 7))^2}$
    * $f'(x) = \frac{(x + 3)(2x - 7)(9x^2 - 12) - (3x^3 - 12x) [(x + 3)(2) + (2x - 7)]}{((x + 3)(2x - 7))^2}$
    * $f'(x) = \frac{(x + 3)(2x - 7)(9x^2 - 12) - (3x^3 - 12x)(4x + 1)}{((x + 3)(2x - 7))^2}$
    * $f'(x) = \frac{18x^4 - 9x^3 - 189x^2 - 24x^2 + 12x + 252 - (12x^4 + 3x^3 - 48x^2 - 12x)}{((x + 3)(2x - 7))^2}$
    * $f'(x) = \frac{6x^4 - 12x^3 - 165x^2+ 24x + 252}{(2x^2 -x - 21)^2}$
    
---

# [Next Lesson](Lesson%205)