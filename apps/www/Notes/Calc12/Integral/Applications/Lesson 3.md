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

# Lesson 3: Integration by Partial Fractions

---

<!--paginate: true-->

## Intro

* The method of partial fraction decomposition as an integration technique involves breaking down an integrand that contains a quotient of polynomials into simpler fractions.
* Consider the integral $\int \frac{A(x)}{B(x)} dx$, where $A(x), B(x)$ are polynomials in $x$.
* There are two cases dependent on whether $A(x)$ or $B(x)$ has a higher degree.

---

## Case I: $\deg A(x) \ge \deg B(x)$

* The first step is to divide the polynomials, producing a quotient polynomial and a remainder.
* The quotient can then be integrated using any prior technique.
* The remainder (if not zero) will then be a fraction where the degree of the denominator is greater than the numerator (Case II).
* Basically: $\int \frac{A(x)}{B(x)} dx = \int Q(x) dx + \int \frac{R(x)}{B(x)} dx$.

---

## Example 1

1. Evaluate the integral using partial fraction decomposition: $\int \frac{2x^2 - x + 1}{x + 1} dx$
    * $\frac{2x^2 - x + 1}{x + 1} = 2x - 3 + \frac{4}{x + 1}$
    * $\int (2x - 3) dx + \int \frac{4}{x + 1} dx$
    * $(\frac{1}{2}2x^2 - 3x + C_1) + (4\ln \lvert x + 1 \rvert + C_2)$
    * $x^2 - 3x + 4\ln \lvert x + 1 \rvert + C$
* In this case, the remainder was a constant and did not requre additional decomposition. Otherwise, this reverts to Case II.

---

## Case II: $\deg A(x) < \deg B(x)$

* First, let's review addition of polynomial fractions. We'll look at the reverse process after for decomposition.
* Consider $\frac{1}{x + 1} + \frac{2}{x + 2}$. If this was the integrand, the solution would be $\ln \lvert x + 1 \rvert + \ln \lvert x + 2 \rvert + C, x \ne -1, -2$
* Now, let's add the fractions using common denominators, distributing and adding:
    * $\frac{x + 2 + 2(x + 1)}{(x + 1)(x + 2)}$
    * $\frac{3x + 4}{x^2 + 3x + 2}$

---

## Case II, cont.

* If $\frac{3x + 4}{x^2 + 3x + 2}$ was the integrand, the solution would not be apparent using previous techniques.
* So, let's rewrite it using Partial Fraction Decomposition:
    * Factor the denominator and split: $\frac{3x + 4}{x^2 + 3x + 2} = \frac{A}{x + 1} + \frac{B}{x + 2}$
    * $3x + 4 = A(x + 2) + B(x + 1)$
    * $3x + 4 = (A + B)x + (2A + B)$
    * $\begin{cases}A + B = 3 \\ 2A + B = 4\end{cases}$

---

## Case II, cont.

* $\begin{cases}A + B = 3 \\ 2A + B = 4\end{cases}$
* $\begin{cases}2A + 2B = 6 \\ 2A + B = 4\end{cases}$
* $\begin{cases}A + B = 3 \\ B = 2\end{cases}$
* $\begin{cases}A = 1 \\ B = 2\end{cases}$
* $\frac{3x + 4}{x^2 + 3x + 2} = \frac{1}{x + 1} + \frac{2}{x + 2}$ (The process is complete!)

---

## More Partial Fractions

* Before proceeding with Case II examples, it is useful to indicate some of the different types of partial fractions we can encounter.
* Types of Partial Fractions:
    * Case II.1: Numerator is constant. Decomposition is not required, but can be used.
    * Case II.2: Denominator is product of linear factors. See prior.


---

## More Partial Fractions, cont. 

* Types of Partial Fractions:
    * Case II.3: Denominator is a repeated linear term. An example is shown below:
        * $\frac{x + 1}{(x + 3)^2} = \frac{A}{x + 3} + \frac{B}{(x + 3)^2}$.
    * This works with the denominator multiplicity greater than two.
    * $\frac{A(x)}{(x + \alpha)^k} = \frac{A}{x + \alpha} + \frac{B}{(x + \alpha)^2} + \dots + \frac{C}{(x + \alpha)^k}$.
    * Case II.4: Denominator is a reducible polynomial of degree 2 or higher. See example.

---

## Example 2

2. Evaluate $\int \frac{1}{x^2 - 25} dx$
    * $\frac{1}{(x + 5)(x - 5)} = \frac{A}{x + 5} + \frac{B}{x - 5}$
    * $1 = A(x - 5) + B(x + 5)$
    * $\begin{cases}A + B = 0 \\ -5A + 5B = 1\end{cases}$
    * $\begin{cases}A + B = 0 \\ 10B = 1\end{cases}$
    * $\begin{cases}A = -\frac{1}{10} \\ B = \frac{1}{10}\end{cases}$

---

## Example 2, cont.

2. Evaluate $\int \frac{1}{x^2 - 25} dx$
    * $\begin{cases}A = -\frac{1}{10} \\ B = \frac{1}{10}\end{cases}$
    * $\frac{1}{(x + 5)(x - 5)} = \frac{1}{-10(x + 5)} + \frac{1}{10(x - 5)}$
    * $-\frac{1}{10}\int \frac{1}{x + 5} dx + \frac{1}{10} \int \frac{1}{x - 5}dx$
    * $-\frac{1}{10}\\ln \lvert x + 5 \rvert + \frac{1}{10} \ln \lvert x - 5 \rvert + C$

---

## More Partial Fractions, cont.

* Types of Partial Fractions:
    * Case II.5: Denominator as a non-reducible quadratic term. An example is shown below:
    * Evaluate $\int \frac{x - 1}{(x^2 + 1)(x + 1)} dx$
    * $\frac{x - 1}{(x^2 + 1)(x + 1)} = \frac{Ax + B}{(x^2 + 1)} + \frac{C}{x + 1}$
    * $x - 1 = (Ax + B)(x + 1) + C(x^2 + 1)$
    * $x - 1 = (A + C)x^2 + (A + B)x + B + C$
    * $\begin{cases}A + C = 0 \\ A + B = 1 \\ B + C = -1\end{cases}$

---

## More Partial Fractions, cont.

* Evaluate $\int \frac{x - 1}{(x^2 + 1)(x + 1)} dx$
    * $\frac{x - 1}{(x^2 + 1)(x + 1)} = \frac{Ax + B}{(x^2 + 1)} + \frac{C}{x + 1}$
    * $\begin{cases}A + C = 0 \\ A + B = 1 \\ B + C = -1\end{cases}$
    * $\begin{cases}A = 1 \\ B = 0 \\ C = -1\end{cases}$
    * $\int \frac{x}{(x^2 + 1)} - \frac{1}{x + 1} dx$

---

## More Partial Fractions, cont.

* Evaluate $\int \frac{x - 1}{(x^2 + 1)(x + 1)} dx$
    * $\int \frac{x}{(x^2 + 1)} - \frac{1}{x + 1} dx$
    * $\int \frac{x}{(x^2 + 1)} dx - \int \frac{1}{x + 1} dx$
        * $u = x^2 + 1, du = 2x dx$
    * $\frac{1}{2} \int \frac{1}{u} du - \int \frac{1}{x + 1} dx$
    * $\frac{\ln \lvert x^2 + 1 \rvert}{2} - \ln \lvert x + 1 \rvert + C$
* Case II.6: Combinations of other types of partial frations. Can be solved by following the patterns presented already.

---

## Example 3

3. Evaluate $\int \frac{x}{x^4 + 3x^2 + 2} dx$
    * $\frac{x}{(x^2 + 1)(x^2 + 2)} = \frac{Ax + B}{(x^2 + 1)} + \frac{Cx + D}{(x^2 + 2)}$
    * $x = (Ax + B)(x^2 + 2) + (Cx + D)(x^2 + 1)$
    * $x = (A + C)x^3 + (2A + C)x + (B + D)x^2 + (2B + D)$
    * $\begin{cases}A + C = 0 \\ B + D = 0 \\ 2A + C = 1 \\ 2B + D = 0\end{cases}$

---

## Example 3, cont.

3. Evaluate $\int \frac{x}{x^4 + 3x^2 + 2} dx$
    * $\frac{x}{(x^2 + 1)(x^2 + 2)} = \frac{Ax + B}{(x^2 + 1)} + \frac{Cx + D}{(x^2 + 2)}$
    * $\begin{cases}A + C = 0 \\ B + D = 0 \\ 2A + C = 1 \\ 2B + D = 0\end{cases}$
    * $\begin{cases}A = 1 \\ B = 0 \\ C = -1 \\ D = 0\end{cases}$

---

## Example 3, cont.

3. Evaluate $\int \frac{x}{x^4 + 3x^2 + 2} dx$
    * $\frac{x}{(x^2 + 1)(x^2 + 2)} = \frac{Ax + B}{(x^2 + 1)} + \frac{Cx + D}{(x^2 + 2)}$
    * $\begin{cases}A = 1 \\ B = 0 \\ C = -1 \\ D = 0\end{cases}$
    * $\int \frac{x}{(x^2 + 1)} - \frac{x}{(x^2 + 2)} dx$
        * $u = x^2 + 1, du = 2x dx, v = x^2 + 2, dv = 2x dx$
    * $\frac{1}{2}\int \frac{1}{u} du - \frac{1}{2} \int \frac{1}{v} dv$

---

## Example 3, cont.

3. Evaluate $\int \frac{x}{x^4 + 3x^2 + 2} dx$
    * $u = x^2 + 1, v = x^2 + 2$
    * $\frac{1}{2}\int \frac{1}{u} du - \frac{1}{2} \int \frac{1}{v} dv$
    * $\frac{\ln \lvert x^2 + 1 \rvert}{2} - \frac{\ln \lvert x^2 + 2 \rvert}{2} + C$

---

## Exercise for Readers

* Solve the following:
    * $\int \frac{x + 1}{x^2} dx$
    * $\int \frac{x^3 - x^2 - 1}{x + 1} dx$
    * $\int \frac{1}{2x^2 - 2} dx$
    * $\int \frac{x + 2}{(x + 1)^2} dx$
    * $\int_3^4 \frac{-x - 1}{x^2 - 3x + 2} dx$
    * $\int_3^4 \frac{2x - 4}{2(x - 2)^2} dx$ 

---

# [Next Lesson](Lesson%204)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Solve $\int \frac{x + 1}{x^2} dx$
    * Algebraic Manipulation:
        * $\int \frac{1}{x} dx + \int \frac{1}{x^2} dx$
        * $\ln \lvert x \rvert - \frac{1}{x} + C$
    * Partial Fraction Decomposition (PFD):
        * $\frac{x + 1}{x^2} = \frac{A}{x} + \frac{B}{x^2}$
        * $x + 1 = Ax + B$
        * $\int \frac{1}{x} dx + \int \frac{1}{x^2} dx$
        * $\ln \lvert x \rvert - \frac{1}{x} + C$

---

## Answers to Exercises, cont.

* Solve $\int \frac{x^3 - x^2 - 1}{x + 1} dx$
    * $\frac{x^3 - x^2 - 1}{x + 1} = x^2 - 2x + 2 - \frac{3}{x + 1}$
    * $\int x^2 dx - \int 2x dx + \int 2 dx - \int \frac{3}{x + 1} dx$
    * $\frac{1}{3} x^3 - x^2 + 2x - 3\ln \lvert x + 1 \rvert + C$

---

## Answers to Exercises, cont.

* Solve $\int \frac{1}{2x^2 - 2} dx$
    * $\int \frac{1}{2(x^2 - 1)} dx$
    * $\frac{1}{2}\int \frac{1}{x^2 - 1} dx$
    * $\frac{1}{(x + 1)(x - 1)} = \frac{A}{x + 1} + \frac{B}{x - 1}$
    * $1 = A(x - 1) + B(x + 1)$
    * $1 = (A + B)x + (-A + B)$
    * $\frac{1}{2}(-\frac{1}{2} \int \frac{1}{x + 1} dx + \frac{1}{2} \int \frac{1}{2x - 1} dx)$
    * $-\frac{1}{4} \ln \lvert x + 1 \rvert + \frac{1}{4} \ln \lvert x - 1 \rvert + C$

---

## Answers to Exercises, cont.

* Solve $\int \frac{x + 2}{(x + 1)^2} dx$
    * $\frac{x + 2}{(x + 1)^2} = \frac{A}{x + 1} + \frac{B}{(x + 1)^2}$
    * $x + 2 = Ax + (A + B)$
    * $\int \frac{1}{x + 1} dx + \int \frac{1}{(x + 1)^2} dx$
        * $u = x + 1, du = dx$
    * $\int \frac{1}{x + 1} dx + \int \frac{1}{u^2} du$
    * $\ln \lvert x + 1 \rvert - \frac{1}{x + 1} + C$

---

## Answers to Exercises, cont.

* Solve $\int_3^4 \frac{-x - 1}{x^2 - 3x + 2} dx$
    * $-\int_3^4 \frac{x + 1}{(x - 2)(x - 1)} dx$
    * $\frac{x + 1}{(x - 2)(x - 1)} = \frac{A}{x - 2} + \frac{B}{x - 1}$
    * $x + 1 = (A + B)x - (A + 2B)$
    * $-\int_3^4 \frac{3}{x - 2} + \frac{-2}{x - 1} dx$
    * $-(3\ln \lvert x - 2 \rvert)_3^4 - (2\ln \lvert x - 1 \rvert)_3^4$
    * $-[5\ln 2 + 2\ln 3]$
    * $-\ln \frac{32}{9}$

---

## Answers to Exercises, cont.

* Solve $\int_3^4 \frac{2x - 4}{2(x - 2)^2} dx$
    * $\int_3^4 \frac{1}{x - 2} dx$
    * $(\ln \lvert x - 2 \rvert)\rvert_3^4$
    * $\ln 2$

---

# [Next Lesson](Lesson%204)