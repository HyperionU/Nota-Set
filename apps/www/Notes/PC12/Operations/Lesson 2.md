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

# Lesson 2: Composition of Functions

---

## Composition of Functions

* A **Composite Function** is a function formed from two functions in which the output of one function (Inner) is used as the input of the other (Outer)
* $h(x) = f(g(x)) = (f \circ g)(x)$

---

## Values of Functions

* If $f(x) = 3x - 4$, determine the value or expression for:
* $f(2)$
    * $6 - 4 = 2$
* $f(-3)$
    * $-9 - 4 = -13$
* $f(c)$
    * $3c - 4$
* $f(x - 1)$
    * $3(x - 1) - 4 = 3x - 7$

---

## Composing Functions 

If $f(x) = 4x, g(x) = x + 6, h(x) = x^2$, determine each expression or value.

* $f(g(x)) = 4(x + 6)$
* $h(g(x)) = (x + 6)^2$
* $h(h(2)) = 2^4 = 16$
* $h(f(x)) = 16x^2$
* $f(g(3)) = 4(9) = 36$
* $g(h(-2)) = 4 + 6 = 10$
* $g(h(x)) = x^2 + 6$

---

## Domain of Composites

* The domain of $f(g(x))$ exists only for $x$ in the domain of $g(x)$.
* Consider $f(x) = \sqrt{x - 1}, g(x) = x^2$. 
    * Determine $(f \circ g)(x), (g \circ f)(x)$.
        * $f \circ g = \sqrt{x^2 - 1}$
        * $g \circ f = x - 1$
    * State each of their domains.

|        | $f(x)$ | $g(x)$ | $f(g(x))$ | $g(f(x))$ |
|--------|--------|--------|-----------|-----------|
| Domain | $x \geq 1$ | $x \in \mathbb{R}$ | $x \geq 1, x \leq -1$ | $x \geq 1$ |

---

## Inner and Outer Functions

If $h(x) = f(g(x))$ is given below, determine $f(x)$ and $g(x)$.

| $h(x)$ | $f(x)$ | $g(x)$ |
|--------|--------|--------|
| $\sqrt{x^3 - 1}$ | $\sqrt{x}$ | $x^3 - 1$ |
| $(x - 2)^4$ | $x^4$ | $x - 2$ |
| $\sin(\cos x)$ | $\sin x$ | $\cos x$ |
| $\frac{1}{4x + 5}$ | $\frac{1}{x}$ | $4x + 5$ |
| $4^{3x + 1}$ | $4^x$ | $3x + 1$ |
| $(x - 2)^2 + 5(x - 2) + 1$ | $x^2 + 5x + 1$ | $x - 2$ |

---

# [Finish <i class="fa-solid fa-flag-checkered"></i>](https://hyperionu.github.io/Nota-Set)

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">