---
marp: true
theme: uncover
class: invert
math: mathjax
---

# <!--fit--> Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2025-->

---

# Lesson 3: Function Operations

---

<!--paginate: true-->

## Intro

* Many functions which we use are made by combining simple functions using the basic operations, or by composing functions.
* I'm assuming you know how to do these operations.

---

## Four Basic Operations

1. Given $g(x) = x^2 - 2x + 1, h(x) = x^2 + 3x - 4$, solve the following:
    - $f(x) = g(x) + h(x)$
        * $f(x) = (x^2 - 2x + 1) + (x^2 + 3x - 4)$
        * $f(x) = 2x^2 + x - 3$
    - $f(x) = g(x) - h(x)$
        * $f(x) = (x^2 - 2x + 1) - (x^2 + 3x - 4)$
        * $f(x) = (-5x + 5)$
        * $f(x) = 5(1 - x)$


---

## Basic Operations, cont.

- $f(x) = g(x)h(x)$
    * $f(x) = (x^2 - 2x + 1)(x^2 + 3x - 4)$
    * $f(x) = x^4 + x^3 - 9x^2 + 11x - 4$

---

## Operations, cont.

- $f(x) = \frac{g(x)}{h(x)}$
    * $f(x) = \frac{(x^2 - 2x + 1)}{(x^2 + 3x - 4)}$
    * $f(x) = \frac{(x - 1)^2}{(x - 1)(x + 4)}, x \neq -4, 1$
    * $f(x) = \frac{(x - 1)}{(x + 4)}, x \neq -4, 1$

* Restrictions are established for the original function. They are retained after cancellation.
* Given $g(x) = \frac{1}{x + 5}, h(x) = \frac{1}{x^2 - 25}$, calculate the basic operations. (ex. for readers)

---

## Operations with Trigonometrics

2. Calculate the basic operations, given $g(x) = \sin^2{x}, h(x) = \cot{x}$.
* $f(x) = g(x) + h(x)$
    * $f(x) = \sin^2{x} + \cot{x}, x \neq n\pi, n \in \mathbb{Z}$
    * $f(x) = \sin^2{x} + \frac{\cos{x}}{\sin{x}}, x \neq n\pi, n \in \mathbb{Z}$
    * $f(x) = \frac{\sin^3{x} + \cos{x}}{\sin{x}}, x \neq n\pi, n \in \mathbb{Z}$
* $f(x) = g(x) - h(x)$
    * $f(x) = \sin^2{x} + \cot{x}, x \neq n\pi, n \in \mathbb{Z}$
    * $f(x) = \frac{\sin^3{x} - \cos{x}}{\sin{x}}, x \neq n\pi, n \in \mathbb{Z}$

---

## Operations with Trig, cont.

2. Calculate the basic operations, given $g(x) = \sin^2{x}, h(x) = \cot{x}$.
* $f(x) = g(x)h(x)$
    * $f(x) = \sin^2{x} + \cot{x}, x \neq n\pi, n \in \mathbb{Z}$
    * $f(x) = \sin^2{x} + \frac{\cos{x}}{\sin{x}}, x \neq n\pi, n \in \mathbb{Z}$
    * $f(x) = \sin{x}\cos{x}, x \neq n\pi, n \in \mathbb{Z}$

---

## Trigonometric Division

2. Calculate the basic operations, given $g(x) = \sin^2{x}, h(x) = \cot{x}$.
* $f(x) = \frac{g(x)}{h(x)}$
    * $f(x) = \frac{\sin^2{x}}{\cot{x}}, x \neq n\pi, x \neq \frac{\pi}{2} + n\pi, n \in \mathbb{Z}$
    * $f(x) = \frac{\sin^2{x}}{\frac{\cos{x}}{\sin{x}}}, x \neq n\pi, x \neq \frac{\pi}{2} + n\pi, n \in \mathbb{Z}$
    * $f(x) = \sin^2{x} \times {\frac{\sin{x}}{\cos{x}}}, x \neq n\pi, x \neq \frac{\pi}{2} + n\pi, n \in \mathbb{Z}$
    * $f(x) = \frac{\sin^3{x}}{\cos{x}}, x \neq n\pi, x \neq \frac{\pi}{2} + n\pi, n \in \mathbb{Z}$

---

## Composition

3. Given $f(x) = x^2, g(x) = x + 4$, evaluate the following:
    - $h(x) = f(g(x)) = (f \circ g)(x)$
        * $h(x) = f(x + 4)$
        * $h(x) = (x + 4)^2$
    - $h(x) = g(f(x)) = (g \circ f)(x)$
        * $h(x) = g(x^2)$
        * $h(x) = x^2 + 4$

* Evaluate the composite functions, given $g(x) = \frac{1}{x}, h(x) = x - 2$ (ex. for reader)

---

## Bonus Exercises

* Determine the following, given $g(x) = \sin{x}, h(x) = x^2$:
    * $\frac{h(x)}{g(x)}$
    * $g(h(x))$
    * $h(g(x))$
* Determine the following, given $g(x) = \frac{1}{\sqrt{x}}, h(x) = x^2 - 1$:
    * $g(x) + h(x)$
    * $g(x)h(x)$
    * $h(g(x))$

---

# [Next Lesson](Lesson%204)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercise

* Given $g(x) = \frac{1}{x + 5}, h(x) = \frac{1}{x^2 - 25}$, calculate the basic operations.
* $f(x) = g(x) + h(x)$
    - $f(x) = \frac{1}{x + 5} + \frac{1}{x^2 - 25}, x \neq \pm 5$
    - $f(x) = \frac{1}{x + 5} + \frac{1}{(x - 5)(x + 5)}, x \neq \pm 5$
    - $f(x) = \frac{(x - 5) + 1}{(x - 5)(x + 5)}, x \neq \pm 5$
    - $f(x) = \frac{x - 4}{x^2 - 25}, x \neq \pm 5$

---

## Answers to Exercise, cont.

* $f(x) = g(x) - h(x)$
    - $f(x) = \frac{1}{x + 5} - \frac{1}{x^2 - 25}, x \neq \pm 5$
    - $f(x) = \frac{1}{x + 5} - \frac{1}{(x - 5)(x + 5)}, x \neq \pm 5$
    - $f(x) = \frac{(x - 5) - 1}{(x - 5)(x + 5)}, x \neq \pm 5$
    - $f(x) = \frac{x - 6}{x^2 - 25}, x \neq \pm 5$
* $f(x) = g(x)h(x)$
    - $f(x) = (\frac{1}{x + 5})(\frac{1}{x^2 - 25}), x \neq \pm 5$
    - $f(x) = \frac{1}{(x + 5)(x^2 - 25)}, x \neq \pm 5$

---

## Answers to Exercise, cont.

* $f(x) = \frac{g(x)}{h(x)}$
    - $f(x) = \frac{\frac{1}{x + 5}}{\frac{1}{x^2 - 25}}, x \neq \pm 5$
    - $f(x) = \frac{(x - 5)(x + 5)}{x + 5}, x \neq \pm 5$
    - $f(x) = x - 5, x \neq \pm 5$

---

## Answers to Exercise, cont.

* Evaluate the composite functions, given $g(x) = \frac{1}{x}, h(x) = x - 2$ (ex. for reader)
    * $f(x) = g(h(x))$
        * $f(x) = \frac{1}{x - 2}$
    * $f(x) = h(g(x))$
        * $f(x) = \frac{1}{x} - 2$
        * $f(x) = \frac{1 - 2x}{x}$

---

# [Next Lesson](Lesson%204)