---
marp: true
theme: uncover
class: invert
math: mathjax
---

$\newcommand\diff[1]{\mathcal{d}_{#1}}$
$\newcommand\eval[3]{\left. #1 \right|_{#2}^{#3}}$

# <!--fit--> Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2025-->

$\newcommand\dd[2][]{\displaystyle\frac{d#1}{d#2}}$
$\newcommand\limit[2]{\displaystyle\lim_{#1 \to #2}}$

---

# Lesson 5: Area Using Numerical Methods

---

<!--paginate: true-->

## Intro

* If we are given a function that is continuous over an interval $[a,b]$, and if we can find an antiderivative, we can find $F(b) - F(a)$.
* Thus, we can find the accumulated signed area under the curve over the stated interval.
* Functions, however, may not always have an easy to find antiderivative.
* These functions require a new method to calculate the area.

---

## Area Using Numerical Methods

* Throughout this lesson, we will look at a number of numerical methods which can be used to find the area.
* Next unit, we'll learn several strategies to find the definite integral.
* However, even given those new tools, there will still be useful applications for numerical methods.

---

## Rectangular Rule

* One of our numerical methods we'll examine proposes dividing the area under the given function $f(x)$ up into a number of rectangles.
* These are of equal length along the $x$-axis, and if there are $n$ such rectangles created in the interval $[a, b]$, then each one is of length $\frac{b - a}{n}$.

---

## Rectangular Rule, cont.

* The height of each rectangle is equal to $f(x)$.
* There is a problem though, since the function has most likely changed in height over the length of the rectangle. We call this point $f(x_i), x_i = a + i(\frac{b - a}{n})$
* We should take note that this is only an approximation, the height we're using is not exact.
* Therefore, our approximation using the rectangular rule will be larger that the actual value.

---

## Area using Rectangular Rule

* Each of the areas of the rectangles is added and the result is our approximation.
* We note this with summation notation: $\displaystyle \frac{b - a}{n} \sum_{i = 1}^n f(x_i)$
* Our concern about the discrepancy in height would be diminished if we used more rectangles and made each rectangle smaller in width.

---

## Area using Rectangular Rule

* This would make the difference between $f(x_i)$ and $f(x_{i + 1})$ smaller, giving a better approximation.
* The actual value of the accumulated signed area is the limiting value of the sum of the areas as the number of rectangles approaches infinity: $\displaystyle \lim_{n \to \infty} \sum_{i = 1}^n f(x_i) \Delta x_i$.
* This works as a partial proof leading to the fundamental theorem of calculus. The full proof is out of scope of this course.

---

## Area using Rectangular Rule

* We can say that an approximation of the definite integral is given by $\displaystyle \int_a^b f(x) dx \approx \frac{b - a}{n} \sum_{i = 1}^n f(x_i)$.
* Also, as $n \to \infty, \displaystyle \int_a^b f(x) dx = \frac{b - a}{n} \sum_{i = 1}^n f(x_i)$.

---

## Example 1

1. Determine the signed area under the function $f(x) = x$ in the interval $[0, 4]$.
    * We chose this because we can find the area graphically, as well as its antiderivative.
    * Graphically, the area is exactly half of a square. So, the area would be $8 \mathrm{u}^2$.
    * $A = \int_0^4 (x)dx = \eval{\frac{1}{2}x^2}{0}{4} = \frac{1}{2}4^2 - \frac{1}{2}0^2$
    * $A = 8$

---

## Example 1, cont.

1. Determine the signed area under the function $f(x) = x$ in the interval $[0, 4]$.
    * Now, let's try using rectangular rule.
    * First, using 4 rectangles:
    * $\frac{4 - 0}{4} = \frac{4}{4} = 1$.
    * $x_i = 0 + i$
    * $\displaystyle A \approx l\sum_{i = 1}^4 x_i = 1(1 + 2 + 3 + 4)$
    * $A \approx 10$

---

## Example 1, cont.

1. Determine the signed area under the function $f(x) = x$ in the interval $[0, 4]$.
    * Now, using 40 rectangles:
    * $\frac{4 - 0}{40} = \frac{4}{40} = \frac{1}{10}$.
    * $x_i = \frac{i}{10}$
    * $\displaystyle A \approx l\sum_{i = 1}^{40} x_i \approx \frac{1}{10}\sum_{i = 1}^{40} \frac{1}{10}i \approx \frac{1}{100}\sum_{i = 1}^{40} i$
    * $\displaystyle A \approx \frac{1}{100}\sum_{i = 1}^{40} i \approx \frac{1}{100}\left(\frac{n(n + 1)}{2}\right)$

---

## Example 1, cont.

1. Determine the signed area under the function $f(x) = x$ in the interval $[0, 4]$.
    * $A \approx \frac{1}{100}\left(\frac{40(40 + 1)}{2}\right) \approx \frac{1}{100}\left(\frac{40(41)}{2}\right)$
    * $A \approx \frac{1640}{200}$
    * $A \approx \frac{1640}{200} \approx \frac{16.4}{2}$
    * $A \approx 8.2$
* Since our function is increasing on the interval, our approximation will be larger.

---

## Riemann Sums

* German mathematician Bernhard Riemann (1826 - 1866) is credited with developing a theorem for finding areas under a curve using rectangular areas.
* This theorem, in its simplest form is the idea proposed by the rectangular rule.
$$S_n = \frac{b - a}{n} \sum_{i = 1}^n f(x_i)$$
* This is a form of the rectangular rule and general Riemann sum.

---

## Upper / Lower Sums

* Riemann also noticed that the value of $f(x)$ was different at the beginning and the end of the rectangle being used.
* Recall that we noted this earlier.
* To remedy this, Riemann chose to create two additional sums dealing with the same sum as his general sum.

---

## Upper Riemann Sum

* For this, we use the same sum and interval as before, except we'll use the maximum value for the height.
$$S_n = \frac{b - a}{n} \sum_{i = 1}^n M_i$$
* $M$ is the maximum value of the function over the interval $i$.

---

## Lower Riemann Sum

* We can use the same sum and interval, except with the minimum value for the height.
$$s_n = \frac{b - a}{n} \sum_{i = 1}^n m_i$$
* $m$ is the maximum value of the function over the interval $i$.

---

## On the Question of Height

* The height of the rectangle is the tallest rectangle that 
    * is completely underneath the function at all points on the interval, and 
    * touches the function.
* In a given section, the function rises to a minimum value of $m_i$ at $f(x_i)$, to a maximum value of $M_i$ at $f(x_{i + 1})$.
* The difference in area is the difference between the sums.

---

## Range of Approximation

* Since the upper sum deals with an approximation that is larger than the actual area, and the lower sum deals with an approximation that is smaller than the actual area, we can say that: $s_n \le \text{general sum} \le S_n$.
* Note that the subscript $n$ can be used to find how many rectangles need to be used.

---

## Example 2

2. Find the area under $f(x) = x^2$ in the interval from the origin to 1 using Reimann sums.
    * $\frac{b - a}{n} = \frac{1 - 0}{4} = \frac{1}{4}$
    * For the upper sums: $M = \frac{1}{16}, \frac{1}{4}, \frac{9}{16}, 1$
    * These values correspond to: $\frac{1}{4}, \frac{1}{2}, \frac{3}{4}, 1$
    * $S_4 = \frac{1}{4}(\frac{1}{16} + \frac{1}{4} + \frac{9}{16} + 1)$
    * $S_4 = \frac{1}{4}(\frac{1 + 4 + 9 + 16}{16})$
    * $S_4 = \frac{1}{4}(\frac{30}{16})$
    * $S_4 = \frac{15}{32}$

---

## Example 2, cont.

2. Find the area under $f(x) = x^2$ in the interval from the origin to 1 using Reimann sums.
    * For the lower sums: $m = 0, \frac{1}{16}, \frac{1}{4}, \frac{9}{16}$
    * $s_4 = \frac{1}{4}(0 + \frac{1}{16} + \frac{1}{4}+ \frac{9}{16})$
    * $s_4 = \frac{1}{4}(\frac{1 + 4 + 9}{16})$
    * $s_4 = \frac{1}{4}(\frac{14}{16})$
    * $s_4 = \frac{7}{32}$
    * $\therefore \frac{7}{32} \le A \le \frac{15}{32}$.
* This gives us a viable method to use.

---

## Trapezoidal Rule

* Our next method involves the division of the functional area into trapezoids rather than rectangles.
* The trapezoids have a flat base, two sides of different lengths, and a top side that is slanted.
* The slanted top side is a closer approximation of the curve than the rectangle.

---

## Trapezoidal Rule, cont.

* Each trapezoid is of width $\frac{b - a}{n}$ given an interval $[a, b]$ and $n$ trapezoids, with area $\frac{b - a}{n} \left(\frac{f(x_i) + f(x_{i + 1})}{2}\right)$.
* That is, the length along the $x$-axis multiplied by the mean height.
* The area is 
$$A = \frac{b - a}{n} \sum_{i = 1}^n \frac{f(x_i) + f(x_{i + 1})}{2}$$ 
where $x_i = a + \frac{b - a}{n}(i)$.

---

## Example 3

3. Use the trapezoid rule to evaluate the area under the curve $f(x) = \frac{1}{x}$ over the interval $[1,5]$ using 8 trapezoids.
    * $A = \frac{b - a}{2n}[f(a) + 2f(x_1) + \dots + 2f(x_{n - 1}) + f(b)]$
    * $A = \frac{5 - 1}{2(8)}[f(1) + 2f(\frac{3}{2}) + 2f(2) + 2f(\frac{5}{2}) + 2f(3) + 2f(\frac{7}{2})$ $+ 2f(4) + 2f(\frac{9}{2}) + f(5)]$
    * $A = \frac{1}{4}[1 + 2(\frac{2}{3}) + 2(\frac{1}{2}) + 2(\frac{2}{5}) + 2(\frac{1}{3}) + 2(\frac{7}{2}) + 2(\frac{1}{4})$ $+ 2(\frac{2}{9}) + \frac{1}{5}]$
    * $A = \frac{1}{4}[2 + \frac{4}{3} + \frac{4}{5} + \frac{2}{3} + \frac{4}{7} + \frac{1}{2} + \frac{4}{9} + \frac{1}{5}]$

---

## Example 3

3. Use the trapezoid rule to evaluate the area under the curve $f(x) = \frac{1}{x}$ over the interval $[1,5]$ using 8 trapezoids.
    * $A = \frac{1}{4}[2 + \frac{4}{3} + \frac{4}{5} + \frac{2}{3} + \frac{4}{7} + \frac{1}{2} + \frac{4}{9} + \frac{1}{5}]$
    * $A = \frac{1}{4}[5 + \frac{4}{7} + \frac{1}{2} + \frac{4}{9}]$
    * $A = \frac{1}{4}[\frac{5(2)(9)(7)}{2(9)(7)} + \frac{4(9)(2)}{7(9)(2)} + \frac{1(9)(7)}{2(9)(7)} + \frac{4(2)(7)}{9(2)(7)}]$
    * $A = \frac{1}{4}[\frac{821}{126}]$
    * $A = \frac{821}{504} \approx 1.63$
* Note the actual value is $\ln 5 \approx 1.61$.

---

## Exercise for Readers

* Use rectangular rule to approximate the area under $f(x) = \cos x$ for the interval $[0, \frac{\pi}{2}]$. Use six rectangles.
* For $f(x) = \cos x$, solve for the area using the antiderivative and compare answers.
* Find the area under $y = 2x^2 + 1$ from 0 to 2 with trapezoid rule using 4 trapezoids.
* Find the area under $y = 2x^2 + 1$ using a definite integral and compare answers.

---

# [Next Unit](../Applications/Lesson%201)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercise

* Use rectangular rule to approximate the area under $f(x) = \cos x$ for the interval $[0, \frac{\pi}{2}]$. Use six rectangles.
    * $\ell = \frac{\frac{\pi}{2} - 0}{6} = \frac{\pi}{12}$
    * $\displaystyle A \approx l\sum_{i = 1}^{6} \cos x_i$ 
    * $A \approx \frac{\pi}{12}[1 + \frac{\sqrt{6} + \sqrt{2}}{4} + \frac{\sqrt{3}}{2} + \frac{\sqrt{2}}{2} + \frac{1}{2} + \frac{\sqrt{6} - \sqrt{2}}{4}]$
    * $A \approx \frac{\pi(\sqrt{6} + \sqrt{3} + \sqrt{2} + 3)}{24}$
    * $A \approx \frac{9}{8}$

---

## Answers to Exercise, cont.

* For $f(x) = \cos x$, solve for the area using the antiderivative and compare answers.
    * $A = \int_0^\frac{\pi}{2} \cos x dx$
    * $A = \eval{\sin x}{0}{\frac{\pi}{2}} = \sin \frac{\pi}{2} - \sin 0$
    * $A = 1$
    * $A_r > A$

---

## Answers to Exercise, cont.

* Find the area under $y = 2x^2 + 1$ from 0 to 2 with trapezoid rule using 4 trapezoids.
    * $A \approx \frac{b - a}{2n}[f(a) + 2f(x_1) + 2f(x_2) + f(b)]$
    * $x_i = \frac{1}{2}i$
    * $A \approx \frac{2 - 0}{2(4)}[f(0) + 2f(\frac{1}{2}) + 2f(1) + 2f(\frac{3}{2}) + f(2)]$
    * $A \approx \frac{1}{4}[(2(0)^2 + 1) + 2(2(\frac{1}{2})^2 + 1) + 2(2(1)^2 + 1)$ $+ 2(2(\frac{3}{2})^2 + 1) + (2(2)^2 + 1)]$
    * $A \approx \frac{15}{2}$

---

## Answers to Exercise, cont.

* Find the area under $y = 2x^2 + 1$ using a definite integral and compare answers.
    * $A = \int_0^2 (2x^2 + 1) dx$
    * $A = \eval{\frac{2}{3}x^3 + x}{0}{2} = (\frac{2}{3}2^3 + 2) - (\frac{2}{3}0^3 + 0)$
    * $A = \frac{22}{3}$
    * $A_t > A$

---

# [Next Unit](../Applications/Lesson%201)