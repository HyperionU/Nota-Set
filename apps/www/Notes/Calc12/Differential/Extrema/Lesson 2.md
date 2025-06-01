---
marp: true
theme: uncover
class: invert
math: mathjax
---

$\newcommand\odd{\mathbb{O}[f(x)]}$

# <!--fit--> Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2025-->

$\newcommand\even{\mathbb{E}[f(x)]}$

---

# Lesson 2: Symmetry of Functions

---

<!--paginate: true-->

## Intro 

* When sketching graphs of functions, it's very useful to know its symmetry.
* For example, if a curve is symmetric about the $y$-axis, you'd only need to find the various aspects for the intervals $(-\infty, 0)$ or $(0, \infty)$, since the rest is just reflected in the $y$-axis.

---

## Even Functions

* Take for example the graph of $f(x) = x^4 - 18x^2 - 19$.
* All of the features of the graph to the left of the $y$-axis are duplicated in the reflection on the right.
* Functions which are symmetric about the $y$-axis are called *Even Functions*.
* To determine if $y = f(x)$ is even, you must find $y = f(-x)$, and if $f(x) = f(-x)$, then $f(x)$ is even.

---

## Example 1

1. Determine if the function $f(x) = 2x - 5$ is even.
    * Assume $f(x) = f(-x)$
    * $f(-x) = 2(-x)^2 - 5$
    * $f(-x) = 2x^2 - 5$
    * $2x^2 - 5 = 2x^2 - 5$ (*Our assumption holds!*)
    * $f(x) = f(-x) \therefore f(x) \in \even$ and is symmetrical around the $y$-axis.
* Note: To make it easier, I'm using $\even$ to represent even functions.

---

## Example 2

2. Is $f(x) = x^3 - 2x + 4$ symmetric about the $y$-axis?
    * Assume $f(x) = f(-x)$
    * $f(-x) = (-x)^3 - 2(-x) + 4$
    * $f(-x) = -x^3 + 2x + 4$
    * $x^3 - 2x + 4 = -x^3 + 2x + 4$ (*Our assumption doesn't hold!*)
    * $f(x) \ne f(-x) \therefore f(x) \not\in \even$ and isn't symmetrical around the $y$-axis.

---

## Odd Functions

* Take for example the graph of $y = x^3 - 20x$.
* The graph is identical if we rotate the graph around the origin by 180 degrees.
* Functions which are symmetric about the origin are called *Odd Functions*.
* To determine if $y = f(x)$ is off, you must find $y = f(-x)$ and $y = -f(x)$, and if $-f(x) = f(-x)$, then $f(x)$ is odd.

---

## Example 3

3. Is $f(x) = x^4 - 2x$ odd?
    * $f(-x) = (-x)^4 - 2(-x)$
    * $f(-x) = x^4 + 2x$
    * $-f(x) = -[x^4 - 2x]$
    * $-f(x) = -x^4 + 2x$
    * $-f(x) \ne f(-x) \therefore f(x) \not\in \odd$.
* Note: To make it easier, I'm using $\odd$ to represent odd functions.

---

## Example 4

4. Is $f(x) = \cos x - \sin x$ odd?
* Note: $\cos x \in \even \therefore \cos x = \cos (-x)$
    * Assume $f(-x) = -f(x)$
    * $f(-x) = \cos(-x) - \sin(-x)$
    * $f(-x) = \cos(x) - \sin(-x)$
    * $-f(x) = -\cos(x) + \sin(x)$
    * $\cos(x) - \sin(-x) = -\cos(x) + \sin(x)$ (*Our assumption doesn't hold!*)
    * $-f(x) \ne f(-x) \therefore f(x) \not\in \odd$.

---

## Example 5

5. Determine if $f(x) = \frac{1}{2}x^5$ is even, odd, or neither.
    * Assume $f(x) = f(-x)$
    * $f(-x) = \frac{1}{2}(-x)^5$
    * $f(-x) = -\frac{1}{2}x^5$ (*Not even.*)
    * $f(x) \ne f(-x) \therefore f(x) \not\in \even$.
    * Assume $-f(x) = f(-x)$
    * $-f(x) = -\frac{1}{2}x^5$
    * $-f(x) \ne f(-x) \therefore f(x) \not\in \odd$.

---

## A Quick Shortcut

* Here's some quick shortcuts to determine if a function is even / odd:
    * $\cos x \in \even$
    * $\sin x \in \odd$
    * All polynomial terms of odd degree are odd.
    * All polynomial terms of even degree are even.
    * $\even \pm \odd = \emptyset$
    * $\even \pm \even = \even$
    * $\odd \pm \odd = \odd$

---

## Exercise for Readers

* Determine if the following are even:
    * $y = 4x^2 - 3$
    * $f(x) = 2x^3 + 3x - 1$
    * $y = 4x^4 + 2x - 1$
    * $y = 2\cos x + 3$
* Determine if the following are odd:
    * $y = 3x^3$
    * $y = 4x^2 - x$
    * $f(x) = 2x^3 + 5x$
    * $y = \frac{1}{2}\sin 2x$   

---

## Exercise for Readers

* Determine what type of symmetry, if any, the following have:
    * $y = 3x^2 - 5$
    * $y = 2x^3 + 7x$
    * $y = x^3 + x^2$
    * $y = 4\sin x \cos x$

---

# [Next Lesson](Lesson%203)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Determine if $y = 4x^2 - 3$ is even.
    * $4x^2 - 3 \in \even$
    * $f(-x) = 4(-x)^2 - 3$
    * $f(-x) = 4x^2 - 3$
    * $y = f(-x) \therefore y \in \even$

---

## Answers to Exercises, cont.

* Determine if $f(x) = 2x^3 + 3x - 1$ is even.
    * $f(x) = 2x^3 + 3x - 1 \not\in \even$
    * $f(-x) = 2(-x)^3 + 3(-x) - 1$
    * $f(-x) = -2x^3 - 3x - 1$
    * $f(x) \ne f(-x) \therefore f(x) \not\in \even$

---

## Answers to Exercises, cont.

* Determine if $y = 4x^4 + 2x - 1$ is even.
    * $4x^4 + 2x - 1 \not\in \even$
    * $f(-x) = 4(-x)^4 + 2(-x) - 1$
    * $f(-x) = 4x^4 - 2x - 1$
    * $y \ne f(-x) \therefore y \not\in \even$

---

## Answers to Exercises, cont.

* Determine if $y = 2\cos x + 3$ is even.
    * $2\cos x + 3 \in \even$
    * $f(-x) = 2\cos(-x) + 3$
    * $f(-x) = 2\cos x + 3$
    * $y = f(-x) \therefore y \in \even$

---

## Answers to Exercises, cont.

* Determine if $y = 3x^3$ is odd.
    * $3x^3 \in \odd$
    * $f(-x) = 3(-x)^3$
    * $f(-x) = -3x^3$
    * $-f(x) = -3x^3$
    * $f(-x) = -f(x) \therefore y \in \odd$

---

## Answers to Exercises, cont.

* Determine if $y = 4x^2 - x$ is odd.
    * $4x^2 - x \not\in \odd$
    * $f(-x) = 4(-x)^2 - (-x)$
    * $f(-x) = 4x^2 + x$
    * $-f(x) = -(4x^2 - x)$
    * $-f(x) = -4x^2 + x$
    * $f(-x) \ne -f(x) \therefore y \not\in \odd$

---

## Answers to Exercises, cont.

* Determine if $f(x) = 2x^3 + 5x$ is odd.
    * $f(x) \in \odd$
    * $f(-x) = 2(-x)^3 + 5(-x)$
    * $f(-x) = -2x^3 - 5x$
    * $f(-x) = -(2x^3 + 5x)$
    * $-f(x) = -(2x^3 + 5x)$
    * $f(-x) = -f(x) \therefore f(x) \in \odd$

---

## Answers to Exercises, cont.

* Determine if $y = \frac{1}{2}\sin 2x$ is odd.
    * $\frac{1}{2}\sin 2x \in \odd$
    * $f(-x) = \frac{1}{2}\sin (-2x)$
    * $f(-x) = -\frac{1}{2}\sin 2x$
    * $-f(x) = -\frac{1}{2}\sin 2x$
    * $f(-x) = -f(x) \therefore f(x) \in \odd$

---

## Answers to Exercises, cont.

* Determine what type of symmetry, if any, $y = 3x^2 - 5$ has.
    * $3x^2 - 5 \in \even$
    * $f(-x) = 3(-x)^2 - 5$
    * $f(-x) = 3x^2 - 5$
    * $y = f(-x) \therefore y \in \even$
    * $-f(x) = -(3x^2 - 5)$
    * $-f(x) = -3x^2 + 5$
    * $f(-x) \ne -f(x) \therefore y \not\in \odd$
    

---

## Answers to Exercises, cont.

* Determine what type of symmetry, if any, $y = 2x^3 + 7x$ has.
    * $2x^3 + 7x \in \odd$
    * $f(-x) = 2(-x)^3 + 7(-x)$
    * $f(-x) = -2x^3 - 7x$
    * $y \ne f(-x) \therefore y \not\in \even$
    * $-f(x) = -(2x^3 + 7x)$
    * $-f(x) = -2x^3 - 7x$
    * $f(-x) = -f(x) \therefore y \in \odd$

---

## Answers to Exercises, cont.

* Determine what type of symmetry, if any, $y = x^3 + x^2$ has.
    * $x^3 + x^2 \in \emptyset[f(x)]$
    * $f(-x) = (-x)^3 + (-x)^2$
    * $f(-x) = -x^3 + x^2$
    * $y \ne f(-x) \therefore y \not\in \even$
    * $-f(x) = -(x^3 + x^2)$
    * $-f(x) = -x^3 - x^2$
    * $f(-x) \ne -f(x) \therefore y \not\in \odd$

---

## Answers to Exercises, cont.

* Determine what type of symmetry, if any, $y = 4\sin x \cos x$ has.
* $y = 2\sin 2x$
    * $2\sin 2x \in \odd$
    * $f(-x) = 2\sin (-2x)$
    * $f(-x) = -2\sin 2x$
    * $y \ne f(-x) \therefore y \not\in \even$
    * $-f(x) = -2\sin 2x$
    * $f(-x) = -f(x) \therefore y \in \odd$

---

# [Next Lesson](Lesson%203)