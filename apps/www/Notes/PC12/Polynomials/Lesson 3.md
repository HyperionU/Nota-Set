---
marp: true
theme: uncover
class: invert
math: mathjax
style: |
  .columns {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1rem;
  }
---

# <!--fit--> Pre-Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2024-->

---

# Lesson 3: Factor Theorem

---

<!--paginate: true-->

## What are Factors?

* Numbers or expressions that divide evenly into a dividend. 
* This means that the modulus is 0. (*remember the previous lesson?*)

---

## Factor Theorem

$\textbf{Theorem: } P(x) / (x - a), (x - a)$ is a factor if and only if $P(a) = 0$

* *This is actually just a special case of the Remainder theorem.*

---

## Finding Factors

Which of the following are factors of $P(x) = x^3 - 7x + 6$
* $x + 1$?
* $x - 1$?
* $x + 2$?
* $x - 2$?
* $x + 3$?

---

## Finding Factors, cont.

<div class = "columns">
<div>

* $x + 1$
    * $(-1)^3 + 7 + 6$
    * $-1 + 13$
    * $\text{n.f.}$
* $x - 1$
    * $(1)^3 - 7 + 6$
    * $1 - 1$
    * $0 \therefore (x - 1) \text{ f.}$ 

</div>
<div>

* $x + 2$
    * $(-2)^3 - 7(-2) + 6$
    * $-8 + 20$
    * $\text{n.f.}$
* $x - 2$
    * $(2)^3 - 14 + 6$
    * $8 - 8$
    * $0 \therefore (x - 2) \text{ f.}$ 

</div>
</div>

---

## Finding Factors, cont.

We can also find them using synthetic division.

$(x + 3)$

$$
    \begin{array}{c|rrrr}
        {} & 1 & 0 & -7 & -6 \\
        -3 & \downarrow & -3 & 9 & -6 \\
        \hline
        {} & 1 & -3 & 2 & \fbox{0} \\
    \end{array}
    
    \therefore (x + 3) \text{ f.}
$$

Then, we get:
$\mathfrak{f}(P(x)) = (x - 1)(x - 2)(x + 3)$

---

## Integral Zero Theorem

Picking numbers is inefficient, so we need some way to make it efficient.

*$\textbf{Theorem:}$ if $(x - a)$ is a factor of $P(x),\ \therefore a \mod c = 0,$ where $c$ is the constant term.*

---

## Finding Integral Roots

Find all possible integral roots of $P(x) = x^3 - 3x^2 - x + 3$
1. Find the integral roots.
    * $3$ is prime, so it's only $\pm 1, \pm 3$.
2. Synthetic Divide to a simpler form

$$
    \begin{array}{c|rrrr}
        {} & 1 & -3 & -1 & 3 \\
        1 & \downarrow & 1 & -2 & -3 \\
        \hline
        {} & 1 & -2 & -3 & \fbox{0} \\
    \end{array}
$$

$\mathfrak{f}(P(x)) = (x - 1)(x^2 - 2x - 3)$

---

## Finding Integral Roots, cont.

We now have $\mathfrak{f}(P(x)) = (x - 1)(x^2 - 2x - 3)$.

3. Factor if possible.
* $x^2 - 2x - 3$
* $(x - 3)(x + 1)

Leaving us with:

$\mathfrak{f}(P(x)) = (x - 1)(x - 3)(x + 1)$

---

## All Possible Zeros

Find the possible zeros of $P(x) = x^4 - 5x^3 + 2x^2 + 20x - 24$

Here's our possible options:
* $\pm 1, \pm 2$
* $\pm 3, \pm 4$
* $\pm 6, \pm 8$
* $\pm 12, \pm 24$

---

## Possible Zeros, Part 2

Here's our possible options:
* $\pm 1, \pm 2$
* $\pm 3, \pm 4$
* $\pm 6, \pm 8$
* $\pm 12, \pm 24$

1. Remove unreasonable answers

Remaining Possibilities: $\pm 2, \pm 3, \pm 4, \pm 6, \pm 8$.

---

## Possible Zeros, Part 3

2. Synthetic divide to simplify.

$$
    \begin{array}{c|rrrr}
        {} & 1 & -5 & 2 & 20 & -24 \\
        3 & \downarrow & 3 & -6 & -12 & 24 \\
        \hline
        {} & 1 & -2 & -4 & 8 & \fbox{0} \\
        2 & \downarrow & 2 & 0 & -8 \\
        \hline
        {} & 1 & 0 & -4 & \fbox{0}
    \end{array}
$$

We get: $\mathfrak{f}(P(x)) = (x - 3)(x - 2)(x^2 - 4)$

---

## Possible Zeros, Part 4

We have: $\mathfrak{f}(P(x)) = (x - 3)(x - 2)(x^2 - 4)$

3. Simplify any non-trivial polynomials

$\mathfrak{f}(P(x)) = (x - 3)(x - 2)^2(x + 2)$

*$(x - 2)$ would be what's known as a **bouncing root**, but we'll get there when we do.*

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%204%20(Rational%20Zero%20Theorem).html) 

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">
