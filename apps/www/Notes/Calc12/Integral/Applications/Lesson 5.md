---
marp: true
theme: uncover
class: invert
math: mathjax
---

$\newcommand\diff[1]{\mathcal{d}_{#1}}$

# <!--fit--> Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2025-->

$\newcommand\dd[2][]{\displaystyle\frac{d#1}{d#2}}$

---

# Lesson 5: Volumes of Revolution

---

<!--paginate: true-->

## Intro

* Previously, we focused on methods for integrating functions.
* Now, we'll develop an application for the area under a curve using the following two points:
1. Rotating a two dimensional region about a line productes a three dimensional solid.
2. Any function can be broken down into smaller regions.

---

## Point 1

1. Rotating a two dimensional region about a line productes a three dimensional solid.
    * For example, if we have a rectangle and rotate (completely) around the x-axis, we obtain a cylindrical disk. 
    * It has a height of $y$, and let's say it has a width of $\Delta x$.
    * We know the volume of a cylinder is $V = \pi r^2 h$, and our radius is the height of the rectangle.
    * Therefore, $V = \pi y^2 \Delta x$.

---

## Point 2

2. Any function can be broken down into smaller regions.
    * We've seen this with the Riemann Sum!
    * Each of the rectangles produces a cylindrical disk, with the solid forming a Volume of Revolution.
    * If we sum the areas of the rectangles and rotate them around a given line, we can approximate the volume of the solid.

---

## The Volume of Revolution

* We can get a better approximation if we make the width smaller.
* If we create $n$ rectangles with width $\Delta x$, over an interval $[a, b]$ and let $n \to \infty$, then $\Delta x \to dx$.
* In this case, $y = f(x)$.
* Using our volume formula: $V(x_i) = \pi f^2(x_i) \Delta x_i$.
* Then, $\displaystyle V = \sum_{i = 1}^n \pi f^2(x_i) \Delta x_i$.
* Therefore, $V = \int_a^b \pi [f(x)]^2 dx$.

---

## Example 1

1. Consider a circle of radius 2 ($x^2 + y^2 = 4$). Find the volume of revolution of the top half ($y \ge 0$)
    * $y = \sqrt{4 - x^2}$
    * $0 \le \sqrt{4 - x^2}$
    * $x^2 \le 4$
    * $|x| \le 2 \implies x \in [-2, 2]$
    * $V = \int_{-2}^2 \pi (4 - x^2) dx$
    * $V = 2\pi \int_0^2 (4 - x^2) dx$
    * $V = 2\pi[4x - \frac{x^3}{3}]_0^2$

---

## Example 1, cont.

1. Consider a circle of radius 2 ($x^2 + y^2 = 4$). Find the volume of revolution of the top half ($y \ge 0$)
    * $V = 2\pi[4x - \frac{x^3}{3}]_0^2$
    * $V = 2\pi[4(2) - \frac{2^3}{3} - 4(0) + \frac{0^3}{3}]$
    * $V = 2\pi[\frac{(3 - 1)2^3}{3}]$
    * $V = \frac{2^5 \pi}{3}$
    * $V = \frac{32\pi}{3}$

---

## Example 2

2. Consider a circle of radius 2 ($x^2 + y^2 = 4$). Find the volume of revolution in Quadrant 1 ($x, y \ge 0$).
    * $V = \int_0^2 \pi (4 - x^2) dx$
    * $V = \pi [4x - \frac{x^3}{3}]_0^2$
    * $V = \pi [4(2) - \frac{2^3}{3}]$
    * $V = \pi \frac{(3 - 1)2^3}{3}$
    * $V = \frac{16 \pi}{3}$

---

## Example 3

3. Prove the answers are correct using the geometric formula for the volume of a sphere.
    * $V = \frac{4}{3}\pi r^3$
    * $V = \frac{2^2}{3}\pi 2^3$
    * $V = \frac{2^5 \pi}{3}$
    * $V = \frac{32\pi}{3}$
* This works for any regular solid (one we have a formula for).

---

## Exercise for Readers

* Find the volume of the solid rotated around the x axis over the given interval:
    * $f(x) = x^2, x \in [2, 3]$
    * $f(x) = \sec x, x \in [0, 45\degree]$ (convert to radians)
    * $y = 2, x \in [0, 3]$ (confirm using geometric formula)
    * $y = (x - 1)^2, x \in [0, 1]$
    * $y = (x - 1)^2, x \in [1, 2]$ (compare w/ above)
    * $y = \sqrt{x}, x \in [0, a], a = 2$

---

# [Next Lesson](Lesson%206)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Find the volume of $f(x) = x^2, x \in [2, 3]$
    * $V = \pi \int_2^3 (x^2)^2 dx$
    * $V = \pi \int_2^3 x^4 dx$
    * $V = \pi [\frac{x^5}{5}]_2^3$
    * $V = \pi\frac{3^5 - 2^5}{5}$
    * $V = \frac{211\pi}{5}$

---

## Answers to Exercises, cont.

* Find the volume of $f(x) = \sec x, x \in [0, 45\degree]$ (convert to radians)
    * $V = \pi \int_0^\frac{45\pi}{180} \sec^2 x dx$
    * $V = \pi \int_0^\frac{\pi}{4} \sec^2 x dx$
    * $V = \pi [\tan x]0^\frac{\pi}{4}$
    * $V = \pi (\tan \frac{\pi}{4} - \tan 0)$
    * $V = \pi$

---

## Answers to Exercises, cont.

* Find the volume of $y = 2, x \in [0, 3]$ (confirm using geometric formula)
    * $V = 4\pi \int_0^3 dx$
    * $V = 12\pi$
    * $V = \pi 2^2 (3)$
    * $V = 12\pi$

---

## Answers to Exercises, cont.

* Find the volume of $y = (x - 1)^2, x \in [0, 1]$
    * $V = \pi \int_0^1 [(x - 1)^2]^2 dx$
    * $V = \pi \int_0^1 (x - 1)^4 dx$
    * $V = \pi [\frac{(x - 1)^5}{5}]_0^1$
    * $V = \frac{\pi}{5}$

---

## Answers to Exercises, cont.

* Find the volume of $y = (x - 1)^2, x \in [1, 2]$ (compare w/ above)
    * $V = \pi [\frac{(x - 1)^5}{5}]_1^2$
    * $V = \frac{\pi}{5}$
    * *They're equal!*

---

## Answers to Exercises, cont.

* Find the volume of $y = \sqrt{x}, x \in [0, a], a = 2$
    * $V = \pi \int_0^a x dx$
    * $V = \pi [\frac{x^2}{2}]_0^a$
    * $V = \frac{a^2 \pi}{2}$
    * $V = 2\pi$

---

# [Next Lesson](Lesson%206)