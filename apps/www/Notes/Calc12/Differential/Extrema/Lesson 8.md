---
marp: true
theme: uncover
class: invert
math: mathjax
---

$\newcommand\diff[1]{\mathcal{d}_{#1}}$
$\newcommand\limit[2]{\displaystyle\lim_{#1 \to #2}}$

# <!--fit--> Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2025-->

$\newcommand\dd[3][]{\displaystyle\frac{d^{#1}#2}{d#3^{#1}}}$
$\newcommand\case[2]{#1 & \text{if} & #2}$

---

# Lesson 8: Oblique Asymptotes

---

<!--paginate: true-->

## Intro 

* An asymptote is a line that a function approaches, but never reaches.
* Previously, we've discussed vertical and horizontal asymptotes.
* Now, we're discussing a very different asymptote: *Oblique* asymptotes.
* These are defined using the slope-intercept form of a line, such that $m \ne 0$.

---

## Determining Oblique Asymptotes

* In general, a function $y = f(x)$ has an oblique asymptote at $y = mx + b$ if either:
    * $\limit{x}{\infty} [f(x) - (mx + b)] = 0$, or
    * $\limit{x}{-\infty} [f(x) - (mx + b)] = 0$
* Similarly with horizontal asymptotes, we use division to determine the equation of the asymptote.
* Typically, rational functions have oblique asymptotes if $\deg N - \deg D = 1$.

---

## Example 1

1. Find the equation of the oblique asymptote of $f(x) = \frac{3x^2 - 2x + 1}{x + 2}$
    * First, complete the division.
        * $
    \begin{array}{c|rrrr}
        & 3 & -2 & 1 \\
        -2 & \downarrow & -6 & 16  \\
        \hline
        & 3 & -8 & 17 \\
    \end{array}$
    * Next, write as a division statement:
        * $\frac{3x^2 - 2x + 1}{x + 2} = 3x - 8 + \frac{17}{x + 2}$

---

## Example 1, cont.

1. Find the equation of the oblique asymptote of $f(x) = \frac{3x^2 - 2x + 1}{x + 2}$
    * $f(x) = 3x - 8 + \frac{17}{x + 2}$
    * $f(x) - (3x - 8) = \frac{17}{x + 2}$
    * Next, evaluate the limit:
        * $\limit{x}{\infty} [f(x) - (3x - 8)] = \limit{x}{\infty} \frac{17}{x + 2}$
        * $\limit{x}{\infty} [f(x) - (3x - 8)] = \limit{x}{\infty} \frac{\frac{17}{x}}{\frac{x}{x} + \frac{2}{x}}$

---

## Example 1, cont.

1. Find the equation of the oblique asymptote of $f(x) = \frac{3x^2 - 2x + 1}{x + 2}$
    * $\limit{x}{\infty} [f(x) - (3x - 8)] = \limit{x}{\infty} \frac{\frac{17}{x}}{\frac{x}{x} + \frac{2}{x}}$
    * $\limit{x}{\infty} [f(x) - (3x - 8)] = \limit{x}{\infty} \frac{\frac{17}{x}}{1 + \frac{2}{x}}$
    * $\limit{x}{\infty} [f(x) - (3x - 8)] = 0$
    * Since this is zero, there is an oblique asymptote at $y = 3x - 8$.

---

## Example 2

2. Find the equation of the oblique asymptote of $f(x) = \frac{2x^2 + 5x - 1}{x + 2}$
    * $
    \begin{array}{c|rrrr}
        & 2 & 5 & -1 \\
        -2 & \downarrow & -4 & -2 \\
        \hline
        & 2 & 1 & -3 \\
    \end{array}$
    * $\frac{2x^2 + 5x - 1}{x + 2} = 2x + 1 + \frac{-3}{x + 2}$
    * $f(x) = 2x + 1 - \frac{3}{x + 2}$
    * $f(x) - (2x + 1) = -\frac{3}{x + 2}$

---

## Example 2, cont.

2. Find the equation of the oblique asymptote of $f(x) = \frac{2x^2 + 5x - 1}{x + 2}$
    * $f(x) - (2x + 1) = -\frac{3}{x + 2}$
    * $\limit{x}{\infty} [f(x) - (2x + 1)] = \limit{x}{\infty} -\frac{3}{x + 2}$
    * $\limit{x}{\infty} [f(x) - (2x + 1)] = \limit{x}{\infty} -\frac{\frac{3}{x}}{\frac{x}{x} + \frac{2}{x}}$
    * $\limit{x}{\infty} [f(x) - (2x + 1)] = \limit{x}{\infty} -\frac{\frac{3}{x}}{1 + \frac{2}{x}}$

---

## Example 2, cont.

2. Find the equation of the oblique asymptote of $f(x) = \frac{2x^2 + 5x - 1}{x + 2}$
    * $\limit{x}{\infty} [f(x) - (2x + 1)] = \limit{x}{\infty} -\frac{\frac{3}{x}}{1 + \frac{2}{x}}$
    * $\limit{x}{\infty} [f(x) - (2x + 1)] = 0$
    * OA: $y = 2x + 1$

---

## Example 3

3. Find the equation of the oblique asymptote of $f(x) = \frac{4x^3 - 2x^2 + 3x + 5}{x^2 - x}$
$
    \begin{array}{rll}
        4x + 2 \phantom{0}\\
        x^2 - x \enclose{longdiv}{4x^3 - 2x^2 + 3x + 5} \\
        - \underline{4x^3 + 4x^2 \phantom{000000000}}\\
        2x^2 + 3x\phantom{0000}\\
        - \underline{2x^2 - 2x \phantom{0000}}\\
        5x + 5
    \end{array}
$

---

## Example 3, cont.

3. Find the equation of the oblique asymptote of $f(x) = \frac{4x^3 - 2x^2 + 3x + 5}{x^2 - x}$
    * So $f(x) = 4x + 2 + \frac{5x + 5}{x^2 - x}$
    * $f(x) - (4x + 2) = \frac{5x + 5}{x^2 - x}$
    * $\limit{x}{\infty} [f(x) - (4x + 2)] = \limit{x}{\infty} \frac{5x + 5}{x^2 - x}$
    * $\limit{x}{\infty} [f(x) - (4x + 2)] = \limit{x}{\infty} \frac{\frac{5x}{x^2} + \frac{5}{x^2}}{\frac{x^2}{x^2} - \frac{x}{x^2}}$

---

## Example 3, cont.

3. Find the equation of the oblique asymptote of $f(x) = \frac{4x^3 - 2x^2 + 3x + 5}{x^2 - x}$
    * $\limit{x}{\infty} [f(x) - (4x + 2)] = \limit{x}{\infty} \frac{\frac{5x}{x^2} + \frac{5}{x^2}}{\frac{x^2}{x^2} - \frac{x}{x^2}}$
    * $\limit{x}{\infty} [f(x) - (4x + 2)] = \limit{x}{\infty} \frac{\frac{5}{x} + \frac{5}{x^2}}{1 - \frac{1}{x}}$
    * $\limit{x}{\infty} [f(x) - (4x + 2)] = 0$
    * OA: $y = 4x + 2$

---

## Exercise for Readers

* Does the following have an oblique asymptote?
    * $f(x) = \frac{3x^2 - x}{x + 7}$
    * $f(x) = \frac{-5x + 2}{x - 3}$
    * $f(x) = \frac{3x^2 + 4}{x}$
    * $f(x) = \frac{3x^3 - x^2}{x^2 + 5}$
    * $f(x) = \frac{6x^3 + 2x^2 + 3x + 1}{-7x^3 + x}$
    * $f(x) = \frac{4x^4 + 6}{2x^2 - 1}$

---

## Exercise for Readers

* Determine the oblique asymptote of 
    * $f(x) = \frac{2x^2 + 3}{x}$
    * $f(x) = \frac{3x^2 - 7x}{x - 2}$
    * $f(x) = \frac{6x^3 - 5x}{x^2 + 1}$
    * $f(x) = \frac{-4x^3 + 2x^2 + x - 4}{x^2 - 2x}$

---

# [Next Unit](../Applications/Lesson%201)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Does $f(x) = \frac{3x^2 - x}{x + 7}$ have an oblique asymptote?
    * Yes, $\deg N - \deg D = 1$
* Does $f(x) = \frac{-5x + 2}{x - 3}$ have an oblique asymptote?
    * N0, $\deg N = \deg D$
* Does $f(x) = \frac{3x^2 + 4}{x}$ have an oblique asymptote?
    * Yes, $\deg N - \deg D = 1$

---

## Answers to Exercises, cont.

* Does $f(x) = \frac{3x^3 - x^2}{x^2 + 5}$ have an oblique asymptote?
    * Yes, $\deg N - \deg D = 1$
* Does $f(x) = \frac{6x^3 + 2x^2 + 3x + 1}{-7x^3 + x}$ have an oblique asymptote?
    * No, $\deg N = \deg D$
* Does $f(x) = \frac{4x^4 + 6}{2x^2 - 1}$ have an oblique asymptote?
    * No, $\deg N - \deg D > 1$

---

## Answers to Exercises, cont.

* Determine the oblique asymptote of $f(x) = \frac{2x^2 + 3}{x}$

$
    \begin{array}{rll}
        2x + 0\phantom{0}\\
        x \enclose{longdiv}{2x^2 + 0x + 3} \\
        - \underline{2x^2 \phantom{00000000}}\\
        2x^2 + 0x\phantom{0000}\\
        - \underline{0x \phantom{0000}}\\
        0x + 3
    \end{array}
$

---

## Answers to Exercises, cont.

* Determine the oblique asymptote of $f(x) = \frac{2x^2 + 3}{x}$
    * $f(x) = 2x + \frac{3}{x}$
    * $f(x) - 2x = \frac{3}{x}$
    * $\limit{x}{\infty} [f(x) - 2x] = \limit{x}{\infty} \frac{3}{x}$
    * $\limit{x}{\infty} [f(x) - 2x] = \limit{x}{\infty} \frac{\frac{3}{x}}{\frac{x}{x}}$
    * $\limit{x}{\infty} [f(x) - 2x] = \limit{x}{\infty} \frac{\frac{3}{x}}{1}$

---

## Answers to Exercises, cont.

* Determine the oblique asymptote of $f(x) = \frac{2x^2 + 3}{x}$
    * $\limit{x}{\infty} [f(x) - 2x] = \limit{x}{\infty} \frac{\frac{3}{x}}{1}$
    * $\limit{x}{\infty} [f(x) - 2x] = 0$
    * OA: $y = 2x$

---

## Answers to Exercises, cont.

* Determine the oblique asymptote of $f(x) = \frac{3x^2 - 7x}{x - 2}$
    * $
    \begin{array}{c|rrrr}
        & 3 & -7 & 0 \\
        2 & \downarrow & 6 & -2 \\
        \hline
        & 3 & -1 & -2 \\
    \end{array}$
    * $f(x) = 3x - 1 - \frac{2}{x - 2}$
    * $f(x) - (3x - 1) = -\frac{2}{x - 2}$
    * $\limit{x}{\infty} [f(x) - (3x - 1)] = - \limit{x}{\infty} \frac{2}{x - 2}$

---

## Answers to Exercises, cont.

* Determine the oblique asymptote of $f(x) = \frac{3x^2 - 7x}{x - 2}$
    * $\limit{x}{\infty} [f(x) - (3x - 1)] = - \limit{x}{\infty} \frac{2}{x - 2}$
    * $\limit{x}{\infty} [f(x) - (3x - 1)] = - \limit{x}{\infty} \frac{\frac{2}{x}}{\frac{x}{x} - \frac{2}{x}}$
    * $\limit{x}{\infty} [f(x) - (3x - 1)] = - \limit{x}{\infty} \frac{\frac{2}{x}}{1 - \frac{2}{x}}$
    * $\limit{x}{\infty} [f(x) - (3x - 1)] = 0$
    * OA: $y = 3x - 1$

---

## Answers to Exercises, cont.

* Determine the oblique asymptote of $f(x) = \frac{6x^3 - 5x}{x^2 + 1}$

$
    \begin{array}{rll}
        6x \phantom{}\\
        x^2 + 0x + 1 \enclose{longdiv}{6x^3 + 0x^2 - 5x + 0} \\
        - \underline{6x^3 + 0x^2 + 6 \phantom{00000}}\\
        0x^2 - 11x + 0
    \end{array}
$

* $f(x) = 6x - \frac{11x}{x^2 + 1}$
* $f(x) - 6x = -\frac{11x}{x^2 + 1}$

---

## Answers to Exercises, cont.

* Determine the oblique asymptote of $f(x) = \frac{6x^3 - 5x}{x^2 + 1}$
    * $f(x) - 6x = -\frac{11x}{x^2 + 1}$
    * $\limit{x}{\infty} [f(x) - 6x] = - \limit{x}{\infty} \frac{11x}{x^2 + 1}$
    * $\limit{x}{\infty} [f(x) - 6x] = - \limit{x}{\infty} \frac{\frac{11x}{x^2}}{\frac{x^2}{x^2} + \frac{1}{x^2}}$
    * $\limit{x}{\infty} [f(x) - 6x] = - \limit{x}{\infty} \frac{\frac{11}{x}}{1 + \frac{1}{x^2}}$

---

## Answers to Exercises, cont.

* Determine the oblique asymptote of $f(x) = \frac{6x^3 - 5x}{x^2 + 1}$
    * $\limit{x}{\infty} [f(x) - 6x] = - \limit{x}{\infty} \frac{\frac{11}{x}}{1 + \frac{1}{x^2}}$
    * $\limit{x}{\infty} [f(x) - 6x] = 0$
    * OA: $y = 6x$

---

## Answers to Exercises, cont.

* Determine the oblique asymptote of $f(x) = \frac{-4x^3 + 2x^2 + x - 4}{x^2 - 2x}$

$
    \begin{array}{rll}
        -4x - 6 \phantom{}\\
        x^2 - 2x \enclose{longdiv}{-4x^3 + 2x^2 + x - 4} \\
        - \underline{-4x^3 + 8x^2 \phantom{0000000}} \\
        -6x^2 + x \phantom{0000} \\
        - \underline{-6x^2 - 12x \phantom{00}} \\
        13x - 4
    \end{array}
$

---

## Answers to Exercises, cont.

* Determine the oblique asymptote of $f(x) = \frac{-4x^3 + 2x^2 + x - 4}{x^2 - 2x}$
    * $f(x) = -4x - 6 + \frac{13x - 4}{x^2 - 2x}$
    * $f(x) + (4x + 6) = \frac{13x - 4}{x^2 - 2x}$
    * $\limit{x}{\infty} [f(x) + (4x + 6)] = \limit{x}{\infty} \frac{13x - 4}{x^2 - 2x}$
    * $\limit{x}{\infty} [f(x) + (4x + 6)] = \limit{x}{\infty} \frac{\frac{13x}{x^2} - \frac{4}{x^2}}{\frac{x^2}{x^2} - \frac{2x}{x^2}}$

---

## Answers to Exercises, cont.

* Determine the oblique asymptote of $f(x) = \frac{-4x^3 + 2x^2 + x - 4}{x^2 - 2x}$
    * $\limit{x}{\infty} [f(x) + (4x + 6)] = \limit{x}{\infty} \frac{\frac{13x}{x^2} - \frac{4}{x^2}}{\frac{x^2}{x^2} - \frac{2x}{x^2}}$
    * $\limit{x}{\infty} [f(x) + (4x + 6)] = \limit{x}{\infty} \frac{\frac{13}{x} - \frac{4}{x^2}}{1 - \frac{2}{x}}$
    * $\limit{x}{\infty} [f(x) + (4x + 6)] = 0$
    * OA: $y = -4x - 6$

---

# [Next Unit](../Applications/Lesson%201)