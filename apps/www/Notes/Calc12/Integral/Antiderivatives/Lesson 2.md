---
marp: true
theme: uncover
class: invert
math: mathjax
---

$\newcommand\diff[1]{\mathcal{d}_{#1}}$
$\newcommand\eval[3]{\left. #1 \right|_{#2}^{#3}}$

# <!--fit--> Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2025-->

$\newcommand\dd[2][]{\displaystyle\frac{d#1}{d#2}}$
$\newcommand\limit[2]{\displaystyle\lim_{#1 \to #2}}$

---

# Lesson 2: Signed Area

---

<!--paginate: true-->

## Intro

* Let's say we need to calculate the signed area under a curve within a boundary (denoted by $a$ and $b$).
* We can look at what this is for a few simple curves, then look at more complex curves.

---

## The Basics

* Consider the function $y = x$.
* What is the area between the origin and $x = 2$?
* We can state these boundaries using Interval Notation ($x \in [a, b], x \in [0, 2]$), or some other similar fashion.
* We can note that this is a triangle with a base of two and a height of two.
* This means that $A = \frac{1}{2} bh$, which we can simplify to $A = \frac {1}{2} 2^2 = 2$.
* This looks familiar. ($A = \frac{x^2}{2}, x = 2, A = 2$)

---

## Area Under Curve

* We know that the area under the curve $f(x) = x$ from the origin to $x = 2$ is exactly 2 units squared.
* We also know that the area could have been found using the antiderivative of the function at this point.
* Maybe, we could use this!

---

## Example 1

1. Consider $f(x) = x$. What is the signed area under the curve between $x = 2$ and $x = 3$,
    * using a geometric formula?
        * $A = (3 - 2)[\frac{f(2) + f(3)}{2}]$
        * $A = \frac{2 + 3}{2}$
        * $A = \frac{5}{2}$
    * What is the general formula?
        * $A(x) = (x - 2)[\frac{f(2) + f(x)}{2}]$
        * $A(x) = \frac{1}{2}(x - 2)(2 + x)$

---

## Example 1, cont.

1. Consider $f(x) = x$. What is the signed area under the curve between $x = 2$ and $x = 3$,
    * What is the general formula?
        * $A(x) = \frac{1}{2}(x - 2)(2 + x)$
        * $A(x) = \frac{x^2}{2} - 2$
    * using a general formula?
        * $A(3) = \frac{3^2}{2} - 2$
        * $A(3) = \frac{9}{2} - \frac{4}{2}$
        * $A(3) = \frac{5}{2}$

---

## Example 1, cont.

1. Consider $f(x) = x$. What is the signed area under the curve between $x = 2$ and $x = 3$,
    * What is the general formula?
        * $A(x) = \frac{1}{2}(x - 2)(2 + x)$
        * $A(x) = \frac{x^2}{2} - 2$
* If we change the left boundary, it would simply change the constant of integration in the antiderivative function.
* Does this constant matter? In this case, **No.**

---

## Using Antiderivatives

* If we used the general antiderivative function and we know the left and right hand values, we can substitute the values into the function.
* This gives us two areas: The area from some x-value to the left hand boundary, and the total area under the curve from some x-value to the right hand boundary.
* Then, we could subtract the two areas to get the area between the left and right boundaries.

---

## Using Antiderivatives, cont.

* Using our example of $f(x) = x$, our $A(x) = \frac{x^2}{2} + C$.
* The signed area between the x-axis and our function on the interval $[2, 3]$ is simply as follows: 
* $\eval{(\frac{x^2}{2} + C)}{2}{3}$
* $A(3) - A(2)$
* $(\frac{3^2}{2} + C) - (\frac{2^2}{2} + C)$
* $\frac{5}{2}$ ($C$ is unimportant since it cancels by substitution.)

---

## Key to Signed Area

* Given that a function $y = f(x)$ is continuous over an interval $[a, b]$, the signed area under $f(x)$ can be found using the general antiderivative $A(x)$.
* Furthermore, the area of a right hand region less the area of the left hand region gives the signed area over the desired interval: $A(b) - A(a)$.
* *Take note of this, this will be important later.*

---

## Example 2

2. Determine the signed area between the $x$-axis and the function $f(x) = x$ in the interval $[-2, -1]$. Determine a formula for the signed area.
    * $A = (-1 - (-2))[\frac{f(-1) + f(-2)}{2}]$
    * $A = \frac{-1 + (-2)}{2}$
    * $A = -\frac{3}{2}$
* For the interval $[-2, x]$:
    * $A(x) = (x - (-2))[\frac{f(-2) + f(x)}{2}]$
    * $A(x) = (x + 2)[\frac{-2 + x}{2}]$

---

## Example 2, cont.

2. Determine the signed area between the $x$-axis and the function $f(x) = x$ in the interval $[-2, -1]$. Determine a formula for the signed area.
* For the interval $[-2, x]$:
    * $A(x) = (x + 2)[\frac{-2 + x}{2}]$
    * $A(x) = \frac{x^2 - 4}{2}$
    * $A(x) = \frac{1}{2}x^2 - 2$
* Using $A(x) = \frac{1}{2}x^2 - 2$: $A(-1) = \frac{1}{2}(-1)^2 - 2$
    * $A(-1) = -\frac{3}{2}$

---

## Example 2, cont.

2. Determine the signed area between the $x$-axis and the function $f(x) = x$ in the interval $[-2, -1]$. Determine a formula for the signed area.
* Another option is to find the antiderivative $A(x) = \frac{1}{2}x^2 + C$, then calculate $A(-1) - A(-2)$. 
* The change is then the accumulated signed area.
    * $\eval{(\frac{1}{2}x^2 + C)}{-2}{-1}$
    * $A(-1) - A(-2)$

---

## Example 2, cont.

2. Determine the signed area between the $x$-axis and the function $f(x) = x$ in the interval $[-2, -1]$. Determine a formula for the signed area.
    * $[\frac{1}{2}(-1)^2 + C] - [\frac{1}{2}(-2)^2 + C]$
    * $\frac{1}{2} - \frac{4}{2}$
    * $-\frac{3}{2}$
* The result is negative because the area is below the $x$-axis.

---

## Example 3

3. Given $f(x) = x + 1$, find the signed area in the interval $[1, x]$, create a general formula, and determine the signed area in the interval $[1, 4]$
    * $A(x) = (x - 1)[\frac{2 + (x + 1)}{2}]$
    * $A(x) = (x - 1)[\frac{x + 3}{2}]$
    * $A(x) = \frac{1}{2}(x^2 + 2x - 3)$
    * $A(x) = \frac{x^2}{2} + x - \frac{3}{2}$
    * $A(4) = \frac{4^2}{2} + 4 - \frac{3}{2}$
    * $A(4) = \frac{21}{2}$

---

## Proving Signed Area = Antiderivative

* At this point, you might wonder why this is the case. Here's a proof why:
* **Theorem:** For a given function $y = f(x)$, $A(x) = \int f(x)$
* **Proof:**
    * Assume that $f(x)$ is continuous along an interval $[a, b]$. Let $A(x)$ be the area in the interval $[0, x]$.
    * Let $b = x + \Delta x, a = x$.

---

## Proving Signed Area = Antiderivative, cont.

* **Theorem:** For a given function $y = f(x)$, $A(x) = \int f(x)$
* **Proof:**
    * Assume that $f(x)$ is continuous along an interval $[a, b]$. 
    * Let $A(x)$ be the area in the interval $[0, x], b = x + \Delta x, a = x$.
    * Therefore, $A'(x) = \limit{\Delta x}{0} \frac{\Delta A}{\Delta x}$.

---

## Proving Signed Area = Antiderivative, cont.

* **Theorem:** For a given function $y = f(x)$, $A(x) = \int f(x)$
* **Proof (cont.):**
    * Let $A(x)$ be the area in the interval $[0, x], b = x + \Delta x, a = x$.
    * Since $A'(x) = \limit{\Delta x}{0} \frac{\Delta A}{\Delta x}$, $\therefore A'(x) = \limit{\Delta x}{0} \frac{A(b) - A(a)}{\Delta x} = \limit{\Delta x}{0} \frac{A(x + \Delta x) - A(x)}{\Delta x}$

---

## Proving Signed Area = Antiderivative, cont.

* **Theorem:** For a given function $y = f(x)$, $A(x) = \int f(x)$
* **Proof (cont.):**
    * Since $A'(x) = \limit{\Delta x}{0} \frac{\Delta A}{\Delta x}$, and given $\Delta A = \frac{1}{2}(\Delta x)[f(a) + f(b)]$, $\therefore A'(x) = \limit{\Delta x}{0} \frac{\frac{1}{2}(\Delta x)[f(a) + f(b)]}{\Delta x}$

---

## Proving Signed Area = Antiderivative, cont.

* **Theorem:** For a given function $y = f(x)$, $A(x) = \int f(x)$
* **Proof (cont.):**
    * Since $A'(x) = \limit{\Delta x}{0} \frac{\frac{1}{2}(\Delta x)[f(a) + f(b)]}{\Delta x}$, and that $a = x, b = x + \Delta x$, $\therefore A'(x) = \limit{\Delta x}{0} \frac{\frac{1}{2}(\Delta x)[f(x) + f(x + \Delta x)]}{\Delta x}$

---

## Proving Signed Area = Antiderivative, cont.

* **Theorem:** For a given function $y = f(x)$, $A(x) = \int f(x)$
* **Proof (cont.):**
    * $A'(x) = \limit{\Delta x}{0} \frac{\frac{1}{2}(\Delta x)[f(x) + f(x + \Delta x)]}{\Delta x}$
    * $A'(x) = \limit{\Delta x}{0} \frac{f(x) + f(x + \Delta x)}{2}$
    * $A'(x) = \frac{f(x) + f(x)}{2}$
    * $A'(x) = f(x)$

---

## Proving Signed Area = Antiderivative, cont.

* **Theorem:** For a given function $y = f(x)$, $A(x) = \int f(x)$
* **Proof (cont.):** Since $A'(x) = f(x)$, $\therefore \int \diff{x} (A(x)) = \int f(x)$
* $\therefore A(x) = \int f(x) \blacksquare$.
* Therefore, for any function $f(x)$, the signed area between the function and the $x$-axis is the antiderivative of the original function.

---

## Example 4

4. Find the signed area under $y = \cos x$ for the interval $[0, \frac{\pi}{2}]$.
    * $f(x) = \cos x$
    * $A(x) = \int \cos x dx = \sin x + C$
    * $A = \eval{(\sin x + C)}{0}{\frac{\pi}{2}} = A(\frac{\pi}{2}) - A(0)$
    * $A = [\sin \frac{\pi}{2} + C] - [\sin 0 + C]$
    * $A = \sin \frac{\pi}{2} - \sin 0$
    * $A = 1$

---

## Exercise for Readers

* Find the signed areas for the given intervals:
    * $f(x) = \frac{1}{x}, [1, 3]$
    * $f(x) = \sin x, [0, \pi]$
    * $\frac{f(x)}{2} = x^2 - 1, [2, 3]$
    * $f(x) = \frac{2 \sqrt{x}}{3}, [1, 4]$
    * $f(x) = x^2 - 4x, [0, 3]$
    * $f(x) = e^x, [0, 1]$

---

# [Next Lesson](Lesson%203)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercise

* Find the signed area for the given interval: $f(x) = \frac{1}{x}, [1, 3]$
    * $A(x) = \int \frac{1}{x} dx = \ln |x| + C$
    * $A = \eval{(\ln |x| + C)}{1}{3} = A(3) - A(1)$
    * $A = \ln 3 - \ln 1$
    * $A = \ln 3$

---

## Answers to Exercise, cont.

* Find the signed area for the given interval: $f(x) = \sin x, [0, \pi]$
    * $A(x) = \int \sin x dx$
    * $A = \eval{(-\cos x)}{0}{\pi} = A(\pi) - A(0)$
    * $A = (\cos 0) - (\cos \pi)$
    * $A = 1 - (-1)$
    * $A = 2$

---

## Answers to Exercise, cont.

* Find the signed area for the given interval: $\frac{f(x)}{2} = x^2 - 1, [2, 3]$
    * $A(x) = 2 \int x^2 - 1 dx = 2(\frac{1}{3}x^3 - x) = \frac{2}{3}x^3 - 2x$
    * $A = \eval{(\frac{2}{3}x^3 - 2x)}{2}{3} = A(3) - A(2)$
    * $A = (\frac{2}{3}(3^3) - 2(3)) - (\frac{2}{3}(2^3) - 2(2))$
    * $A = 12 - \frac{4}{3}$
    * $A = \frac{32}{3}$

---

## Answers to Exercise, cont.

* Find the signed area for the given interval: $f(x) = \frac{2 \sqrt{x}}{3}, [1, 4]$
    * $A(x) = \frac{2}{3} \int x^\frac{1}{2} dx = \frac{4}{9}x^\frac{3}{2}$
    * $A = \eval{(\frac{4}{9}x^\frac{3}{2})}{1}{4} = A(4) - A(1)$
    * $A = (\frac{4}{9}(4)^\frac{3}{2}) - (\frac{4}{9}(1)^\frac{3}{2})$
    * $A = \frac{12}{9} - \frac{4}{9}$
    * $A = \frac{8}{9}$

---

## Answers to Exercise, cont.

* Find the signed area for the given interval: $f(x) = x^2 - 4x, [0, 3]$
    * $A(x) = \int x^2 - 4x dx = \frac{1}{3} x^3 - 2x^2$
    * $A = \eval{(\frac{1}{3}x^3 - 2x^2)}{0}{3} = A(3) - A(0)$
    * $A = (\frac{1}{3}(3^3) - 2(3^2)) - (\frac{1}{3}(0^3) - 2(0^2))$
    * $A = -9$

---

## Answers to Exercise, cont.

* Find the signed area for the given interval: $f(x) = e^x, [0, 1]$
    * $A(x) = \int e^x dx = e^x$
    * $A = \eval{e^x}{0}{1} = A(1) - A(0)$
    * $A = e^1 - e^0$
    * $A = e - 1$

---

# [Next Lesson](Lesson%203)