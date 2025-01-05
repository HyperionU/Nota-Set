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

<!--paginate: true-->

# Lesson 5: Logarithmic / Exponential Equations

---

## Types of Equations

There are three types of equations:

* Type I: All terms have logs.
    * $\log_b P = \log_b Q \implies P = S$
* Type II: Some terms have logs.
    * $\log_b A = c \implies b^c = A$ 
* Type III: Exponentials w/o same base.
    * $P^x = Q^y \implies x \log P = y \log Q$

---

## Type I Example

* $\log_3 (x - 1) + \log_3 x = \log_3 12$
* State Restrictions: $x > 1, x > 0$
    * Simplifies to $x > 1$
* $\log_3 (x(x - 1)) = \log_3 12$
* $x^2 - x = 12$
* $x^2 - x - 12 = 0$
* $(x - 4)(x + 3)$
* $x = 4, x \neq 3\ (\not\in x > 1, EV)$

---

## Type II Example

* $\log_5 (x - 6) = 1 - \log_5 (x - 2)$
* State Restrictions: $x > 6, x > 2$
    * Simplifies to $x > 6$
* $\log_5 (x - 6) + \log_5 (x - 2) = 1$
* $\log_5 [(x - 6)(x - 2)] = 1$
* $(x - 6)(x - 2) = 5^1$
* $x^2 - 8x + 12 = 5$
* $x^2 - 8x + 7 = 0$

---

## Type II Example, cont.

* $x^2 - 8x + 7 = 0$
* $(x - 7)(x - 1)$
* $x = 7, x \neq 1\ (\not \in x > 6, EV)$

---

## Type II Example 2

* $\log (8x + 4) = 1 + \log (x + 1)$
* State Restrictions: $x > -1, x > -\frac{1}{2}$
    * Simplifies to $x > -\frac{1}{2}$
* $\log(8x + 4) - \log(x + 1) = 1$
* $\log[\frac{8x + 4}{x + 1}] = 1$
* $\frac{8x + 4}{x + 1} = 10$

---

## Type II, cont.

* $\frac{8x + 4}{x + 1} = 10$
* $8x + 4 = 10(x + 1)$
* $8x + 4 = 10x + 10$
* $2x = -6$
* $x \neq -3\ (\not \in x > -\frac{1}{2}, EV)$
* No Solution. *Oh well.*

---

## Type III Example

* $3^{x + 1} = 5^x$
* Take log of both sides
* $\log 3^{x + 1} = \log 5^x$
* $(x + 1) \log 3 = x \log 5$
* $x \log 3 + \log 3 = x \log 5$
* $\log 3 = x \log 5 - x \log 3$
* $\log 3 = x (\log 5 - \log 3)$

---

## Type III Example, cont.

* $\log 3 = x (\log 5 - \log 3)$
* $x = \frac{\log 3}{\log 5 - \log 3}$
* $x = 2.15$

---

## Exponentials with Coefficients

* Be careful! $\alpha \cdot b^x \neq (\alpha b)^x$
* Example: $2(5)^{x - 2} = 4^{3x - 1}$
* $\log[2(5)^{x - 2}] = \log 4^{3x - 1}$
* $\log 2 + (x - 2) \log 5 = (3x - 1) \log 4$
* $\log 2 + x \log 5 - 2 \log 5 = 3x \log 4 - \log 4$ 
* *Wow! This is complicated.*

---

## Clearing the Static

* We have $\log 2 + x \log 5 - 2 \log 5 = 3x \log 4 - \log 4$.
* With some shifting: $\log 2 + \log 4 - 2 \log 5 = 3x \log 4 - x \log 5$
* $\log \frac{8}{25} - x (3 \log 4 - \log 5)$
* $x = \log \frac{8}{25} / \log \frac{64}{5}$
* $x = -0.45$

---

## Calculation Flow

* Same Base (Type I)
    * Set values to each other
    * If logarithm, make sure answer fits restrictions.
* Dif. Base (Exponential, Type III)
    * Take log on both sides
    * Solve
* Dif. Base (Logarithmic, Type II)
    * Convert to Exponential
    * Solve, verify if answer fits restrictions (if needed).

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%206%20(Applications).html)

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">