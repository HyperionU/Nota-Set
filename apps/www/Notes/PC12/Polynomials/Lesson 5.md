---
marp: true
theme: uncover
class: invert
math: mathjax
---

# <!--fit--> Pre-Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2024-->

---

# Lesson 5: Solving Polynomial Equations

---

<!--paginate: true-->

## Solving

Solving requires more steps than factoring:
* Solve $x^2 - x - 42 = 0$
* $(x + 6)(x - 7) = 0$ 
* $x + 6 = 0, x - 7 = 0$
* $x = -6, 7$

---

## How to Solve

Here's how to solve:
1. Set the polynomial to equal 0
2. Factor the polynomial
3. Find the roots.

---

## Example
Solve $x^3 + 12 = 3x^2 + 4x$

1. Set to 0
* $x^3 - 3x^2 - 4x + 12 = 0$
2. Synthetic Divide
$$
    \begin{array}{c|rrrr}
        {} & 1 & -3 & -4 & 12 \\
        -2 & \downarrow & -2 & 10 & -12 \\
        \hline
        {} & 1 & -5 & 6 & \fbox{0} \\
    \end{array}, (x + 2)(x^2 - 5x + 6)
$$

---

## Example, cont.

3. Factor
* $(x + 2)(x^2 - 5x + 6)$
* $(x + 2)(x - 3)(x - 2)$
4. Set factors to zero.
* $x \pm 2 = 0, x - 3 = 0$
* $x = \pm 2, 3$

---

## Solving non-Factorable Factors

* Solve $x^3 + 9x^2 + 13x + 5 = 0$
1. Synthetic Divide
$$
    \begin{array}{c|rrrr}
        {} & 1 & 9 & 13 & 5 \\
        -1 & \downarrow & -1 & -8 & -5 \\
        \hline
        {} & 1 & 8 & 5 & \fbox{0} \\
    \end{array}, (x + 1)(x^2 + 8x + 5)
$$
* $x = -1$, but the second factor is more challenging.

---

## Quad Formula: The $mp$-Formula

Let's take our quadratic $x^2 + 8x + 5$.
1. Get the midpoint: $m \frac{b}{2}$ and the Product: $p = c$
2. Here's the formula: $-m \pm \sqrt{m^2 - p}$
3. Use the formula.
* $m = 4, p = 5$
* $-4 \pm \sqrt{16 - 5}$
* $-4 \pm \sqrt{11}$

---

## Trivial Solutions

* Solve $x^3 + 1 = 0$
* *We could factor this, but there's an easier way.*
* $x^3 = -1$
* $\sqrt[3]{x^{\not 3}} = \sqrt[3]{-1}$
* $x = -1$, among others.

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%206%20(Characteristics).html) 

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">