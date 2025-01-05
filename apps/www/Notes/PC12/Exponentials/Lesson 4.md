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

<!--paginate: true-->

# Lesson 4: Points of Discontinuity

---

## Levels of Continuity

Throughout Math, you will find many levels of continuity.

1. Absolute Continuity (Limit and Value Continuous)
2. Removable Discontinuity or "hole" (Limit Continuous)
3. Asymptotic Discontinuity ($x,y \to \pm \infty$ as $x,y \to c$)
4. Absolute Discontinuity or "gap" (Limit and Value Discontinuous)

Last time, we focused on Asymptotic Discontinuity.
Now, let's look at Removable / Point Discontinuities.

---

## Points of Discontinuity

* PODs are singular points missing or separate from the graph.
* They result from simplification, often cancelling something out.
* They are drawn as holes in the graph.

---

## Examples

Try graphing $y = \frac{x^2 - 5x + 6}{x - 3}$. We are left with $y = x - 2, x \neq 3$.

Since it's a line, there is no asymptotes.

The behaviour at $x = 3$: $y \to 1$. But, $y \neq 1$. It's a hole.

As well, try graphing $y = \frac{x^2 - 4}{x^2 - x - 2}$.

---

## Characteristics to Equation

Write the equation of a possible rational function with the following characteristics:

* A vertical asymptote at $x = 2$
* A removable discontinuity at $(-1, -2/3)$
* x-intercept of -3

$y = \frac{(x + 3)(x + 1)}{(x - 2)(x + 1)}, a = 1$

---

## Determining Horizontal Asymptotes

* Look at the dominant terms (Degree).
    * $y = \frac{3x^2 - 5x + 6}{4x^2 + x - 2} \to \frac{3x^2}{4x^2}$, $y = \frac{3}{4}$
    * $y = \frac{6x^4 - 5}{2x^2} \to \frac{6x^4}{2x^2}$, $y = \frac{3x^2}{1} \therefore$ no HA.
    * $y = \frac{1}{x - 2} \to \frac{1}{x}$, $y = 0$

---

## Determine Characteristics

* $x$-int: set numerator = $0$
* $y$-int: set $x = 0$
* Restrictions: set denominator = $0$
* VA: Factor not in numerator
* POD: Factor also in numerator
* Domain: use restrictions
* Range: use HA and PODs

---

## Determine Characteristics, cont.

$$
\text{HA} = 

\begin{cases}
    \frac{x^m}{x^n}, n > m \therefore y = 0 \\
    \frac{x^m}{x^n}, m > n \therefore \emptyset \\
    \frac{ax^n}{bx^n} \therefore y = \frac{a}{b}
\end{cases}
$$

---

# [Next Unit <i class="fa-solid fa-diagram-next"></i>](../Logarithms/Lesson%201%20(Graphing).html)

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">