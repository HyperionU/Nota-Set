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

# Lesson 4: Area Between Curves

---

<!--paginate: true-->

## Intro

* In this lesson, we'll expand our ability to find the area under a continuous function.
* Up until now, we've used the $x$-axis as our lower determining edge, but that may not always be the case.
* Now, let's learn how to determine the enclosed area between any two continuous functions in an interval.

---

## Example 1

1. Find the area enclosed by the functions $f(x) = x^2$ and $g(x) = \frac{x}{2}$ in the interval $[1, 2]$.
    * Method 1: Difference of Integrals
        * Determine the area between function $f$ and the $x$-axis in the interval $[1, 2]$
        * $A\{f(x)\} = \int_1^2 x^2 dx = \eval{(\frac{1}{3}x^3 + C)}{1}{2}$
        * $A\{f(x)\} = \frac{1}{3}(2)^3 - \frac{1}{3}(1)^3 = \frac{7}{3}$

---

## Example 1, cont.

1. Find the area enclosed by the functions $f(x) = x^2$ and $g(x) = \frac{x}{2}$ in the interval $[1, 2]$.
    * Method 1: Difference of Integrals
        * Determine the area between function $g$ and the $x$-axis in the interval $[1, 2]$
        * $A\{g(x)\} = \int_1^2 \frac{x}{2} dx = \eval{(\frac{1}{4}x^2 + C)}{1}{2}$
        * $A\{g(x)\} = \frac{1}{4}(2)^2 - \frac{1}{4}(1)^2 = \frac{3}{4}$
        * $A\{f(x), g(x)\} = \frac{7}{3} - \frac{3}{4}$
        * $A\{f(x), g(x)\} = \frac{19}{12}$

---

## Example 1, cont.

1. Find the area enclosed by the functions $f(x) = x^2$ and $g(x) = \frac{x}{2}$ in the interval $[1, 2]$.
    * Method 2: Integral of Difference Function
        * $\digamma(x) = f(x) - g(x)$
        * $\digamma(x) = x^2 - \frac{1}{2}x$
        * $A\{\digamma(x)\} = \int_1^2 \digamma(x) dx = \int_1^2 (x^2 - \frac{1}{2}x) dx$
        * $A\{\digamma(x)\} = \int_1^2 (x^2 - \frac{1}{2}x) dx = \eval{(\frac{1}{3}x^3 - \frac{1}{4}x^2)}{1}{2}$
        * $A\{\digamma(x)\} = (\frac{1}{3}(2)^3 - \frac{1}{4}(2)^2) - (\frac{1}{3}(1)^3 - \frac{1}{4}(1)^2)$
        * $A\{\digamma(x)\} = \frac{19}{12}$

---

## Curve Intersection

* In many cases, we aren't dealing with a simple case of one curve hovering over a lower curve for the entire interval.
* Sometimes, they intersect. 
* In order to deal with these possibilities it is useful to graph the two functions over the interval and see if we have intersection points.

---

## Curve Intersection, cont.

* Knowing where these graphs intersect and how they position themselves before and after these points allow us to continue solving our questions.
* Often, these points are part of the question. We are only interested in intersection points or discontinuities in the interval in question.

---

## Example 2

2. Determine the area enclosed by the functions $p(x) = x^2$ and $q(x) = x^3$ in the interval extending from the origin to the $x$-component of their point of intersection.
    * Determine the point(s) of intersection.
        * $p(x) = q(x)$
        * $x^2 = x^3$
        * $x^3 - x^2 = 0$
        * $x^2(x - 1) = 0$
        * $x = 0, x = 1$

---

## Example 2, cont.

2. Determine the area enclosed by the functions $p(x) = x^2$ and $q(x) = x^3$ in the interval extending from the origin to $x = 1$.
    * In the interval $[0, 1], p(x) \geq q(x)$.
    * $\digamma(x) = p(x) - q(x)$
    * $\digamma(x) = x^2 - x^3$
    * $A\{\digamma(x)\} = \int (x^2 - x^3) dx = \eval{(\frac{1}{3}x^3 - \frac{1}{4}x^4)}{0}{1}$
    * $A\{\digamma(x)\} = (\frac{1}{3}(1)^3 - \frac{1}{4}(1)^4) - (\frac{1}{3}(0)^3 - \frac{1}{4}(0)^4)$
    * $A\{\digamma(x)\} = \frac{1}{12}$

---

## Example 3

3. Determine the area enclosed by the $y$- axis and the functions $f(x) = \tan x$ and $g(x) = 2 - x^3$
    * $\tan x = 2 - x^3$
    * $2 - x^3 - \tan x = 0$
    * $x \approx \frac{9}{10}$ (by technology)
    * $A\{f(x), g(x)\} = \int_0^\frac{9}{10} (2 - x^3 - \tan x) dx$
    * $A\{f(x), g(x)\} \approx 1.16$

---

## Exercise for Readers

* Find the area of the region between the given curves over the indicated interval. If there are intersection points, indicate them.
    * $f(x) = x^2$ and $g(x) = 1$ in quadrant 1.
    * $f(x) = x^2$ and $g(x) = 1$ between both intersection points.
    * $y = -x^2 + 4$ and $y = -2x$ for any area bounded between the curves and the $y$-axis (as a right-hand boundary)

---

## Exercise for Readers, cont.

* Find the area of the region between the given curves over the indicated interval. If there are intersection points, indicate them.
    * $y = x^2 - 4$, above the $x$-axis and the line $x = 4$.
    * $y = \sin x$ and $y = \cos x$ between the $y$-axis and $\frac{\pi}{4}$ radians along the positive $x$-axis.
    * $y = x^3 - 3x^2 + x + 4, y = -x^2 + 4x + 4$ and the $y$-axis in Quadrant I.

---

# [Next Lesson](Lesson%205)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercise

* Find the area of the region between $f(x) = x^2$ and $g(x) = 1$ in quadrant 1. If there are intersection points, indicate them.
    * $x \geq 0$
    * $f(x) = g(x)$
    * $x^2 = 1$
    * $x^2 - 1 = 0$
    * $(x - 1)(x + 1) = 0$
    * $x = 1$

---

## Answers to Exercise, cont.

* Find the area of the region between $f(x) = x^2$ and $g(x) = 1$ in quadrant 1. If there are intersection points, indicate them.
    * $\digamma(x) = g(x) - f(x)$
    * $\digamma(x) = 1 - x^2$
    * $A\{\digamma(x)\} = \int_0^1 (1 - x^2)dx = \eval{(x - \frac{1}{3}x^3)}{0}{1}$
    * $A\{\digamma(x)\} = \eval{(x - \frac{1}{3}x^3)}{0}{1} = (1 - \frac{1}{3}1^3) - (0 - \frac{1}{3}0^3)$
    * $A\{\digamma(x)\} = \frac{2}{3}$

---

## Answers to Exercise, cont.

* Find the area of the region between $f(x) = x^2$ and $g(x) = 1$ between both intersection points. Indicate them.
    * $f(x) = g(x)$
    * $x^2 = 1$
    * $x^2 - 1 = 0$
    * $(x - 1)(x + 1) = 0$
    * $x = \pm 1$

---

## Answers to Exercise, cont.

* Find the area of the region between $f(x) = x^2$ and $g(x) = 1$ between both intersection points. Indicate them.
    * $\digamma(x) = g(x) - f(x)$
    * $\digamma(x) = 1 - x^2$
    * $A\{\digamma(x)\} = \int_{-1}^1 (1 - x^2)dx = \int_0^1 (1 - x^2)dx$
    $A\{\digamma(x)\} = 2\int_0^1 (1 - x^2)dx = 2 [\eval{(x - \frac{1}{3}x^3)}{0}{1}]$
    * $A\{\digamma(x)\} = 2[\eval{(x - \frac{1}{3}x^3)}{0}{1}] = 2[(1 - \frac{1}{3}1^3) - (0 - \frac{1}{3}0^3)]$
    * $A\{\digamma(x)\} = \frac{4}{3}$

---

## Answers to Exercise, cont.

* Find the area of the region between $y = -x^2 + 4$ and $y = -2x$ for any area bounded between the curves and the $y$-axis (as a right-hand boundary). If there are intersection points, indicate them.
    * $x \leq 0$
    * $4 - x^2 = -2x$
    * $-x^2 + 2x + 4 = 0$
    * $x = \frac{-2 \pm \sqrt{2^2 - 4(-1)(4)}}{2(-1)}$
    * $x = \frac{-2 \pm \sqrt{20}}{-2}$

---

## Answers to Exercise, cont.

* Find the area of the region between $y = -x^2 + 4$ and $y = -2x$ for any area bounded between the curves and the $y$-axis (as a right-hand boundary). If there are intersection points, indicate them.
    * $x \leq 0$
    * $x = \frac{-2 \pm \sqrt{20}}{-2}$
    * $x = 1 \mp \frac{\sqrt{20}}{2}$
    * $x = 1 - \frac{\sqrt{20}}{2}$

---

## Answers to Exercise, cont.

* Find the area of the region between $y = -x^2 + 4$ and $y = -2x$ for any area bounded between the curves and the $y$-axis (as a right-hand boundary). If there are intersection points, indicate them.
    * $\digamma(x) = -x^2 + 2x + 4$
    * $A\{\digamma(x)\} = \int_{1 - \frac{\sqrt{20}}{2}}^0 (-x^2 + 2x + 4) dx$
    * $A\{\digamma(x)\} = \eval{(-x^2 + 2x + 4)}{1 - \frac{\sqrt{20}}{2}}{0}$
    * $A\{\digamma(x)\} = [-(0)^2 + 2(0) + 4] -$ $[-(1 - \frac{\sqrt{20}}{2})^2 + 2(1 - \frac{\sqrt{20}}{2}) + 4]$

---

## Answers to Exercise, cont.

* Find the area of the region between $y = -x^2 + 4$ and $y = -2x$ for any area bounded between the curves and the $y$-axis (as a right-hand boundary). If there are intersection points, indicate them.
    * $A\{\digamma(x)\} = [-(0)^2 + 2(0) + 4] -$ $[-(1 - \frac{\sqrt{20}}{2})^2 + 2(1 - \frac{\sqrt{20}}{2}) + 4]$
    * $A\{\digamma(x)\} = 4 - [-(6 - \sqrt{20}) + (2 - \sqrt{20}) + 4]$
    * $A\{\digamma(x)\} = 4 + (6 - \sqrt{20}) - (2 - \sqrt{20}) - 4$
    * $A\{\digamma(x)\} = 4$

---

## Answers to Exercise, cont.

* Find the area of the region between $y = x^2 - 4$, above the $x$-axis and the line $x = 4$. If there are intersection points, indicate them.
    * $x^2 - 4 = 0$
    * $x^2 = 4$
    * $x = \pm 2$
    * $A\{y\} = \int_2^4 (x^2 - 4) dx = \eval{(\frac{1}{3}x^3 - 4x)}{2}{4}$
    * $A\{y\} = \eval{(\frac{1}{3}x^3 - 4x)}{2}{4} = (\frac{1}{3}(4)^3 - 4(4)) - (\frac{1}{3}(2)^3 - 4(2))$
    * $A\{y\} = (\frac{1}{3}(4)^3 - 4(4)) - (\frac{1}{3}(2)^3 - 4(2))$

---

## Answers to Exercise, cont.

* Find the area of the region between $y = x^2 - 4$, above the $x$-axis and the line $x = 4$. If there are intersection points, indicate them.
    * $A\{y\} = \eval{(\frac{1}{3}x^3 - 4x)}{2}{4} = (\frac{1}{3}(4)^3 - 4(4)) - (\frac{1}{3}(2)^3 - 4(2))$
    * $A\{y\} = (\frac{1}{3}(4)^3 - 4(4)) - (\frac{1}{3}(2)^3 - 4(2))$
    * $A\{y\} = \frac{4^3 - 3(4^2)}{3} + \frac{3(8) - 8}{3}$
    * $A\{y\} = \frac{4^2}{3} + \frac{2^4}{3}$
    * $A\{y\} = \frac{2^4 + 2^4}{3}$
    * $A\{y\} = \frac{2^5}{3}$

---

## Answers to Exercise, cont.

* Find the area of the region between $y = x^2 - 4$, above the $x$-axis and the line $x = 4$. If there are intersection points, indicate them.
    * $A\{y\} = \frac{2^4 + 2^4}{3}$
    * $A\{y\} = \frac{2^5}{3}$
    * $A\{y\} = \frac{32}{3}$

---

## Answers to Exercise, cont.

* Find the area of the region between $y = \sin x$ and $y = \cos x$ between the $y$-axis and $\frac{\pi}{4}$ radians along the positive $x$-axis. If there are intersection points, indicate them.
    * $x = \frac{\pi}{4}$
    * $\digamma(x) = \cos x - \sin x$
    * $A\{\digamma(x)\} = \int_0^\frac{\pi}{4} (\cos x - \sin x) dx = \eval{(\sin x + \cos x)}{0}{\frac{\pi}{4}}$
    * $A\{\digamma(x)\} = \eval{(\sin x + \cos x)}{0}{\frac{\pi}{4}} = (\sin \frac{\pi}{4} + \cos \frac{\pi}{4})$ $- (\sin 0 + \cos 0)$

---

## Answers to Exercise, cont.

* Find the area of the region between $y = \sin x$ and $y = \cos x$ between the $y$-axis and $\frac{\pi}{4}$ radians along the positive $x$-axis. If there are intersection points, indicate them.
    * $A\{\digamma(x)\} = \eval{(\sin x + \cos x)}{0}{\frac{\pi}{4}} = (\sin \frac{\pi}{4} + \cos \frac{\pi}{4})$ $- (\sin 0 + \cos 0)$
    * $A\{\digamma(x)\} = (\sin \frac{\pi}{4} + \cos \frac{\pi}{4}) - (\sin 0 + \cos 0)$
    * $A\{\digamma(x)\} = (\frac{1}{\sqrt{2}} + \frac{1}{\sqrt{2}}) - 1$
    * $A\{\digamma(x)\} = \sqrt{2} - 1$

---

## Answers to Exercise, cont.

* Find the area of the region between $y = x^3 - 3x^2 + x + 4, y = -x^2 + 4x + 4$ and the $y$-axis in Quadrant I. If there are intersection points, indicate them.
    * $x \geq 0$
    * $x^3 - 3x^2 + x + 4 = -x^2 + 4x + 4$
    * $x^3 - 2x^2 - 3x = 0$
    * $x(x^2 - 2x - 3) = 0$
    * $x(x - 3)(x + 1) = 0$
    * $x = 0, 3$

---

## Answers to Exercise, cont.

* Find the area of the region between $y = x^3 - 3x^2 + x + 4, y = -x^2 + 4x + 4$ and the $y$-axis in Quadrant I. If there are intersection points, indicate them.
    * $\digamma(x) = x^3 - 3x^2 + x + 4 - (-x^2 + 4x + 4)$
    * $\digamma(x) = x^3 - 2x^2 - 3x$
    * $A\{\digamma(x)\} = \int_0^3 (x^3 - 2x^2 - 3x)dx =$ $\eval{(\frac{1}{4}x^4 - \frac{2}{3}x^3 - \frac{3}{2}x^2)}{0}{3}$
    * $A\{\digamma(x)\} = \eval{(\frac{1}{4}x^4 - \frac{2}{3}x^3 - \frac{3}{2}x^2)}{0}{3}$

---

## Answers to Exercise, cont.

* Find the area of the region between $y = x^3 - 3x^2 + x + 4, y = -x^2 + 4x + 4$ and the $y$-axis in Quadrant I. If there are intersection points, indicate them.
    * $A\{\digamma(x)\} = \eval{(\frac{1}{4}x^4 - \frac{2}{3}x^3 - \frac{3}{2}x^2)}{0}{3}$
    * $A\{\digamma(x)\} = (\frac{1}{4}(3)^4 - \frac{2}{3}(3)^3 - \frac{3}{2}(3)^2)$
    * $A\{\digamma(x)\} = \frac{81}{4} - 18 - \frac{27}{2}$
    * $A\{\digamma(x)\} = -\frac{45}{4}$

---

# [Next Lesson](Lesson%205)