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

# Lesson 2: Integration by Substitution

---

<!--paginate: true-->

## Intro

* The method of integration by substitution is a technique through which we express the function in simpler terms by 
    * utilizing a new variable, 
    * solve the function, and 
    * restore the original variable

---

## Example 1

1. Evaluate $\int 2x(x^2 + 1)dx$
    * For this integral, there are a number of different methods to solve.
    * First, by substitition:
        * Let $u = x^2 + 1$
        * $du = 2x dx$
        * $dx = \frac{du}{2x}$
        * $\int u du$
        * $\frac{u^2}{2} + C = \frac{1}{2}(x^2 + 1) + C$.

---

## Example 1, cont.

1. Evaluate $\int 2x(x^2 + 1)dx$
    * Next, by expansion:
        * $\int 2x^3 + 2x dx$
        * $2\int x^3 dx + 2\int x dx$
        * $2(\frac{1}{4} x^4 + C_1) + 2 (\frac{1}{2}x^2 + C_2)$
        * $2(\frac{1}{4} x^4 + \frac{1}{2}x^2 + C_3)$
        * $\frac{1}{2} x^4 + x^2 + \frac{1}{2} + C$
        * $\frac{1}{2}(x^4 + 2x^2 + 1) + C$
        * $\frac{1}{2}(x^2 + 1) + C$


---

## Example 2

2. Evaluate $\int (x^2 + 6)^8 (2x) dx$
    * Let $u = x^2 + 6$
    * $du = 2x dx$
    * $dx = \frac{du}{2x}$
    * $\int u^8 du$
    * $\frac{1}{9}u^9 + C$
    * $\frac{1}{9}(x^2 + 6)^9 + C$

---

## Example 3

3. Find $\int 20x(x + 1)^\frac{1}{2} dx$ by substitution.
    * Let $u = (x + 1)^\frac{1}{2}$
    * $u^2 = x + 1$
    * $x = u^2 - 1$
    * $dx = 2u du$
    * $\int 20(u^2 - 1)2u^2 du$
    * $40 \int (u^4 - u^2) du$
    * $40 (\frac{1}{5}u^5 - \frac{1}{3}u^3) + C$

---

## Example 3, cont.

3. Find $\int 20x(x + 1)^\frac{1}{2} dx$ by substitution.
    * $u = (x + 1)^\frac{1}{2}$
    * $40 (\frac{1}{5}u^5 - \frac{1}{3}u^3) + C$
    * $8u^5 - \frac{40}{3}u^3 + C$
    * $8(x + 1)^\frac{5}{2} - \frac{40}{3}(x + 1)^\frac{3}{2} + C$
    * $8(\sqrt{x + 1})^5 - \frac{40}{3}(\sqrt{x + 1})^3 + C$

---

## Example 4

4. Evaluate $\int \cos x(\sin x + 1) dx$
    * Let $u = \sin x + 1$
    * $du = \cos x dx$
    * $\int u du$
    * $\frac{1}{2}u^2 + C$
    * $\frac{1}{2}(\sin x + 1)^2 + C$

---

## How Substitution Works

* The chain rule states that $\diff{x} F(g(x))dx = \diff{x} F(g(x)) [\diff{x} g(x)] = F'(g(x)) g'(x)$
* Reversing this statement and stating in terms of integrals: $\int F'(g(x)) g'(x)dx = F(g(x)) + C$
* If $u = g(x)$ and $du = g'(x) dx$: $\int F'(u) du = \int f(u)du = F(u) + C$.
* This also works for definite integrals: $\int_a^b f(g(x))g'(x) dx = \int_{g(a)}^{g(b)} f(u) du$.

---

## Example 5

5. Evaluate $\int_2^3 e^{2x} dx$
    * Let $u = 2x$
    * $du = 2dx, dx = \frac{du}{2}$
    * $x = 2, u = 4$ and $x = 2, u = 6$
    * $\frac{1}{2} \int_4^6 e^u du$
    * $\frac{1}{2}(e^u + C)\rvert_4^6$
    * $\frac{1}{2}(e^6 - e^4) \approx 174.415$

---

## Example 6

6. Evaluate the following definite integral using substitution: $\int_0^3 (\sqrt{x + 1}) dx$
    * $u = (x + 1)^\frac{1}{2}$
    * $u^2 = x + 1$
    * $2u du = dx$
    * $\int_\sqrt{0 + 1}^\sqrt{3 + 1}2u^2 du$
    * $2\int_1^2 u^2 du$
    * $2(\frac{1}{3}u^3)\rvert_1^2$

---

## Example 6, cont.

6. Evaluate the following definite integral using substitution: $\int_0^3 (\sqrt{x + 1}) dx$
    * $2(\frac{1}{3}u^3)\rvert_1^2$
    * $2(\frac{2^3 - 1^3}{3})$
    * $2(\frac{7}{3})$
    * $\frac{14}{3}$

---

## Exercise for Readers

* Evaluate the following:
    * $\int \cot x dx$
    * $\int \frac{2e^\sqrt{x}}{\sqrt{x}} dx$
    * $\int_0^2 \frac{x}{(2 + x^2)^2} dx$
    * $\int_3^4 \frac{1}{x - 1} dx$
        * using substitution
        * without substitution.

---

# [Next Lesson](Lesson%203)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Evaluate $\int \cot x dx$
    * $\int \frac{\cos x}{\sin x} dx$
    * Let $u = \sin x$, $du = \cos x dx$
    * $\int \frac{1}{u} du$
    * $\ln \lvert u \rvert + C$
    * $\ln \lvert \sin x \rvert + C$

---

## Answers to Exercises, cont.

* Evaluate $\int \frac{2e^\sqrt{x}}{\sqrt{x}} dx$
    * $\int 2e^{x^\frac{1}{2}}x^{-\frac{1}{2}} dx$
    * Let $u = x^\frac{1}{2}$, $du = \frac{1}{2}x^{-\frac{1}{2}} dx$
    * $2du = x^{-\frac{1}{2}} dx$
    * $4\int e^u du$
    * $4(e^u + C_1)$
    * $4e^\sqrt{x} + 4C_1$
    * $4e^\sqrt{x} + C$ ($C = 4C_1$)

---

## Answers to Exercises, cont.

* Evaluate $\int_0^2 \frac{x}{(2 + x^2)^2} dx$
    * Let $u = 2 + x^2$, $du = 2x dx$
    * $\int_2^6 \frac{1}{2}u^{-2} du$
    * $(-\frac{1}{2u})\rvert_2^6$
    * $\frac{1}{2(2)} - \frac{1}{2(6)}$
    * $\frac{3 - 1}{12}$
    * $\frac{1}{6}$

---

## Answers to Exercises, cont.

* Evaluate $\int_3^4 \frac{1}{x - 1} dx$ using substitution.
    * Let $u = x - 1$, $du = dx$
    * $\int_2^3 \frac{1}{u} du$
    * $(\ln \lvert u \rvert)\rvert_2^3$
    * $\ln 3 - \ln 2$
    * $\ln (\frac{3}{2})$

---

## Answers to Exercises, cont.

* Evaluate $\int_3^4 \frac{1}{x - 1} dx$ without substitution.
    * $(\ln \lvert x - 1 \rvert)\rvert_3^4$
    * $\ln \lvert 4 - 1 \rvert - \ln \lvert 3 - 1 \rvert$
    * $\ln 3 - \ln 2$
    * $\ln (\frac{3}{2})$

---

# [Next Lesson](Lesson%203)