---
marp: true
theme: uncover
class: invert
math: mathjax
---

$\newcommand\limit[2]{\displaystyle\lim_{#1 \to #2}}$

# <!--fit--> Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2025-->

$\newcommand\case[2]{#1 & \text{if} & #2}$

---

# Lesson 1: Intro to Limits

---

<!--paginate: true-->

## Intro

* Consider the following sequence: $\frac{1}{2}, \frac{1}{4}, \frac{1}{8}, \frac{1}{16}, \cdots$
* It can be expressed as $t_n = (\frac{1}{2})^n \text{ or } t_n = \frac{1}{2^n}$
* The sequence is infinite. The value slowly gets smaller and smaller towards zero as $n \to \infty$, but never reaches zero.
* We say that the 'limit' of the sequence is zero, as $n \to \infty$.
* Notation: $\limit{n}{\infty}(\frac{1}{2^n}) = 0$

---

## Limit Handedness

* Given $f(x) = x^2 - x - 6$, find $f(4)$
    * Since $f(4) = (4)^2 - 4 - 6 = 6$,
    * We can assume that $\limit{x}{4} (x^2 - x - 6) = 6$
* Here, the limit is the same as $f(4)$, but it won't always be. (*What? Why?*)
* The limit is how the function behaves around the point being considered, not the actual value.

---

## Limit Handedness

* To get the actual limit, we need to consider a 'Left'-handed and 'Right'-handed limit.
* We can take our example ($f(x) = x^2 - x - 6$) and consider what happens as we approach 4 from the left and the right.
* For the left, we get that $\limit{x}{4^-} f(x)= 6$
* For the right, we get that $\limit{x}{4^+} f(x)= 6$
* Since the limit exists for both sides, and they are both equal, the limit exists and is equal.

---

## Continuous Functions

* For many limits, you can find them by evaluating the function at the value that $x$ is approaching.
* This is true for all Continuous functions, or Continuous intervals where the limit is calculated.
* $f(x)$ is Continuous at $x = a$ if:
    * $f(a)$ exists.
    * $\limit{x}{a}(f(x))$ exists.
    * The quantities are equal.

---

## Continuous Example

1. Evaluate the following limit: $\limit{x}{3} [2x^2 - 4x]$
    * Since the function is continuous,
    * $\limit{x}{3} [2x^2 - 4x] = \limit{x}{3} [2(x^2 - 2x)]$ 
    * $\limit{x}{3} [2(x^2 - 2x)] = 2((3)^2 - 2(3))$
    * $\limit{x}{3} [2x^2 - 4x] = 2(9 - 6)$
    * $\limit{x}{3} [2x^2 - 4x] = 2(3) = 6$
* Evaluate $\limit{x}{20} [2x^2 - 10x]$ (ex. for reader)

---

## Piecewise Functions

* Some functions are defined by different rules in different parts of the domain.
* These are known as Piecewise Functions, and because of these different rules, there may be discontinuities at certain points.

---

## Types of Discontinuities

1. Absolute Continuity (Limit and Value Continuous)
2. Removable Discontinuity or "hole" (Limit Continuous)
3. Asymptotic Discontinuity ($x,y \to \pm \infty$ as $x,y \to c$)
4. Absolute Discontinuity or "gap" (Limit and Value Discontinuous)

In Pre-Calculus 12, you focused on levels 1-3 of Continuity. Piecewise functions can have any level of continuity. We'll be focusing on all four of these levels.

---

## Piecewise Example

2. Given $f(x) = \begin{cases} \case{x^2 - 2x + 1}{x < 1} \\ \case{3 - x}{x \ge 1} \end{cases}$
    * Find $\limit{x}{1} [f(x)]$
    * First, find the limit from the left: $\lim_{x \to 1^-}[f(x)]$
        * $(1)^2 - 2(1) + 1 \therefore \limit{x}{1^-}[f(x)] = 0$
    * Next, find the limit from the right: $\limit{x}{1^+}[f(x)]$
        * $3 - (1) \therefore \limit{x}{1^+}[f(x)] = 2$
    * The handed limits aren't equal, $\therefore \limit{x}{1}[f(x)]\ \text{DNE}$.

---

## Piecewise Exercises:

* Given $f(x) = \begin{cases}\case{-x^3}{x < -1} \\ \case{(x + 2)^2}{x > -1} \end{cases}$, find $\limit{x}{-1}[f(x)]$ (ex. for reader)
* Given $f(x) = \begin{cases}\case{2x}{x > 1} \\ x & \text{if} & x \le 1\end{cases}$
    * Evaluate $\limit{x}{1^-}[f(x)]$ (ex. for reader)
    * Evaluate $\limit{x}{1^+}[f(x)]$ (ex. for reader)
    * Evaluate $\limit{x}{1}[f(x)]$ (ex. for reader)

---

## Exercises for Readers

* Evaluate the limits for these continuous functions:
    * $\limit{x}{2}[2x^2 - x]$
    * $\limit{x}{10}[x^2 - 10x]$

---

## Exercises for Readers (cont.)

* Evaluate the following limits, given $f(x) = \begin{cases}\case{2x + 4}{x < -1} \\ \case{x^2}{-1 \le x < 2} \\ \case{6 - x}{x > 2} \end{cases}$
    * $\limit{x}{-1^+}[f(x)]$
    * $\limit{x}{-1^-}[f(x)]$
    * $\limit{x}{-1}[f(x)]$

---

## Exercises for Readers (cont.)

* Evaluate the following limits, given $f(x) = \begin{cases}\case{2x + 4}{x < -1} \\ \case{x^2}{-1 \le x < 2} \\ \case{6 - x}{x > 2} \end{cases}$
    * $\limit{x}{2^+}[f(x)]$
    * $\limit{x}{2^-}[f(x)]$
    * $\limit{x}{2}[f(x)]$

---

# [Next Lesson](Lesson%202)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Evaluate $\limit{x}{20} [2x^2 - 10x]$
    * $\limit{x}{20} [2x(x - 5)]$
    * $2(20)[(20) - 5]$
    * $40(15)$
    * $600$

---

## Answers to Exercises (cont.)

* Given $f(x) = \begin{cases}-x^3 & \text{if} & x < -1 \\ (x + 2)^2 & \text{if} & x > -1 \end{cases}$, find $\limit{x}{-1}[f(x)]$
    * $\limit{x}{-1^-}[f(x)] = -x^3$
    * $-(-1)^3$
    * $1$
    * $\limit{x}{-1^+}[f(x)] = (x + 2)^2$
    * $(1)^2$
* $\limit{x}{1}[f(x)] = 1$

---

## Answers to Exercises (cont.)

* Given $f(x) = \begin{cases}2x & \text{if} & x > 1 \\ x & \text{if} & x \le 1\end{cases}$
    * $\limit{x}{1^-}[f(x)] = 1$ 
    * $\limit{x}{1^+}[f(x)] = 2$
    * $\limit{x}{1}[f(x)]\ \text{DNE}$

---

## Answers to Exercises (cont.)

* Evaluate the limits for these continuous functions:
    * $\limit{x}{2}[2x^2 - x]$
        * $\limit{x}{2}[x(2x - 1)]$
        * $(2)[2(2) - 1]$
        * $2(4 - 1)$
        * $2(3)$
        * $6$

---

## Answers to Exercises (cont.)
* Evaluate the limits for these continuous functions:
    * $\limit{x}{10}[x^2 - 10x]$
        * $\limit{x}{10}[x(x - 10)]$
        * $(10)[(10) - 10]$
        * $10(0)$
        * $0$

---

## Answers to Exercises (cont.)

* Evaluate the following limits, given $f(x) = \begin{cases}\case{2x + 4}{x < -1} \\ \case{x^2}{-1 \le x < 2} \\ \case{6 - x}{x > 2} \end{cases}$
    * $\limit{x}{-1^+}[f(x)] = x^2$
        * $(-1)^2$
        * $1$

---

## Answers to Exercises (cont.)

* Evaluate the following limits, given $f(x) = \begin{cases}\case{2x + 4}{x < -1} \\ \case{x^2}{-1 \le x < 2} \\ \case{6 - x}{x > 2} \end{cases}$
    * $\limit{x}{-1^-}[f(x)] = 2x + 4$
        * $2(-1) + 4$
        * $-2 + 4$
        * $2$

---

## Answers to Exercises (cont.)

* Evaluate the following limits, given $f(x) = \begin{cases}\case{2x + 4}{x < -1} \\ \case{x^2}{-1 \le x < 2} \\ \case{6 - x}{x > 2} \end{cases}$
    * $\limit{x}{-1}[f(x)]$
        * $\limit{x}{-1}[f(x)]\ \text{DNE}$

---

## Answers to Exercises (cont.)

* Evaluate the following limits, given $f(x) = \begin{cases}\case{2x + 4}{x < -1} \\ \case{x^2}{-1 \le x < 2} \\ \case{6 - x}{x > 2} \end{cases}$
    * $\limit{x}{2^+}[f(x)] = 6 - x$
        * $6 - (2)$
        * $4$

---

## Answers to Exercises (cont.)

* Evaluate the following limits, given $f(x) = \begin{cases}\case{2x + 4}{x < -1} \\ \case{x^2}{-1 \le x < 2} \\ \case{6 - x}{x > 2} \end{cases}$
    * $\limit{x}{2^-}[f(x)] = x^2$
        * $(2)^2$
        * $4$
    * $\limit{x}{2}[f(x)] = 4$

---

# [Next Lesson](Lesson%202)