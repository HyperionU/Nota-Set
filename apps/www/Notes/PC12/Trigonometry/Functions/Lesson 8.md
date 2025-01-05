---
marp: true
theme: uncover
class: invert
math: mathjax
---

$\newcommand\gensol[1][2]{\pm #1\pi n, n \in \mathbb{N}}$

# <!--fit--> Pre-Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2024-->

$\def\reals{\mathbb{R}}$

---

<!--paginate: true-->

# Lesson 8: General Solution

---

## The General Solution

A way to state that there are many solutions that go up by some multiple amount each time.

Here's an Example: Solve over $\reals$: $\sin x = \frac{3}{5}$

* $x_r = \sin^{-1}(\frac{3}{5}) = 0.6435$
* $x_1 = x_r \gensol$
* $x_2 = (\pi - x_r) \gensol$
* $x_1 = 0.64 \gensol$, $x_2 = 2.50 \gensol$

---

## Quadratic General Solutions

Solve over $\reals$: $2 \cos^2 x - \cos x - 1 = 0$

* $(2\cos x + 1)(\cos x - 1)$
* $\cos x = 1, -\frac{1}{2}$
* $x = 0 \gensol$
* $x_r = \cos^{-1}(\frac{1}{2}) = \frac{\pi}{3}$
* $x_1 = (\pi - x_r) \gensol$, $x_2 = (\pi + x_r) \gensol$

---

## Quadratic General Solution

$$ x = 
    \begin{cases}
        0 \gensol \\
        \frac{4\pi}{3} \gensol \\
        \frac{2\pi}{3} \gensol
    \end{cases}
$$

---

## Non-Factorable General Solution

Solve over $\reals$: $5 \tan^2 x + 3 \tan x - 3 = 0$

For this, we'll use the quadratic formula.

1. $a$-reduction
    * $\tan^2 x + \frac{3}{5} \tan x - \frac{3}{5}$
2. Find Midpoint: $m = \frac{3}{10}$ and Product: $c = -\frac{3}{5}$

$-\frac{3}{10} \pm \sqrt{(\frac{3}{10})^2 + \frac{3}{5}}$

---

## Non-Factorable Solution, cont.

* $-\frac{3}{10} \pm \sqrt{\frac{69}{100}}$
* $\frac{-3 \pm \sqrt{69}}{10}$
* $\tan x = 0.5307, -1.1307$
* $x_{r1} = \tan^{-1}(0.5307) = 0.4879$
* $x_{r2} = \tan^{-1}(1.1307) = 0.8467$
* $x_1 = x_{r1} \gensol[]$
* $x_2 = (\pi - x_{r2}) \gensol[]$

For $\tan x$, it repeats every $\pi$

---

## Non-Factorable General Solution:

$$ x = 
    \begin{cases}
        0.49 \gensol[] \\
        2.29 \gensol[]
    \end{cases}
$$

---

# [Next Unit <i class="fa-solid fa-diagram-next"></i>](../Graphing/Lesson%201%20(Plotting%20Trigonometric%20Functions).html)

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">