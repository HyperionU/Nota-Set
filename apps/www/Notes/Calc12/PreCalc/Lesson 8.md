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

# Lesson 8: Absolute Value Inequalities

---

<!--paginate: true-->

## Intro

* The absolute value is defined as follows:
    * $|x| = \begin{cases}
        x & \text{if } x \ge 0 \\
        -x & \text{if } x < 0
    \end{cases}$
* For equations and inequalities, we can use this definition to solve them.

---

## Example 1

1. Solve $|x| = 5$
    * (1) $x \ge 0$: $|x| = 5 \rightarrow x = 5$
    * (2) $x < 0$: $|x| = 5 \rightarrow -(x) = 5, x = -5$
    * $x = \pm 5$

* Solve $|3x + 4| = 13$ (ex. for reader)

---

## Example 2

2. Solve $|2x + 5| < 7$
    * (1) $2x + 5 \ge 0$:
        * $x \ge -\frac{5}{2}, |2x + 5| < 7 \rightarrow 2x + 5 < 7, x < 1$ 
        * $-\frac{5}{2} \le x < 1$
    * (2) $2x + 5 < 0$:
        * $x < -\frac{5}{2}, |2x + 5| < 7 \rightarrow -(2x + 5) < 7, x > -6$ 
        * $-6 < x < -\frac{5}{2}$
    * Combine cases: $-6 < x < 1$

---

## Example 2, cont.

2. Solve $|2x + 5| < 7$
    * Combine cases: $-6 < x < 1$
    * Check each region:
        * $x < -6$: Ex.
        * $-6 < x < 1$: In.
        * $x > 1$: Ex.
    * $(-6, 1)$

* Solve $|3x + 1| \ge 8$ (ex. for reader)

---

## Rationals with Absolute Value

3. Solve $\frac{|x|}{|x - 1|} > 1$
    * Undefined Values: $x \ne 1$
    * Solve $\frac{|x|}{|x - 1|} = 1$ for Critical Values.

---

## Rationals, cont.

3. Solve $\frac{|x|}{|x - 1|} > 1$
    * (1) $x \ge 0, x - 1 > 0$ ($x > 1$):
        * $\frac{|x|}{|x - 1|} = 1 \rightarrow \frac{x}{x - 1} = 1, 0 = -1$
        * No Solution for (1)
    * (2) $x \ge 0, x - 1 < 0$ ($x < 1$):
        * $\frac{|x|}{|x - 1|} = 1 \rightarrow \frac{x}{-(x - 1)} = 1, 2x = 1$
        * $x = \frac{1}{2}$

---

## Rationals, cont.

3. Solve $\frac{|x|}{|x - 1|} > 1$
    * (3) $x < 0, x - 1 > 0$ ($x > 1$):
        * $0 > x > 1$ (*what the...*)
        * No Solution for (3)
    * (4) $x < 0, x - 1 < 0$ ($x < 1$):
        * $\frac{|x|}{|x - 1|} = 1 \rightarrow \frac{-x}{-(x - 1)} = 1$
        * Same as (1)
        * No Solution for (4)

---

## Rationals, cont.

3. Solve $\frac{|x|}{|x - 1|} > 1$
    * Critical Values: $x = \frac{1}{2}, x \ne 1$
    * Check each region:
        * $x < \frac{1}{2}$: Ex.
        * $\frac{1}{2} < x < 1$: In.
        * $x > 1$: In.
    * $[\frac{1}{2}, 1) \cup (1, \infty)$

* Solve $|\frac{x - 5}{x}| \ge 0$ (ex. for reader)

---

## Exercise

* Solve $|x + 1| < 5$ (ex. for reader)
* Solve $|x + 2| > 6$ (ex. for reader)
* Solve $|x - 4| - 3 \le 0$ (ex. for reader)
* Solve $|5x - 2| < 6$ (ex. for reader)

---

# [Next Lesson](Lesson%209)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercise

* Solve $|3x + 4| = 13$
    * (1) $3x + 4 \ge 0$: 
        * $x \ge -\frac{4}{3}, |3x + 4| = 13 \rightarrow 3x + 4 = 13, x = 3$ (Inc.)
    * (2) $3x + 4 < 0$: 
        * $x < -\frac{4}{3}, |3x + 4| = 13 \rightarrow -(3x + 4) = 13, x = -\frac{17}{3}$ (Inc.)
    * $x = 3, -\frac{17}{3}$

---

## Answers to Exercise

* Solve $|3x + 1| \ge 8$
    * (1) $3x + 1 \ge 0$ ($x \ge -\frac{1}{3}$):
        * $|3x + 1| \ge 8 \rightarrow 3x + 1 \ge 8, x \ge \frac{7}{3}$
    * (2) $3x + 1 < 0$ ($x < -\frac{1}{3}$):
        * $|3x + 1| \ge 8 \rightarrow -(3x + 1) \ge 8, x \le -3$
    * $(-\infty, -3] \cup [\frac{7}{3}, \infty)$

---

## Answers to Exercise

* Solve $|\frac{x - 5}{x}| \ge 0$ 
    * (1) $\frac{x - 5}{x} \ge 0$:
        * $|\frac{x - 5}{x}| = 0 \rightarrow \frac{x - 5}{x} = 0, x = 5$ (CV)
    * (2) $\frac{x - 5}{x} < 0$ :
        * $|\frac{x - 5}{x}| = 0 \rightarrow -(\frac{x - 5}{x}) = 0, x = 5$ (CV)
    * $(-\infty, 0] \cup [0, \infty)$
    * $(-\infty, \infty)$

---

## Answers to Exercise

* Solve $|x + 1| < 5$
    * (1) $x + 1 \ge 0$ ($x \ge -1$):
        * $|x + 1| < 5 \rightarrow x + 1 < 5, x < 4$ ($-1 \le x < 4$)
    * (2) $x + 1 < 0$ ($x < -1$):
        * $|x + 1| < 5 \rightarrow -(x + 1) < 5, x > -6$ ($-6 < x < -1$)
    * Combine: $-6 < x < 4$
    * $(-6, 4)$

---

## Answers to Exercise

* Solve $|x + 2| > 6$
    * (1) $x + 2 \ge 0$ ($x \ge -2$):
        * $|x + 2| > 6 \rightarrow x + 2 > 6, x > 4$ ($x > 4$)
    * (2) $x + 2 < 0$ ($x < -2$):
        * $|x + 2| > 6 \rightarrow -(x + 2) > 6, x < -8$ ($x < -8$)
    * Combine: $x > 4, x < -8$
    * $(-\infty, -8) \cup (4, \infty)$

---

## Answers to Exercise
* Solve $|x - 4| - 3 \le 0$
    * $|x - 4| \le 3$
    * (1) $x - 4 \ge 0$ ($x \ge 4$):
        * $|x - 4| \le 3 \rightarrow x - 4 \le 3, x \le 7$ ($4 \le x \le 7$)
    * (2) $x - 4 < 0$ ($x < 4$):
        * $|x - 4| \le 3 \rightarrow -(x - 4) \le 3, x - 4 \ge -3, x \ge 1$
        ($1 \le x < 4$)
    * Combine: $1 \le x \le 7$
    * $[1, 7]$
---

## Answers to Exercise

* Solve $|5x - 2| < 6$
    * (1) $5x - 2 \ge 0$ ($x \ge \frac{2}{5}$)
        * $|5x - 2| < 6 \rightarrow 5x - 2 < 6, x < \frac{8}{5}$ ($\frac{2}{5} \le x < \frac{8}{5}$ or $[\frac{2}{5}, \frac{8}{5})$)
    * (2) $5x - 2 < 0$ ($x < \frac{2}{5}$)
        * $|5x - 2| < 6 \rightarrow -(5x - 2) < 6, x > -\frac{4}{5}$ ($-\frac{4}{5} \le x < \frac{2}{5}$ or $(-\frac{4}{5}, \frac{2}{5})$)
    * Combine: $(-\frac{4}{5}, \frac{8}{5})$

---

# [Next Lesson](Lesson%209)