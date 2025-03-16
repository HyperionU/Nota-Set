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

---

# Lesson 2: Limits for Rational Expressions

---

<!--paginate: true-->

## Intro

* Consider this limit: $\limit{x}{3}(\frac{x - 3}{x + 3})$
    * $\frac{(3) - 3}{(3) + 3}$
    * $\frac{0}{6}$
    * $0$
* We get that the numerator approaches $0$, and the denominator approaches $6$, which means that the limit is $0$.

---

## Example 1

1. Evaluate the following Limit: $\limit{x}{-5} \frac{x + 5}{x + 7}$
    * $\frac{-5 + 5}{-5 + 7}$
    * $\frac{0}{2}$
    * $0$

---

## Example 2: 'Undefined' Values

2. Evaluate the following limit: $\limit{x}{3} \frac{x^2 - 9}{x - 3}$
    * $\limit{x}{3} \frac{(x - 3)(x + 3)}{x - 3}$
    * $\limit{x}{3} x + 3 = 6$
* The function is undefined at $x = 3$, but the limit exists. It's a *Removable Discontinuity*.
* Evaluate the following limit: $\limit{x}{-4} \frac{x^2 + 6x + 8}{x^2 + 7x + 12}$ (ex.)

---

## Example 3: Rationalization

3. Evaluate the following limit: $\limit{x}{2} \frac{x - \sqrt{3x - 2}}{x^2 - 4}$
    * Rationalize: $\limit{x}{2} \frac{(x - \sqrt{3x - 2})(x + \sqrt{3x - 2})}{(x^2 - 4)(x + \sqrt{3x - 2})}$
    * $\limit{x}{2} \frac{x^2 - 3x + 2}{(x - 2)(x + 2)(x + \sqrt{3x - 2})}$
    * $\limit{x}{2} \frac{(x - 2)(x - 1)}{(x - 2)(x + 2)(x + \sqrt{3x - 2})}$

---

## Example 3, cont.

* $\limit{x}{2} \frac{(x - 2)(x - 1)}{(x - 2)(x + 2)(x + \sqrt{3x - 2})}$
    * $\limit{x}{2} \frac{(x - 1)}{(x + 2)(x + \sqrt{3x - 2})}$
    * $\frac{(2 - 1)}{(2 + 2)(2 + \sqrt{3(2) - 2})}$
    * $\frac{1}{16}$
* Evaluate the following limit: $\limit{x}{3} \frac{x - \sqrt{x + 6}}{x - 3}$ (ex.)
    
---

## Example 4: Infinite Limits

4. Find $\limit{x}{1} \frac{x^2 + 1}{x - 1}$
    * $\limit{x}{1^+} \frac{x^2 + 1}{x - 1} = \infty$
    * $\limit{x}{1^-} \frac{x^2 + 1}{x - 1} = -\infty$
    * $\limit{x}{1} \frac{x^2 + 1}{x - 1}\ \text{DNE}$
* Evaluate the limit: $\limit{x}{0} \frac{x^2 + x}{x}$ (ex. for reader)

---

## Exercises for Readers

* Evaluate the following limits:
    * $\limit{x}{3} \frac{x^2 - 9}{2x^2 - x - 15}$

    * $\limit{x}{5} \frac{\sqrt{x - 1} - 2}{x - 5}$

    * $\limit{x}{2} \frac{x^2 + 2x - 8}{x^3 - 8}$

    * $\limit{x}{-3} \frac{\frac{1}{3} + \frac{1}{x}}{3 + x}$

---

# [Next Lesson](Lesson%203)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Evaluate the following limit: $\limit{x}{-4} \frac{x^2 + 6x + 8}{x^2 + 7x + 12}$
    * $\limit{x}{-4} \frac{(x + 4)(x + 2)}{(x + 3)(x + 4)}$
    * $\limit{x}{-4} \frac{(x + 2)}{(x + 3)}$
    * $\frac{(-4 + 2)}{(-4 + 3)}$
    * $\frac{-2}{-1} = 2$

---

## Answers to Exercises, cont.

* Evaluate the following limit: $\limit{x}{3} \frac{x - \sqrt{x + 6}}{x - 3}$
    * $\limit{x}{3} \frac{(x - \sqrt{x + 6})(x + \sqrt{x + 6})}{(x - 3)(x + \sqrt{x + 6})}$
    * $\limit{x}{3} \frac{x^2 - x + 6}{(x - 3)(x + \sqrt{x + 6})}$
    * $\limit{x}{3} \frac{(x - 3)(x + 2)}{(x - 3)(x + \sqrt{x + 6})}$
---

## Answers to Exercises, cont.

* Evaluate the following limit: $\limit{x}{3} \frac{x - \sqrt{x + 6}}{x - 3}$
    * $\limit{x}{3} \frac{x + 2}{x + \sqrt{x + 6}}$
    * $\frac{3 + 2}{3 + \sqrt{3 + 6}}$
    * $\frac{5}{6}$

---

## Answers to Exercises, cont.

* Evaluate the limit: $\limit{x}{0} \frac{x^2 + x}{x}$
    * $\limit{x}{0} \frac{x(x + 1)}{x}$
    * $\limit{x}{0} x + 1$
    * $1$

---

## Answers to Exercises, cont.

* Evaluate $\limit{x}{3} \frac{x^2 - 9}{2x^2 - x - 15}$
    * $\limit{x}{3} \frac{(x - 3)(x + 3)}{(x - 3)(2x + 5)}$
    * $\limit{x}{3} \frac{x + 3}{2x + 5}$
    * $\frac{3 + 3}{2(3) + 5}$
    * $\frac{6}{6 + 5}$
    * $\frac{6}{11}$

---

## Answers to Exercises, cont.

* Evaluate $\limit{x}{5} \frac{\sqrt{x - 1} - 2}{x - 5}$
    * $\limit{x}{5} \frac{(\sqrt{x - 1} - 2)(\sqrt{x - 1} + 2)}{(x - 5)(\sqrt{x - 1} + 2)}$
    * $\limit{x}{5} \frac{x - 1 - 4}{(x - 5)(\sqrt{x - 1} + 2)}$
    * $\limit{x}{5} \frac{x - 5}{(x - 5)(\sqrt{x - 1} + 2)}$
    * $\limit{x}{5} \frac{1}{\sqrt{x - 1} + 2}$

---

## Answers to Exercises, cont.

* Evaluate $\limit{x}{5} \frac{\sqrt{x - 1} - 2}{x - 5}$
    * $\frac{1}{\sqrt{5 - 1} + 2}$
    * $\frac{1}{2 + 2}$
     $\frac{1}{4}$

---

## Answers to Exercises, cont.

* Evaluate $\limit{x}{2} \frac{x^2 + 2x - 8}{x^3 - 8}$
    * $\limit{x}{2} \frac{(x - 2)(x + 4)}{(x - 2)(x^2 + 2x + 4)}$
    * $\limit{x}{2} \frac{x + 4}{x^2 + 2x + 4}$
    * $\frac{2 + 4}{(2)^2 + 2(2) + 4}$
    * $\frac{6}{12}$
    * $\frac{1}{2}$

---

## Answers to Exercises, cont.

* Evaluate $\limit{x}{-3} \frac{\frac{1}{3} + \frac{1}{x}}{3 + x}$
    * $\limit{x}{-3} \frac{\frac{x}{3x} + \frac{3}{3x}}{3 + x}$
    * $\limit{x}{-3} \frac{x + 3}{3x} / (3 + x)$
    * $\limit{x}{-3} \frac{x + 3}{3x(x + 3)}$
    * $\limit{x}{-3} \frac{1}{3x}$

---

## Answers to Exercises, cont.

* Evaluate $\limit{x}{-3} \frac{\frac{1}{3} + \frac{1}{x}}{3 + x}$
    * $\frac{1}{3(-3)}$
    * $-\frac{1}{9}$

---

# [Next Lesson](Lesson%203)