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

# Lesson 1: Long & Synthetic Division

---

<!--paginate: true-->

## Long Division Review

Divide $327 / 12$.

$$
    \begin{array}{rll}
        27 \\
        12 \enclose{longdiv}{327}\\
        - \underline{24\phantom{0}}\\
        87\\
        - \underline{84}\\
        3
    \end{array}
$$

$327/12 = 27 + \frac{1}{4}$

---

## Division Statements

* Can be written in these two ways:
* $\frac{\text{dividend}}{\text{divisor}} = \text{quotient} + \frac{\text{remainder}}{\text{divisor}}$ or
* $\text{dividend} = (\text{divisor} \cdot \text{quotient}) + \text{remainder}$
* Examples:
    * $\frac{327}{12} = 27 + \frac{1}{4}$ or
    * $327 = (12 \cdot 27) + 3$

---

## Polynomial Division

Long divide $(x^2 + 7x + 17) / (x + 3)$, restriction: $x \neq -3$

$$
    \begin{array}{rll}
        x + 4 \phantom{0}\\
        x + 3 \enclose{longdiv}{x^2 + 7x + 17}\\
        - \underline{x^2 + 3x\phantom{00000}}\\
        4x + 17\\
        - \underline{4x + 12}\\
        5
    \end{array}
$$

$x^2 + 7x + 17 = (x + 3)(x + 4) + 5$

---

## Synthesizing Division

* Another method of dividing polynomials is called **"Synthetic Division"**

$$
    \begin{array}{c|rrrr}
        & 1 & 7 & 14 & 9 \\
        -1 & \downarrow & -1 & -6 & -9 \\
        \hline
        & 1 & 6 & 8 & 1 \\
    \end{array}
$$

$x^3 + 7x^2 + 14x + 9 = (x + 1)(x^2 + 6x + 8) + 1$

* You could do the long division to check.
$(\text{left as exercise for reader})$

---

## Special Case: no remainder

$(2x^3 + 3x^2 - 4x + 15) / (x + 3)$

$$
    \begin{array}{c|rrrr}
        & 2 & 3 & -4 & 15 \\
        -3 & \downarrow & -6 & 9 & -15 \\
        \hline
        & 2 & -3 & 5 & 0 \\
    \end{array}
$$

$2x^3 + 3x^2 - 4x + 15 = (x + 3)(2x^2 - 3x + 5)$

* *Wait... This is the factored form!*

---

## Case: Missing Terms

$(x^3 - 10x + 6) / (x + 4)$

* What do we do? Add a zero for missing terms!

$$
    \begin{array}{c|rrrr}
        & 1 & 0 & -10 & 6 \\
        -4 & \downarrow & -4 & 16 & -24 \\
        \hline
        & 1 & -4 & 6 & -18 \\
    \end{array}
$$

$x^3 - 10x + 6 = (x + 4)(x^2 - 4x + 6) - 18$

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%202%20(Remainder%20Theorem).html) 

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">
