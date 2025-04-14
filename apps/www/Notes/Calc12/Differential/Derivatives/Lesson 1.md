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

# Lesson 1: Differentials Using First Principles (Limits)

---

<!--paginate: true-->

## Intro 

* In the previous unit, you learned how to calculate the *Instantaneous Rate of Change* using this limit: $\limit{h}{0} \frac{f(x + h) - f(x)}{h}$
* This is so important to our studies that it has been given its own name: **The Derivative**. The act of finding these derivatives is known as **Differentiation**.

---

## A Note of Notation

* Due to the complex origins of Calculus, we'll be using a mixture of notations, including:
    * $\dd{x}f(x)$
    * $\dd[y]{x}$
    * $f'(x)$
    * $y'$
    * $\dot{x}$
    * $\diff{x} f(x)$

---

## Example 1

1. Find the derivative of the following function using first principles. Find the slope of the tangent at $P(4, 8)$ and write the equation of the tangent line.
* $f(x) = 2x^2 - 6x$
    * $f'(x) = \limit{h}{0} \frac{f(x + h) - f(x)}{h}$
    * $f'(x) = \limit{h}{0} \frac{2(x + h)^2 - 6(x + h) - (2x^2 - 6x)}{h}$

---

## Example 1, cont.

1. Find the derivative of the following function using first principles. Find the slope of the tangent at $P(4, 8)$ and write the equation of the tangent line.
    * $f'(x) = \limit{h}{0} \frac{2(x + h)^2 - 6(x + h) - (2x^2 - 6x)}{h}$
    * $f'(x) = \limit{h}{0} \frac{2x^2 + 4xh + 2h^2 - 6x - 6h - 2x^2 + 6x}{h}$
    * $f'(x) = \limit{h}{0} \frac{4xh + 2h^2 - 6h}{h}$

---

## Example 1, cont.

1. Find the derivative of the following function using first principles. Find the slope of the tangent at $P(4, 8)$ and write the equation of the tangent line.
    * $f'(x) = \limit{h}{0} \frac{4xh + 2h^2 - 6h}{h}$
    * $f'(x) = \limit{h}{0} \frac{h(4x + 2h - 6)}{h}$
    * $f'(x) = \limit{h}{0} (4x + 2h - 6)$
    * $f'(x) = 4x - 6$

---

## Example 1, cont.

1. Find the derivative of the following function using first principles. Find the slope of the tangent at $P(4, 8)$ and write the equation of the tangent line.
    * $f'(x) = 4x - 6$
    * The slope ($m$) can be found by substituting $x$ into the derivative.
    * $f'(4) = 4(4) - 6$
    * $f'(4) = 10$

---

## Example 1, cont.

1. Find the derivative of the following function using first principles. Find the slope of the tangent at $P(4, 8)$ and write the equation of the tangent line.
    * $f'(x) = 4x - 6$
    * $f'(4) = 10 = m$
    * $m = \frac{y_2 - y_1}{x_2 - x_1}$
    * $10 = \frac{y - 8}{x - 4}$
    * $y - 8 = 10(x - 4)$

---

## Example 2

2. Find the derivative of $y = \frac{1}{x^2}$ using first principles. Find the slope of the tangent at $P(2, \frac{1}{4})$ and write the equation of the tangent line.
    * $\dd[y]{x} = \limit{h}{0} \frac{f(x + h) - f(x)}{h}$
    * $\dd[y]{x} = \limit{h}{0} \frac{\frac{1}{(x + h)^2} - \frac{1}{x^2}}{h}$
    * $\dd[y]{x} = \limit{h}{0} \frac{\frac{x^2 - (x + h)^2}{x^2 (x + h)^2}}{h}$

---

## Example 2, cont.

2. Find the derivative of $y = \frac{1}{x^2}$ using first principles. Find the slope of the tangent at $P(2, \frac{1}{4})$ and write the equation of the tangent line.
    * $\dd[y]{x} = \limit{h}{0} \frac{\frac{x^2 - (x + h)^2}{x^2 (x + h)^2}}{h}$
    * $\dd[y]{x} = \limit{h}{0} \frac{x^2 - (x^2 + 2xh + h^2)}{h x^2 (x + h)^2}$
    * $\dd[y]{x} = \limit{h}{0} \frac{- 2xh - h^2}{h x^2 (x + h)^2}$

---

## Example 2, cont.

2. Find the derivative of $y = \frac{1}{x^2}$ using first principles. Find the slope of the tangent at $P(2, \frac{1}{4})$ and write the equation of the tangent line.
    * $\dd[y]{x} = \limit{h}{0} \frac{- 2xh - h^2}{h x^2 (x + h)^2}$
    * $\dd[y]{x} = \limit{h}{0} \frac{-h(2x + h)}{h x^2 (x + h)^2}$
    * $\dd[y]{x} = \limit{h}{0} \frac{-(2x + h)}{x^2 (x + h)^2}$

---

## Example 2, cont.

2. Find the derivative of $y = \frac{1}{x^2}$ using first principles. Find the slope of the tangent at $P(2, \frac{1}{4})$ and write the equation of the tangent line.
    * $\dd[y]{x} = \limit{h}{0} \frac{-(2x + h)}{x^2 (x + h)^2}$
    * $\dd[y]{x} = \frac{-2x}{x^2 x^2}$
    * $\dd[y]{x} = \frac{-2}{x^3}$

---

## Example 2, cont.

2. Find the derivative of $y = \frac{1}{x^2}$ using first principles. Find the slope of the tangent at $P(2, \frac{1}{4})$ and write the equation of the tangent line.
    * $\displaystyle\dd[y]{x} = \frac{-2}{x^3}$
    * $m = \frac{-1}{4}$
    * $-\frac{1}{4} = \frac{y - \frac{1}{4}}{x - 2}$
    * $\frac{1}{4}(2 - x) = y - \frac{1}{4}$

---

## Exercises for Readers

* Find the derivative using first principles:
    * $f(x) = 4x^2 - 7$
    * $y = 2x^3 - 6x$
    * $y = \frac{1}{x}$
    * $f(x) = \sqrt{3x + 1}$

---

# [Next Lesson](Lesson%202)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Find the derivative using first principles:
    * $f(x) = 4x^2 - 7$
        * $f'(x) = \limit{h}{0} \frac{f(x + h) - f(x)}{h}$
        * $f'(x) = \limit{h}{0} \frac{4(x + h)^2 - 7 - (4x^2 - 7)}{h}$
        * $f'(x) = \limit{h}{0} \frac{4(x^2 + 2xh + h^2) - 7 - 4x^2 + 7}{h}$
        * $f'(x) = \limit{h}{0} \frac{8xh + 4h^2}{h}$

---

## Answers to Exercises, cont

* Find the derivative using first principles:
    * $f(x) = 4x^2 - 7$
        * $f'(x) = \limit{h}{0} \frac{8xh + 4h^2}{h}$
        * $f'(x) = \limit{h}{0} \frac{h(8x + 4h)}{h}$
        * $f'(x) = \limit{h}{0} 8x + 4h$
        * $f'(x) = 8x$

---

## Answers to Exercises, cont

* Find the derivative using first principles:
    * $y = 2x^3 - 6x$
        * $\dd[y]{x} = \limit{h}{0} \frac{f(x + h) - f(x)}{h}$
        * $\dd[y]{x} = \limit{h}{0} \frac{2(x + h)^3 - 6(x + h) - (2x^3 - 6x)}{h}$
        * $\dd[y]{x} = \limit{h}{0} \frac{2(x^3 + 3x^2 h + 3xh^2 + h^3) - 6h - 2x^3}{h}$
        * $\dd[y]{x} = \limit{h}{0} \frac{6x^2 h + 6xh^2 + 2h^3 - 6h}{h}$

---

## Answers to Exercises, cont

* Find the derivative using first principles:
    * $y = 2x^3 - 6x$
        * $\dd[y]{x} = \limit{h}{0} \frac{6x^2 h + 6xh^2 + 2h^3 - 6h}{h}$
        * $\dd[y]{x} = \limit{h}{0} \frac{h(6x^2 + 6xh + 2h^2 - 6)}{h}$
        * $\dd[y]{x} = \limit{h}{0} 6x^2 + 6xh + 2h^2 - 6$
        * $\dd[y]{x} = 6x^2 - 6$

---

## Answers to Exercises, cont

* Find the derivative using first principles:
    * $y = \frac{1}{x}$
        * $\dd[y]{x} = \limit{h}{0} \frac{f(x + h) - f(x)}{h}$
        * $\dd[y]{x} = \limit{h}{0} \frac{\frac{1}{x + h} - \frac{1}{x}}{h}$
        * $\dd[y]{x} = \limit{h}{0} \frac{\frac{x - (x + h)}{x(x + h)}}{h}$

---

## Answers to Exercises, cont

* Find the derivative using first principles:
    * $y = \frac{1}{x}$
        * $\dd[y]{x} = \limit{h}{0} \frac{\frac{x - (x + h)}{x(x + h)}}{h}$
        * $\dd[y]{x} = \limit{h}{0} \frac{-1}{x(x + h)}$
        * $\dd[y]{x} = \frac{-1}{x^2}$

---

## Answers to Exercises, cont

* Find the derivative using first principles:    
    * $f(x) = \sqrt{3x + 1}$
        * $f'(x) = \limit{h}{0} \frac{f(x + h) - f(x)}{h}$
        * $f'(x) = \limit{h}{0} \frac{\sqrt{3(x + h) + 1} - \sqrt{3x + 1}}{h}$
        * $f'(x) = \limit{h}{0} \frac{3(x + h) + 1 - (3x + 1)}{h(\sqrt{3(x + h) + 1} + \sqrt{3x + 1})}$

---

## Answers to Exercises, cont

* Find the derivative using first principles:    
    * $f(x) = \sqrt{3x + 1}$
        * $f'(x) = \limit{h}{0} \frac{3(x + h) + 1 - (3x + 1)}{h(\sqrt{3(x + h) + 1} + \sqrt{3x + 1})}$
        * $f'(x) = \limit{h}{0} \frac{3x + 3h + 1 - 3x - 1}{h(\sqrt{3(x + h) + 1} + \sqrt{3x + 1})}$
        * $f'(x) = \limit{h}{0} \frac{3h}{h(\sqrt{3x + 3h + 1} + \sqrt{3x + 1})}$

---

## Answers to Exercises, cont

* Find the derivative using first principles:    
    * $f(x) = \sqrt{3x + 1}$
        * $f'(x) = \limit{h}{0} \frac{3}{\sqrt{3x + 3h + 1} + \sqrt{3x + 1}}$
        * $f'(x) = \frac{3}{2\sqrt{3x + 1}}$

---

# [Next Lesson](Lesson%202)