---
marp: true
theme: uncover
class: invert
math: mathjax
---

$\newcommand\diff[1]{\mathcal{d}_{#1}}$
$\newcommand\dd[3][]{\displaystyle\frac{d^{#1}#2}{d#3^{#1}}}$

# <!--fit--> Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2025-->

$\newcommand\limit[2]{\displaystyle\lim_{#1 \to #2}}$

---

# Lesson 6: Higher Order Derivatives

---

<!--paginate: true-->

## Intro

* The first time a function is differentiated, the result is known as the first derivative.
* However, we can go farther than that.
* We can differentiate the first derivative to get the second derivative.
* And we can differentiate the second derivative to get the third derivative, and so on.
* These are known as **Higher Order Derivatives**.

---

## A Note On Notation

* The *Order* of a derivative is the amount of times we have differentiated from the original function.
* Here's some common notation for
    * Second Order Derivatives:
        * $f''(x)$ or $y''$
        * $\dd[2]{y}{x}$ or $\dd[2]{f}{x}$
        * $(\diff{x}\circ\diff{x})f(x) = \diff{x}(\diff{x}(f(x))) = \diff{x}^2(f(x))$

---

## A Note On Notation, cont.
* Here's some common notation for
    * Third Order Derivatives:
        * $f'''(x)$ or $y'''$
        * $\dd[3]{y}{x}$ or $\dd[3]{f}{x}$
        * $(\diff{x} \circ \diff{x}\circ\diff{x})f(x) = \diff{x}(\diff{x}(\diff{x}(f(x)))) = \diff{x}^3(f(x))$
* Higher Order Derivatives represent the rate of change of the slope of the tangent line of the Derivative 1 degree lower.

---

## Important Note
* It's important to fully simplify each derivative before taking the next derivative. 
* This reduces the number of rules required and keeps differentiation manageable.

---

## Example 1

1. Find the Second derivative of $f(x) = x^3 - 2x^2 + 5x - 7$
    * $\diff{x}^2 f(x) = \diff{x}(\diff{x}(x^3 - 2x^2 + 5x - 7))$
    * $\diff{x}(\diff{x} f(x)) = \diff{x}(\diff{x}(x^3) - \diff{x}(2x^2) + \diff{x}(5x) - \diff{x}(7))$
    * $\diff{x}(\diff{x} f(x)) = \diff{x}(\diff{x}(x^3) - \diff{x}(2x^2) + \diff{x}(5x) - \diff{x}(7))$
    * $\diff{x} f'(x) = \diff{x}(3x^2 - 4x + 5)$
    * $\diff{x} f'(x) = \diff{x}(3x^2) - \diff{x}(4x) + \diff{x}(5)$
    * $f''(x) = 6x - 4$

---

## Example 2

2. Find the Second derivative of $y = \frac{2x^2}{3x - 1}$
    * $g(x) = 2x^2$
    * $h(x) = 3x - 1$
    * $\diff{x}^2 y = \diff{x} \frac{(3x - 1) (\diff{x} (2x^2)) - (2x^2) (\diff{x} (3x - 1))}{(3x - 1)^2}$
    * $\diff{x}^2 y = \diff{x} \frac{(3x - 1) [\diff{x} (2x^2)] - (2x^2) [\diff{x} (3x) - \diff{x} (1)]}{(3x - 1)^2}$
    * $\diff{x} \dd{y}{x} = \diff{x} \frac{(3x - 1)(4x) - (2x^2)(3)}{(3x - 1)^2}$
    * $\diff{x} \dd{y}{x} = \diff{x} \frac{12x^2 - 4x - 6x^2}{(3x - 1)^2}$

---

## Example 2, cont.

2. Find the Second derivative of $y = \frac{2x^2}{3x - 1}$
    * $\diff{x} \dd{y}{x} = \diff{x} \frac{12x^2 - 4x - 6x^2}{(3x - 1)^2}$
    * $\diff{x} \dd{y}{x} = \diff{x} \frac{6x^2 - 4x}{(3x - 1)^2}$
    * $g(x) = 6x^2 - 4x$
    * $h(x) = (3x - 1)^2$
    * $a(u) = u^2$
    * $u = 3x - 1$

---

## Example 2, cont.

2. Find the Second derivative of $y = \frac{2x^2}{3x - 1}$
    * $g(x) = 6x^2 - 4x$
    * $h(x) = (3x - 1)^2$
    * $a(u) = u^2$
    * $u = 3x - 1$
    * $\diff{x} \dd{y}{x} =$ $\frac{(3x - 1)^2 [\diff{x} (6x^2 - 4x)] - (6x^2 - 4x) (\diff{u} (u^2) (\diff{x} (3x - 1)))}{[(3x - 1)^2]^2}$
    * $\diff{x} \dd{y}{x} =$ $\frac{(3x - 1)^2 [\diff{x} (6x^2) - \diff{x} (4x)] - (6x^2 - 4x) (\diff{u} (u^2) (\diff{x} (3x) - \diff{x} (1)))}{[(3x - 1)^2]^2}$

---

## Example 2, cont.

2. Find the Second derivative of $y = \frac{2x^2}{3x - 1}$
    * $g(x) = 6x^2 - 4x$
    * $h(x) = (3x - 1)^2$
    * $a(u) = u^2$
    * $u = 3x - 1$
    * $\diff{x} \dd{y}{x} =$ $\frac{(3x - 1)^2 [\diff{x} (6x^2) - \diff{x} (4x)] - (6x^2 - 4x) (\diff{u} (u^2) (\diff{x} (3x) - \diff{x} (1)))}{[(3x - 1)^2]^2}$
    * $\dd[2]{y}{x} =$ $\frac{(3x - 1)^2 (12x - 4) - (6x^2 - 4x)(6)(3x - 1)}{(3x - 1)^4}$

---

## Example 2, cont.

2. Find the Second derivative of $y = \frac{2x^2}{3x - 1}$
    * $\dd[2]{y}{x} = \frac{(3x - 1)^2 (12x - 4) - (6x^2 - 4x)(6)(3x - 1)}{(3x - 1)^4}$
    * $\dd[2]{y}{x} = \frac{4(3x - 1)^3 - 6(6x^2 - 4x)(3x - 1)}{(3x - 1)^4}$
    * $\dd[2]{y}{x} = \frac{2(3x - 1)[2(3x - 1)^2 - 3(6x^2 - 4x)]}{(3x - 1)^4}$
    * $\dd[2]{y}{x} = \frac{2(3x - 1)[18x^2 - 12x + 2 - 18x^2 + 12x]}{(3x - 1)^4}$

---

## Example 2, cont.

2. Find the Second derivative of $y = \frac{2x^2}{3x - 1}$
    * $\dd[2]{y}{x} = \frac{2(3x - 1)[18x^2 - 12x + 2 - 18x^2 + 12x]}{(3x - 1)^4}$
    * $\dd[2]{y}{x} = \frac{4(3x - 1)}{(3x - 1)^4}$
    * $\dd[2]{y}{x} = \frac{4}{(3x - 1)^3}$

---

## Example 3

3. Find the second derivative of $f(x) = \frac{\sqrt{x}}{x + 3}$
    * $g(x) = x^\frac{1}{2}$
    * $h(x) = x + 3$
    * $\diff{x}^2 f(x) = \diff{x} \frac{(x + 3) [\diff{x} (x^\frac{1}{2})] - (x^\frac{1}{2}) [\diff{x} (x + 3)]}{(x + 3)^2}$
    * $\diff{x}^2 f(x) = \diff{x} \frac{(x + 3) [\diff{x} (x^\frac{1}{2})] - (x^\frac{1}{2}) [\diff{x} (x) + \diff{x} (3)]}{(x + 3)^2}$
    * $\diff{x} f'(x) = \diff{x} \frac{(x + 3) [\diff{x} (x^\frac{1}{2})] - (x^\frac{1}{2}) [\diff{x} (x) + \diff{x} (3)]}{(x + 3)^2}$
    * $\diff{x} f'(x) = \diff{x} \frac{(x + 3) \frac{1}{2}(x^{-\frac{1}{2}}) - x^\frac{1}{2}}{(x + 3)^2}$

---

## Example 3, cont.

3. Find the second derivative of $f(x) = \frac{\sqrt{x}}{x + 3}$
    * $\diff{x} f'(x) = \diff{x} \frac{(x + 3) \frac{1}{2}(x^{-\frac{1}{2}}) - x^\frac{1}{2}}{(x + 3)^2}$
    * $\diff{x} f'(x) = \diff{x} \frac{\frac{1}{2}x^{-\frac{1}{2}} (x + 3 - 2x)}{(x + 3)^2}$
    * $\diff{x} f'(x) = \diff{x} \frac{3 - x}{2x^\frac{1}{2}(x + 3)^2}$

---

## Example 3, cont.

3. Find the second derivative of $f(x) = \frac{\sqrt{x}}{x + 3}$
    * $g(x) = 3 - x$
    * $h(x) = 2x^\frac{1}{2}(x + 3)^2$
    * $u = x + 3$
    * $\diff{x} f'(x) =$ $\frac{[2x^\frac{1}{2}(x + 3)^2] [\diff{x} (3 - x)] - (3 - x) (\diff{x} (2x^\frac{1}{2}) [\diff{u} u^2 (\diff{x} (x + 3))] + (x + 3)^2 [\diff{x} (2x^\frac{1}{2})])}{[2x^\frac{1}{2}(x + 3)^2]^2}$
    * $\diff{x} f'(x) =$ $\frac{[2x^\frac{1}{2}(x + 3)^2] [\diff{x} (3) - \diff{x} (x)] - (3 - x) (2x^\frac{1}{2}) [\diff{u} u^2 (\diff{x} (x) + \diff{x} (3))] + (x + 3)^2 [\diff{x} (2x^\frac{1}{2})]}{[2x^\frac{1}{2}(x + 3)^2]^2}$

---

## Example 3, cont.

3. Find the second derivative of $f(x) = \frac{\sqrt{x}}{x + 3}$
    * $g(x) = 3 - x$
    * $h(x) = 2x^\frac{1}{2}(x + 3)^2$
    * $u = x + 3$
    * $\diff{x} f'(x) =$ $\frac{[2x^\frac{1}{2}(x + 3)^2] [\diff{x} (3) - \diff{x} (x)] - (3 - x) (2x^\frac{1}{2}) [\diff{u} u^2 (\diff{x} (x) + \diff{x} (3))] + (x + 3)^2 [\diff{x} (2x^\frac{1}{2})]}{[2x^\frac{1}{2}(x + 3)^2]^2}$
    * $f''(x) = \frac{[2x^\frac{1}{2}(x + 3)^2] (-1) - (3 - x) (2x^\frac{1}{2}) [2(x + 3)] + (x + 3)^2 (x^{-\frac{1}{2}})}{[2x^\frac{1}{2}(x + 3)^2]^2}$

---

## Example 3, cont.

3. Find the second derivative of $f(x) = \frac{\sqrt{x}}{x + 3}$
    * $f''(x) = \frac{[2x^\frac{1}{2}(x + 3)^2] (-1) - (3 - x) [(4x^\frac{1}{2})(x + 3) + (x + 3)^2 (x^{-\frac{1}{2}})]}{[2x^\frac{1}{2}(x + 3)^2]^2}$
    * $f''(x) = \frac{-x^{-\frac{1}{2}}(x + 3)[2x(x + 3) + 4x(3 - x) + (x + 3)(3 - x)]}{4x(x + 3)^4}$
    * $f''(x) = \frac{-[2x^2 + 6x + (12x - 4x^2) + 9 - x^2]}{4x^\frac{3}{2}(x + 3)^3}$
    * $f''(x) = \frac{3x^2 + 18x + 9}{4x^\frac{3}{2}(x + 3)^3}$
    * $f''(x) = \frac{3(x^2 + 6x + 3)}{4x^\frac{3}{2}(x + 3)^3}$
    
---

## Example 4

4. Given $f(x) = 12x^4 - 3x^2$, find $f''(-2)$
    * $\diff{x}^2 f(x) = \diff{x}^2 (12x^4 - 3x^2)$
    * $\diff{x}[\diff{x} f(x)] = \diff{x}[\diff{x} (12x^4 - 3x^2)]$
    * $\diff{x}[\diff{x} f(x)] = \diff{x}[\diff{x} (12x^4) - \diff{x} (3x^2)]$
    * $\diff{x} f'(x) = \diff{x}(48x^3 - 6x)$
    * $\diff{x} f'(x) = \diff{x} (48x^3) - \diff{x} (6x)$
    * $f''(x) = 144x^2 - 6$
    * $f''(-2) = 144(-2)^2 - 6$
    * $f''(-2) = 570$

---

## Exercise for Readers

* Find the second derivative of the following:
    * $f(x) = 3x^3 - 9x^2 + 16x - 5$
    * $f(x) = 10x$
    * $y = \frac{4x}{x - 7}$
    * $y = (3x^2 - 5)^3$
* Given the following, find $f''(-1)$
    * $f(x) = 7x^3 - 2x$
    * $f(x) = \frac{5x + 1}{x^2}$

---

# [Next Lesson](Lesson%207)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Find the second derivative of $f(x) = 3x^3 - 9x^2 + 16x - 5$
    * $\diff{x}^2 f(x) = \diff{x}^2 (3x^3 - 9x^2 + 16x - 5)$
    * $\diff{x}(\diff{x} f(x)) = \diff{x}[\diff{x} (3x^3 - 9x^2 + 16x - 5)]$
    * $\diff{x}(\diff{x} f(x)) = \diff{x}[\diff{x} (3x^3) - \diff{x} (9x^2) + \diff{x} (16x) - \diff{x} (5)]$
    * $\diff{x} f'(x) = \diff{x} (9x^2 - 18x + 16)$
    * $\diff{x} f'(x) = \diff{x} (9x^2) - \diff{x} (18x) + \diff{x} (16)$
    * $f''(x) = 18x - 18$ or $f''(x) = 18(x - 1)$

---

## Answers to Exercises, cont. 

* Find the second derivative of $f(x) = 10x$
    * $\diff{x}^2 f(x) = \diff{x}^2 (10x)$
    * $\diff{x} [\diff{x} f(x)] = \diff{x} (\diff{x} (10x))$
    * $\diff{x} f'(x) = \diff{x} (10)$
    * $f''(x) = 0$

---

## Answers to Exercises, cont. 

* Find the second derivative of $y = \frac{4x}{x - 7}$
    * $g(x) = 4x$
    * $h(x) = x - 7$
    * $\diff{x}^2 y = \diff{x} \frac{(x - 7) (\diff{x} (4x)) - (4x) (\diff{x} (x - 7))}{(x - 7)^2}$
    * $\diff{x} (\diff{x} y) = \diff{x} \frac{(x - 7) (\diff{x} (4x)) - (4x) (\diff{x} (x) - \diff{x} (7))}{(x - 7)^2}$
    * $\diff{x} \dd{y}{x} = \diff{x} \frac{4(x - 7) - 4x}{(x - 7)^2}$
    * $\diff{x} \dd{y}{x} = \diff{x} \frac{-28}{(x - 7)^2}$

---

## Answers to Exercises, cont. 

* Find the second derivative of $y = \frac{4x}{x - 7}$
    * $\diff{x} \dd{y}{x} = \diff{x} \frac{-28}{(x - 7)^2}$
    * $\diff{x} \dd{y}{x} = \diff{x} [-28(x - 7)^{-2}]$
    * $u = x - 7$
    * $\diff{u} (u^{-2}) [\diff{x} (x - 7)]$
    * $\diff{x} \dd{y}{x} = -28 [\diff{u} (u^{-2}) [\diff{x} (x - 7)]]$
    * $\diff{x} \dd{y}{x} = -28 [\diff{u} (u^{-2}) [\diff{x} (x) - \diff{x} (7)]]$

---

## Answers to Exercises, cont. 

* Find the second derivative of $y = \frac{4x}{x - 7}$
    * $u = x - 7$
    * $\diff{x} \dd{y}{x} = -28 [\diff{u} (u^{-2}) [\diff{x} (x) - \diff{x} (7)]]$
    * $\dd[2]{y}{x} = -28 [-2(x - 7)^{-3}]$
    * $\dd[2]{y}{x} = \frac{56}{(x - 7)^3}$


---

## Answers to Exercises, cont. 

* Find the second derivative of the following: $y = (3x^2 - 5)^3$
    * $u = 3x^2 - 5$
    * $\diff{x}^2 y = \diff{x} [\diff{u} u^3 (\diff{x} (3x^2 - 5))]$
    * $\diff{x} (\diff{x} y) = \diff{x} [\diff{u} u^3 (\diff{x} (3x^2) - \diff{x} (5))]$
    * $\diff{x} \dd{y}{x} = \diff{x} [18x (u^2)]$
    * $\diff{x} \dd{y}{x} = (18x) [\diff{u} (u^2) \diff{x} (3x^2 - 5)] + (3x^2 - 5)^2 [\diff{x} (18x)]$

---

## Answers to Exercises, cont. 

* Find the second derivative of the following: $y = (3x^2 - 5)^3$
    * $u = 3x^2 - 5$
    * $\diff{x} \dd{y}{x} = (18x) [\diff{u} (u^2) \diff{x} (3x^2 - 5)] + (3x^2 - 5)^2 [\diff{x} (18x)]$
    * $\diff{x} \dd{y}{x}$ = $(18x) [\diff{u} (u^2) \diff{x} (3x^2) - \diff{x}(5)] + (3x^2 - 5)^2 [\diff{x} (18x)]$
    * $\dd[2]{y}{x} = 18(3x^2 - 5)[12x^2 + 3x^2 - 5]$
    * $\dd[2]{y}{x} = 18(3x^2 - 5)[15x^2 - 5]$

---

## Answers to Exercises, cont. 

* Find the second derivative of the following: $y = (3x^2 - 5)^3$
    * $\dd[2]{y}{x} = 18(3x^2 - 5)[15x^2 - 5]$
    * $\dd[2]{y}{x} = 90(3x^2 - 5)(3x^2 - 1)$

---

## Answers to Exercises, cont. 

* Given the following, find $f''(-1)$: $f(x) = 7x^3 - 2x$
    * $\diff{x}^2 f(x) = \diff{x}^2 (7x^3 - 2x)$
    * $\diff{x}[\diff{x} f(x)] = \diff{x}[\diff{x} (7x^3 - 2x)]$
    * $\diff{x}[\diff{x} f(x)] = \diff{x}[\diff{x} (7x^3) - \diff{x} (2x)]$
    * $\diff{x} f'(x) = \diff{x} (21x^2 - 2)$
    * $\diff{x} f'(x) = \diff{x} (21x^2) - \diff{x} (2)$
    * $f''(x) = 42x^2$
    * $f''(-1) = 42(-1)^2$
    * $f''(-1) = 42$

---

## Answers to Exercises, cont. 

* Given the following, find $f''(-1)$: $f(x) = \frac{5x + 1}{x^2}$
    * $g(x) = 5x + 1$
    * $h(x) = x^2$
    * $\diff{x}^2 f(x) = \diff{x} \frac{(x^2) (\diff{x} (5x + 1)) - (5x + 1) (\diff{x} (x^2))}{(x^2)^2}$
    * $\diff{x}^2 f(x) = \diff{x} \frac{(x^2) [\diff{x} (5x) + \diff{x} (1)] - (5x + 1) [\diff{x} (x^2)]}{(x^2)^2}$
    * $\diff{x} f'(x) = \diff{x} \frac{5x^2 - 10x^2 + 2x}{x^4}$
    * $\diff{x} f'(x) = \diff{x} \frac{-5x^2 + 2x}{x^4}$
    * $\diff{x} f'(x) = \diff{x} \frac{(2 - 5x)}{x^3}$

---

## Answers to Exercises, cont. 

* Given the following, find $f''(-1)$: $f(x) = \frac{5x + 1}{x^2}$
    * $\diff{x} f'(x) = \diff{x} \frac{(2 - 5x)}{x^3}$
    * $g(x) = 2 - 5x$
    * $h(x) = x^3$
    * $\diff{x} f'(x) = \frac{(x^3) [\diff{x} (2 - 5x)] - (2 - 5x) (\diff{x} (x^3))}{(x^3)^2}$
    * $\diff{x} f'(x) = \frac{(x^3) [\diff{x} (2) - \diff{x} (5x)] - (2 - 5x) (\diff{x} (x^3))}{(x^3)^2}$
    * $f''(x) = \frac{15x^3 - 5x^3 - 6x^2}{(x^6)}$
    * $f''(x) = \frac{10x^3 - 6x^2}{x^6}$

---

## Answers to Exercises, cont. 

* Given the following, find $f''(-1)$: $f(x) = \frac{5x + 1}{x^2}$   
    * $f''(x) = \frac{10x^3 - 6x^2}{x^6}$
    * $f''(x) = \frac{x^2(10x - 6)}{x^6}$
    * $f''(x) = \frac{10x - 6}{x^4}$
    * $f''(-1) = \frac{10(-1) - 6}{(-1)^4}$
    * $f''(-1) = -(10 + 6)$
    * $f''(-1) = -16$

---

# [Next Lesson](Lesson%207)