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

# Lesson 4: Rational Zero Theorem

---

<!--paginate: true-->

## Rational Zeros Theorem

Sometimes, zeros could be rational if the lead coefficient isn't 1.

*$\textbf{Theorem:}$ if $(ax - b) \in \mathfrak{f}(P(x)), b \mod A = 0, a \mod C = 0$.*

---

## Find Rational Roots

1. Find all possible Rational roots of $3x^3 - 4x^2 + 5x - 4$.
* $\pm 1, \pm 2, \pm 4 / \pm 1, \pm 3$
* This gives us $\pm 1, \pm 2, \pm 4, \pm\frac{1}{3}, \pm\frac{2}{3}, \pm\frac{4}{3}$.
2. Factor $3x^3 - 4x^2 + 5x - 4$

$$
    \begin{array}{c|rrrr}
        {} & 3 & -4 & 5 & -4 \\
        1 & \downarrow & 3 & -1 & 4 \\
        \hline
        {} & 3 & -1 & 4 & \fbox{0} \\
    \end{array}
$$

We get: $(x - 1)(3x^2 - x + 4)$

---

## Factoring Practice: $a \not = 1$

* We have two different paths: Factor by Inspection ("The Shortcut") and Decomposition.

* $2x^2 - 5x - 3$
    * Factor by inspection: $(2x + 1)(x - 3)$
* $3x^2 - 2x - 5$
    * Decomposition:
        * $3x^2 + 3x - 5x - 5$
        * $3x(x + 1) - 5(x + 1)$
        * $(3x - 5)(x + 1)$

---

## How To Factor

You now have another possible way added to your toolbelt:
* Product / Sum (The First Path)
* Diff. of Squares (Binomials only)
* PST ($x^2 + 2xy + y^2$)
* Decomposition ($a \not = 1$)
* Inspection ("The Shortcut")

Recognising which method to use makes factoring easier.

---

## Example:

Factor $2x^3 - 5x^2 - x + 6$

1. Determine all possible Rational Roots
* $\pm 1, \pm 2 / \pm 1, \pm 2, \pm 3, \pm 6$
* $\pm 1, \pm 2, \pm\frac{1}{2}, \pm\frac{1}{3}, \pm\frac{1}{6}, \pm\frac{2}{3}$
2. Synthetic divide to simplify

$$
    \begin{array}{c|rrrr}
        {} & 2 & -5 & -1 & 6 \\
        2 & \downarrow & 4 & -2 & -6 \\
        \hline
        {} & 2 & -1 & -3 & \fbox{0} \\
    \end{array},\ (x - 2)(2x^2 - x - 3)
$$

---

## Example, cont.

We have: $(x - 2)(2x^2 - x - 3)$

3. Simplify, if possible.
    * Using factoring by inspection on the trinomial, we get $(2x - 3)(x + 1)$

Result: $(x - 2)(x + 1)(2x - 3)$

---

## Determining Coefficients

Determine $k$, s.t. $x + 1$ is a factor of $x^3 - x^2 + kx - 3$.

* $x^3 - x^2 + kx - 3 = 0$
* $(-1)^3 - (-1)^2 + k(-1) - 3 = 0$
* $-1 - 1 - k - 3 = 0$
* $-k - 5 = 0$
* $k = -5$

---

## Applications Example 1

The Volume $V$ of a prism is given by $x^3 + 14x^2 + 63x + 90$. If the height is $x + 5$, what polynomials represent the possible length and width.

* Common Assumption: $V = \ell{w}h$.
* $x^3 + 14x^2 + 63x + 90 = \ell{w}(x + 5)$

$$
    \begin{array}{c|rrrr}
        {} & 1 & 14 & 63 & 90 \\
        -5 & \downarrow & -5 & -45 & -90 \\
        \hline
        {} & 1 & 9 & 18 & \fbox{0} \\
    \end{array},\ (x^2 + 9x + 18)
$$

---

## Applications Example 1, cont.

We now know that $\ell{w} = x^2 + 9x + 18$
* Finally, factor to get our values.
* $\ell \text{ and } w = (x + 6)(x + 3)$

---

## Applications Example 2

A boardwalk that is $x$ feet wide is built around a rectangular pond. The Pond is $30 \text{ ft} \times 40 \text{ ft}$. The combined surface area is $2000 \text{ ft}^2$. What is the width of the boardwalk.
* Try drawing a picture to help you.

---

## Applications Example 2 Answer

* What we Know:
    * $A_C = 2000 \text{ ft}^2$
    * $A_C = (2x + 40)(2x + 30)$
* Solve:
$$
    \begin{array}{ccc}
        (2x + 40)(2x + 30) & = & 2000 \\
        4x^2 + 140x + 1200 & = & 2000 \\
        4x^2 + 140x - 800 & = & 0 \\
        4(x^2 + 35x - 200) & = & 0
    \end{array}
$$

---

## Applications Example 2, cont.

* We have: $4(x^2 + 35x - 200) =  0$
* Continuing solving:

$$
    \begin{array}{ccc}
        4(x^2 + 35x - 200) & = & 0 \\
        x^2 + 35x - 200 & = & 0 \\
        (x + 40)(x - 5) & = & 0 \\
    \end{array}
$$

* This gets us: $x = \not-40, 5$
* And finally, our result: $x = 5$.

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%205%20(Polynomial%20Equations).html) 

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">