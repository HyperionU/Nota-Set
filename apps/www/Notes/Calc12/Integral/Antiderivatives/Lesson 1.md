---
marp: true
theme: uncover
class: invert
math: mathjax
---

$\newcommand\diff[1]{\mathcal{d}_{#1}}$
$\newcommand\eval[3]{\left. #1 \right|_{#2 = #3}}$

# <!--fit--> Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2025-->

$\newcommand\dd[2][]{\displaystyle\frac{d#1}{d#2}}$

---

# Lesson 1: The Antiderivative

---

<!--paginate: true-->

## Intro

* In prior units, you learned how to differentiate functions and equations. (Units 3 and 4)
* As such, differential equations are obtained, and how they can be used to observe rates of change. (Units 5 and 6)
* However, in many instances, it's useful to go back a step in the differentiation process and observe a function prior to differentiation.
* This process is known as **Integration**.

---

## Why use Integration?

* Throughout these final two units, you'll see examples as to why integration is so important.
* Just for now, we'll look at a concrete look at the mechanics (or plumbing) behind determining the antiderivative.
* Next unit, you'll get some techniques to quickly find the antiderivative or integral of certain functions (the porcelain).

---

## The Antiderivative

* Consider the following functions and their derivatives:
    * $y_1 = 2x^2, \diff{x} y_1 = 4x$
    * $y_2 = 2x^2 + 4, \diff{x} y_2 = 4x$
    * $y_3 = 2x^2 - 6, \diff{x} y_3 = 4x$
* Each of these contain a common $2x^2$ term, but the constant in each case is different. They're vertical translations of each other!
* But, their derivatives are the same. These functions are the *antiderivative* of $4x$.

---


## The Antiderivative, cont.

* It should be fair to say that $4x$ has an infinite number of antiderivatives, each with a different constant $C$ value attached to the $2x^2$ term.
* Therefore, if $\dd[y]{x} = 4x, y = 2x^2 + C$.

---

## Slope Fields

* A slope field for a differential equation gives a picture of its family of antiderivative functions.
* Each segment represents a portion of the tangent line at a particular point on an antiderivative function.
* Using the differential equation $\dd[y]{x} = 4x$:
    * At a point $(2, 1)$ on one of the antiderivative functions the slope will be equal to $\eval{\dd[y]{x}}{x}{2} = 4(2) = 8$

---

## What this means

* When we solve for the antiderivative, we get an infinite amount of vertically translated solutions, all differing by some constant $C$.

---

## The Indefinite Integral I: Differential Equations

* To understand the integral, we need to understand differential equations.
* A **differential equation** is an equation containing a quotient of differential terms.
* Basically, it is an equation which contains a derivative or a number of derivatives.
* From prior: $\dd[y]{x} = 4x$ is a differential equation.

---

## The Indefinite Integral II

* Previously, we'd solved the differential equation when we found all of the functions whose derivative is equal to the equation.
* Therefore the solution of $\dd[y]{x} = 4x$ is $y = 2x^2 + C$.
* Another way to represent this solution is the **Indefinite Integral**: $\int (4x) dx = 2x^2 + C$
* The $4x$ is the **integrand**, which is the derivative of the function we're trying to find. The $dx$ is the differential, representing the variable we're integrating with.

---

## Example 1

1. Evaluate the following indefinite integrals and verify by differentiating your result.
    * $\int 6 dx$
        * $6x + C$
        * $\diff{x} (6x + C) = 6$
    * $\int x dx$
        * $\frac{1}{2}x^2 + C$
        * $\diff{x} (\frac{1}{2}x^2 + C) = x$
    * $\int x^2 dx$

---

## Example 1, cont.

1. Evaluate the following indefinite integrals and verify by differentiating your result.
    * $\int x^2 dx$
        * $\frac{1}{3}x^3 + C$
        * $\diff{x} (\frac{1}{3}x^3 + C) = x^2$

* Throughout this example, you should see a pattern start to emerge.
* This is our **Reverse Power Rule**: $\int x^n dx = \frac{x^{n + 1}}{n + 1} + C, n \ne 1$. ($-1$ is an exception.)

---

## Example 2

2. Evaluate each indefinite integral:
    * $\int x^{10} dx$
        * $\int x^{10} dx = \frac{x^{10 + 1}}{10 + 1} + C = \frac{x^{11}}{11} + C$
    * $\int 20x^4 dx$
        * $\int 20x^4 dx = \frac{20x^{4 + 1}}{4 + 1} + C = 4x^5 + C$
    * $\int p^3 dp$
        * $\int p^3 dp = \frac{p^{3 + 1}}{3 + 1} + C = \frac{p^4}{4} + C$

---

## Evaluating Integrals (Diff. Eq.)

* Consider $\int x^{10} dx$ from previous example.
* Our differential equation is $\dd[y]{x} = x^{10}$
* Separate the differential components: $dy = x^{10} dx$
* Integrate both sides: $\int dy = \int x^{10} dx$ or $\int 1 dy = \int x^{10} dx$
* We get: $y + C_y = \frac{1}{11}x^{11} + C_x$
* And finally: $y = \frac{1}{11}x^{11} + C$

---

## Example 3

3. Evaluate $\int (\cos x) dx$
    * Method 1: Antidifferentiation
        * $\int (\cos x) dx = \sin x + C$
    * Method 2: Solving Differential Equation
        * $\dd[y]{x} = \cos x$
        * $dy = \cos x dx$
        * $\int dy = \int \cos x dx$
        * $y + C_y = \sin x + C_x$
        * $y = \sin x + C$

---

## Example 4

4. Evaluate $\int \sqrt[3]{x} dx$
    * $\int x^\frac{1}{3} dx$
    * $\frac{x^{\frac{1}{3} + 1}}{\frac{1}{3} + 1} + C$
    * $\frac{x^{\frac{4}{3}}}{\frac{4}{3}} + C$
    * $\frac{3}{4}x^{\frac{4}{3}} + C$

* Similarly, integrating a sum or difference is similar to differentiating: $\int[f(x) \pm g(x)]dx = \int f(x) dx \pm \int g(x) dx$

---

## Example 5

5. Evaluate $\int (3x^2 - 10x + 11) dx$
    * $\int (3x^2) dx - \int (10x) dx + \int (11) dx$
    * $(\frac{3x^{2 + 1}}{2 + 1} + C_1) - (\frac{10x^{1 + 1}}{1 + 1} + C_2) + (11x + C_3)$
    * $(\frac{3x^{3}}{3}) - (\frac{10x^{2}}{2}) + 11x + C$
    * $x^3 - 5x^2 + 11x + C$

---

## Fundamental Integration Laws

1. Constant: $\int kf(x) dx = k \int f(x) dx, \int a dx = ax + C$
2. Sum / Difference: $\int[f(x) \pm g(x)]dx = \int f(x) dx \pm \int g(x) dx$
3. Reverse Power: $\int x^n dx = \frac{1}{n + 1} x^{n + 1} + C$
4. Cosine: $\int \cos x dx = \sin x + C$
5. Sine: $\int \sin x dx = C - \cos x$
6. Exponential: $\int (b^x \ln b) dx = b^x + C$
7. Logarithmic: $\int \frac{1}{x \ln b} dx = \log_b |x| + C$

---

## Example 6

6. Evaluate $\int (e^x + x^\frac{2}{3} - \frac{1}{x}) dx$
    * $e^x + \frac{3}{5}x^\frac{5}{3} - \ln |x| + C$

---

## Porcelain I: $u$-Substitution

* Consider $\int [(2x)^3] dx$. What is its integral?
* We can't use the Reverse Power rule, since our base is no longer just $x$.
* *Couldn't we just expand this out?* Sure, we can. But what happens when we get some very complicated integrands?
* Here's an easier way: $u$-substitution.

---

## $u$-Substitution, cont.

* Okay, starting with $\int [(2x)^3] dx$
* Let $u = 2x$.
* $u = 2x \implies du = 2 dx$ or $dx = \frac{1}{2} du$
* We get $\int u^3 \frac{1}{2} du$,
* then $\frac{1}{2} \int u^3 du$,
* $\frac{1}{8} u^4 + C$,
* and finally $\int [(2x)^3] dx = \frac{1}{8} (2x)^4 + C$
* *Expanding this out would be way easier.* 
* I know. But, we now have a shortcut for more complex integrands.

---

## Example 7

7. Simplify $\int (10x + 7)^8 dx$
    * Okay. There's no way we're expanding this out.
    * Let $u = 10x + 7, du = 10 dx$
    * $\int u^8 \frac{du}{10}$
    * $\frac{1}{10} \int u^8 du$
    * $\frac{1}{10} \frac{1}{9} u^9 + C$
    * $\frac{1}{90} u^9 + C$
    * $\frac{1}{90} (10x + 7)^9 + C$
* *Okay, I get it now.*

---

## Note: Porcelain v Plumbing

* *What do you mean by 'Porcelain' and 'Plumbing'?*
* These terms come from tech, specifically from `git`.
* Porcelain would be the more 'user-friendly' commands (`commit`, `branch`, etc.)
* Plumbing would be the internals. While not necessarily user-friendly, they are used in some case.
* *So, in this case, 'porcelain' would be the shortcuts and fundamental integration laws, while the 'plumbing' would be the full process?* Absolutely.

---

## Example 8

8. Evaluate $\int [(\sqrt{5x^2 + 8})(20x)] dx$
    * Woah, okay then. Let's start simple.
    * $\int [(5x^2 + 8)^\frac{1}{2}(20x)] dx$
    * Let $u = 5x^2 + 8, du = 10x dx$
    * $\int (u)^\frac{1}{2}(20x) \frac{du}{10x}$
    * $\int 2(u)^\frac{1}{2} du$
    * $2 \frac{(u)^{\frac{1}{2} + 1}}{\frac{1}{2} + 1}$
    * $\frac{4}{3} (u)^\frac{3}{2} = \frac{4}{3} (5x^2 + 8)^\frac{3}{2}$

---

## Example 9

9. Evaluate $\int \sin (10x) dx$
    * Let $u = 10x, du = 10 dx$
    * $\int \sin u \frac{1}{10} du$
    * $\frac{1}{10} \int \sin u du$
    * $\frac{1}{10} (-\cos u) + C$
    * $-\frac{1}{10}\cos 10x + C$

---

## Example 10

10. Evaluate $\int (e^{4x^2})(2x) dx$
    * Let $u = 4x^2, du = 8x dx$
    * $\int (e^u)(2x) \frac{du}{8x}$
    * $\int (e^u)\frac{1}{4}du$
    * $\frac{1}{4} \int e^u du$
    * $\frac{1}{4} e^u + C$
    * $\frac{1}{4} e^{4x^2} + C$

---

## Example 11

11. Evaluate $\int [\frac{1}{7x} + \frac{1}{(7x)^2}] dx$
    * Oh god. We can do this.
    * $\int \frac{1}{7x} dx + \int \frac{1}{(7x)^2} dx$
    * $\frac{1}{7} \int \frac{1}{x} dx + \int (7x)^{-2} dx$
    * $\frac{1}{7} \ln |x| + C_1 + \int (7x)^{-2} dx$
    * Let $u = 7x, du = 7 dx$
    * $\frac{1}{7} \ln |x| + C_1 + \int u^{-2} \frac{du}{7}$
    * $\frac{1}{7} \ln |x| + C_1 + \frac{1}{7} \int u^{-2} du$

---

## Example 11, cont.

11. Evaluate $\int [\frac{1}{7x} + \frac{1}{(7x)^2}] dx$
    * $\frac{1}{7} \ln |x| + C_1 + \frac{1}{7} \int u^{-2} du$
    * $\frac{1}{7} \ln |x| + C_1 - \frac{1}{7} u^{-1} + C_2$
    * $\frac{1}{7} \ln |x| - \frac{1}{7} u^{-1} + C$
    * *Huh. That was easier than I thought.*

---

## Example 12

12. Evaluate $\int (\sin^3 x)(\cos x) dx$
    * $\int (\sin x)^3(\cos x) dx$
    * Let $u = \sin x, du = \cos x dx$
    * $\int u^3 (\cos x) \frac{du}{\cos x}$
    * $\int u^3 du$
    * $\frac{1}{4}u^4 + C$
    * $\frac{1}{4} \sin^4 x + C$

---

## Exercise for Readers

* Solve the following differential equations:
    * $\dd[y]{x} = -3x^2 - 2x + 1$
    * $\dd[p]{z} = \frac{3}{z} - \frac{3}{z^2} + \frac{2}{z^3}, z \ne 0$
    * $\dd[y]{x} = \sec^2 x$
    * $\dd[u]{y} = y - \cos y$

---

## Exercise for Readers, cont.

* Evaluate each indefinite integral
    * $\int x^5 dx$
    * $\int 5^x (\ln 5) dx$
    * $\int (\sin^2 x + \cos^2 x) dx$
    * $\int 27e^x dx$
    * $\int (5x - 3)^{12} dx$
    * $\int (\sqrt{4x^2 - 10x})(4x - 5)dx$
    * $\int (\cos^4 8x)(\sin 8x) dx$
    * $\int e^{\ln 4x} (\frac{1}{x}) dx$

---

# [Next Lesson](Lesson%202)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Solve the following differential equation: $\dd[y]{x} = -3x^2 - 2x + 1$
    * $dy = -(3x^2 + 2x - 1) dx$
    * $\int dy = \int -(3x^2 + 2x - 1) dx$
    * $y = -(\frac{1}{3}3x^3 + \frac{1}{2}2x^2 - x) + C$
    * $y = -x^3 - x^2 + x + C$

---

## Answers to Exercises, cont.

* Solve the following differential equation: $\dd[p]{z} = \frac{3}{z} - \frac{3}{z^2} + \frac{2}{z^3}, z \ne 0$
    * $dp = (\frac{3}{z} - \frac{3}{z^2} + \frac{2}{z^3}) dz$
    * $\int dp = \int (\frac{3}{z} - \frac{3}{z^2} + \frac{2}{z^3}) dz$
    * $\int dp = \int 3(\frac{1}{z}) dz - \int 3(z^{-2}) dz + \int 2(z^{-3}) dz$
    * $p = 3 \ln |z| + \frac{3}{z} - z^{-2} + C$

---

## Answers to Exercises, cont.

* Solve the following differential equation: $\dd[y]{x} = \sec^2 x$
    * $dy = \sec^2 x dx$
    * $\int dy = \int \sec^2 x dx$
    * $y = \tan x$

---

## Answers to Exercises, cont.

* Solve the following differential equation: $\dd[u]{y} = y - \cos y$
    * $du = (y - \cos y) dy$
    * $\int du = \int (y - \cos y) dy$
    * $u = \frac{1}{2}y^2 - \sin y + C$

---

## Answers to Exercises, cont.

* Evaluate $\int x^5 dx$
    * $\frac{1}{6}x^6 + C$
* Evaluate $\int 5^x (\ln 5) dx$
    * $5^x + C$
* Evaluate $\int (\sin^2 x + \cos^2 x) dx$
    * $\int 1 dx$
    * $x + C$
* Evaluate $\int 27e^x dx$
    * $27e^x + C$

---

## Answers to Exercises, cont.

* Evaluate $\int (5x - 3)^{12} dx$
    * Let $u = 5x - 3, du = 5 dx$
    * $\int u^{12} \frac{1}{5}du$
    * $\frac{1}{5}\frac{1}{13} u^{13}$
    * $\frac{1}{65} (5x - 3)^{13}$

---

## Answers to Exercises, cont.

* Evaluate $\int (\sqrt{4x^2 - 10x})(4x - 5)dx$
    * $\frac{1}{2} \int 2(\sqrt{4x^2 - 10x})(4x - 5)dx$
    * $\frac{1}{2} \int (4x^2 - 10x)^\frac{1}{2}(8x - 10)dx$
    * Let $u = 4x^2 - 10x, du = 8x - 10 dx$
    * $\frac{1}{2} \int u^\frac{1}{2} du$
    * $\frac{1}{2} \frac{2}{3} u^\frac{3}{2} + C$
    * $\frac{1}{3} (4x^2 - 10x)^\frac{3}{2} + C$

---

## Answers to Exercises, cont.

* Evaluate $\int (\cos^4 8x)(\sin 8x) dx$
    * $\int (\cos 8x)^4(\sin 8x) dx$
    * Let $u = \cos 8x, du = -8 \sin 8x dx$
    * $\int u^4(\sin 8x) \frac{du}{-8 \sin 8x}$
    * $-\frac{1}{8} \int u^4 du$
    * $-\frac{1}{8}\frac{1}{5}u^5$
    * $-\frac{1}{40} \cos^5 8x + C$

---

## Answers to Exercises, cont.

* Evaluate $\int e^{\ln 4x} (\frac{1}{x}) dx$
    * $\int 4x (\frac{1}{x}) dx$
    * $\int 4 dx$
    * $4x + C$

---

# [Next Lesson](Lesson%202)