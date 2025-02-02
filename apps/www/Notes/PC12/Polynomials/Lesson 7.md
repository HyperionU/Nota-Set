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

# Lesson 7: Graphing Polynomials

---

<!--paginate: true-->

## "Graphing"

When I say graphing, unless you're using an actual graphing calculator, you only need to make a sketch.

---

## Factoring Expressions

Factor $x^4 + x^3 - 10x^2 - 4x + 24$

$$
    \begin{array}{c|rrrrr}
        {} & 1 & 1 & -10 & -4 & 24 \\
        -2 & \downarrow & -2 & 2 & 16 & -24 \\
        \hline
        {} & 1 & -1 & -8 & 12 & \fbox{0} \\
        2 & \downarrow & 2 & 2 & -12 \\
        \hline
        {} & 1 & 1 & -6 & \fbox{0}
    \end{array}
$$

$(x + 2)(x - 2)(x^2 + x - 6)$
$(x + 2)(x - 2)^2(x + 3)$

---

## Graphing

Graph $f(x) = x^4 + x^3 - 10x^2 - 4x + 24$
$(x + 2)(x - 2)^2(x + 3)$

* LC: $1, R \uparrow$
* Deg: $4, L \uparrow$
* max 4 directions, 3 turns, 4 roots
* $y$-int: $(0, 24)$
* $x$-int: $2 (B), -2 (C), -3 (C)$
* Try graphing this in Desmos. What do you notice?

---

## Multiplicity

For a zero:
* if $n \mod 2 = 0, f(x)$ will bounce.
* if $n \mod 2 = 1$ and $n = 1$ $f(x)$ will cross $x$-axis straight.
* if $n \mod 2 = 1$ and $n \geq 3$ $f(x)$ will cross $x$-axis curved.

---

## Graphing Factored Expressions

Graph $y = -2(x + 1)^2(x - 1)(x + 3)$
* LC: $-2, R \downarrow$
* Deg: $4, L \downarrow$
* max 4 directions, 3 turns, 4 roots
* $y$-int: $(0, 6)$
* $x$-int: $-1 (B), 1 (C), -3 (C)$

---

## Determining Equations

Determine an equation for a polynomial, with roots at 3 and -2 ($M = 2$), and passes through the point $(1, 5)$.

* Roots: $3, -2(M2)$
* Point: $(1,5)$
$f(x) = a(x - 3)(x + 2)^2$
* Find $a$

To find $a$, we disregard $a$, and plug in $P_x$, and divide $P_y$ by that value.

We get $f(x) = \frac{-5}{18}(x - 3)(x + 2)^2$.

---

# [Next Unit <i class="fa-solid fa-diagram-next"></i>](../Trigonometry/Functions/Lesson%201%20(Radians).html)

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">