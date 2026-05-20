---
marp: true
theme: uncover
class: invert
math: mathjax
---

$\newcommand\diff[1]{\mathcal{d}_{#1}}$

# <!--fit--> Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2025-->

$\newcommand\dd[2][]{\displaystyle\frac{d#1}{d#2}}$

---

# Lesson 1: The Fundamental Theorem of Calculus

---

<!--paginate: true-->

## Intro

* In previous units, we studied how to differentiate a function (Units 3-6) and integrate a function (Unit 7).
* Integrals can be calculated as limits of sums, a long and arduous process.
* However, there is a concise method for determining the value of a definite integral.
* Similarly, we can use these other concise methods to quickly find antiderivatives. This unit focuses on this "porcelain".

---

## The Fundamental Theorem

* For a continuous function $y = f(x)$ on an interval $[a, b]$, the accumulated signed area under the curve $f(x)$ from point $a$ to $b$ can be represented by the definite integral $\int_a^b f(x) dx$.
* From our study of accumulated signed area, we know this is equal to $F(a) - F(b)$, where $F(x)$ is any antiderivative of $f(x)$.
* In other words, $F'(x) = f(x)$.
* Thus, **The Fundamental Theorem of Calculus** has two parts.

---

## The Fundamental Theorem, Part I

1. If $f$ is a continuous function on an interval $[a, b]$, then $F(x) = \int_a^x f(t) dt$ has a derivative at every point in the interval $[a, b]$, such that $\dd{x}[F(x)] = \dd{x} \int_a^x f(t) dt = f(x)$.
    * This part states that the definite integral of a continuous function is a differentiable function of its upper limit of integration.
    * The integrand is the derivative of that function.
    * The antiderivative of any continuous function exists.

---

## The Fundamental Theorem, Part II

2. If $f$ is a continuous function on an interval $[a, b]$ and $F$ is any antiderivative of $f$, then $\int_a^b f(x) dx = F(b) - F(a)$.
    * This part describes how to evaluate a definite integral.
    * The integral of the derivative between the bounds equals the original function at the bounds.

---

## Example 1

1. Evaluate $\int_1^3 x^2 dx$
    * $x^2$ is continuous (trivial)
    * $F(x) = \frac{1}{3}x^3 + C$.
    * $\int_1^3 x^2 dx = (\frac{1}{3}x^3 + C)\rvert_1^3$
    * $(\frac{1}{3}x^3 + C)\rvert_1^3 = (\frac{1}{3}3^3 + C) - (\frac{1}{3}1^3 + C)$
    * $\frac{27}{3} - \frac{1}{3}$
    * $\frac{26}{3}$

---

## Tables and Properties

* We can create tables of integration showing the integrals we have learned
* Typical Advanced Calculus texts often have appendices with tables of integrals, starting from basics but concentrating on complicated integrals. 
* In Lessons 2 - 4, we'll learn new techniques for solving more complicated integrals, at which point you can expand or create your own tables.

---

## Fundamental Integration Laws

1. Linearity: $\int [\alpha f(x) + \beta g(x)] dx = \alpha \int f(x) dx + \beta \int g(x) dx$ 
2. Reverse Power: $\int x^n dx = \frac{1}{n + 1} x^{n + 1} + C, n \ne -1$
3. Cosine: $\int \cos x dx = \sin x + C$
4. Sine: $\int \sin x dx = C - \cos x$
5. Exponential: $\int (b^x \ln b) dx = b^x + C$
    * Special Case: $\int e^x dx = e^x + C$
6. Logarithmic: $\int \frac{1}{x \ln b} dx = \log_b |x| + C, x \ne 0$
    * Special Case: $\int \frac{1}{x} dx = \ln \lvert x \rvert + C, x \ne 0$.

---

## Exercise for Readers

* Given $\int_a^b f(x) dx = F(3) - F(1)$, find $a$ and $b$.
* Given $f(x) = \frac{1}{x^2}$ and $F'(x) = f(x)$, find $F(x)$.
* Find $\int \sin x dx$
* Evaluate $\int_0^\pi \sin x dx$
* Evaluate $\int_2^3 4 dx$

---

# [Next Lesson](Lesson%202)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Given $\int_a^b f(x) dx = F(3) - F(1)$, find $a$ and $b$.
    * $\int_a^b f(x) dx = F(b) - F(a)$
    * $a = 1, b = 3$
* Given $f(x) = \frac{1}{x^2}$ and $F'(x) = f(x)$, find $F(x)$.
    * $F(x) = \int \frac{1}{x^2} dx$
    * $F(x) = \int x^{-2} dx$
    * $F(x) = \frac{1}{-2 + 1} x^{-2 + 1} + C$ (Reverse Power Rule)
    * $F(x) = -\frac{1}{x} + C$

---

## Answers to Exercises, cont.

* Find $\int \sin x dx$
    * $\int \sin x dx = C - \cos x$
* Evaluate $\int_0^\pi \sin x dx$
    * $\int_0^\pi \sin x dx = (C - \cos x)\rvert_0^\pi$
    * $(C - \cos x)\rvert_0^\pi = (C - \cos \pi) - (C - \cos 0)$
    * $\cos 0 - \cos \pi$
    * $2$

---

## Answers to Exercises, cont.

* Evaluate $\int_2^3 4 dx$
    * $\int_2^3 4 dx = (4x)\rvert_2^3$
    * $(4x)\rvert_2^3 = 4(3) - 4(2)$
    * $4(3) - 4(2) = 4(3 - 2)$
    * $4$

---

# [Next Lesson](Lesson%202)