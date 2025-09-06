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

# Lesson 3: The Fundamental Theorem of Calculus

---

<!--paginate: true-->

## Intro

* Previously, we found a method for determining the signed area of a continuous function $y = f(x)$ and the $x$-axis in the interval $[a, b]$.
* We've also proved that the signed area function $A(x) = \int f(x)$, and that the signed area $A = A(b) - A(a)$.
* Now, let's introduce some notation for that signed area.

---

## The Riemann Sum

* A lot of the work that we have done came as a result of a method by Georg Riemann (1826 - 1866), which is done by considering the limiting value of the sums of areas of geometric figures.
* Eventually, as the number of figures approach infinity, the width will approach zero, no matter what the initial value was.

---

## Right-hand Approximation Method 

* The width of each rectangle is the interval width divided by the number of rectangles. ($W = \frac{b - a}{n}$)
* The length of each rectangle is the value of the function at the right edge of each rectangle. ($l = f(i)$)
* The total area is $\displaystyle \sum_{i = a + \frac{b - a}{n}}^{n} \frac{b - a}{n}[f(i)]$

---

## Right RAM Example

* Let's start by considering what happens with 4 rectangles ($n = 4$) over the interval $[0, 4]$ for the function $f(x) = x^2$.
* We get that the total area is $\displaystyle \sum_{i = 1}^{n} \frac{4 - 0}{4}[f(i)]$
* Which means $\displaystyle \sum_{i = 1}^{n} [f(i)] = f(1) + f(2) + f(3) + f(4) = 33$
* Can we make this better?

---

## Generalized Right RAM

* For the function $f(x) = x^2$, over the interval $[0, 4]$, consider $n$ rectangles.
* We get that the total area is $\displaystyle \sum_{i = 1}^{n} \frac{4}{n}(\frac{4}{n}i)^2$
* Extracting a common factor: $\displaystyle (\frac{4}{n})^3 \sum_{i = 1}^{n} [i^2]$
* Note that $\displaystyle \sum_{i=1}^n i^2 = \frac{2n^3 + 3n^2 + n}{6}$

---

## Generalized Right RAM, cont.

* We have $\displaystyle (\frac{4}{n})^3 \sum_{i = 1}^{n} [i^2]$
* Note that $\displaystyle \sum_{i=1}^n i^2 = \frac{2n^3 + 3n^2 + n}{6}$

---

## Generalized Right RAM, cont.

* We get that $\frac{4^3}{n^3} \frac{2n^3 + 3n^2 + n}{6} = \frac{32(2n^3 + 3n^2 + n)}{3n^3} = \frac{64n^3 + 96n^2 + 32n}{3n^3}$
* The desired area would be the limiting value as the number of rectangles tend to infinity.
* $A = \limit{n}{\infty} \frac{64n^3 + 96n^2 + 32n}{3n^3}$
* $A = \limit{n}{\infty} [\frac{64n^3}{3n^3} + \frac{96n^2}{3n^3} + \frac{32n}{3n^3}]$
* $A = \limit{n}{\infty} [\frac{64n^3}{3n^3}] + \limit{n}{\infty} [\frac{96n^2}{3n^3}] + \limit{n}{\infty} [\frac{32n}{3n^3}]$

---

## Generalized Right RAM, cont.

* $A = \limit{n}{\infty} [\frac{64n^3}{3n^3}] + \limit{n}{\infty} [\frac{96n^2}{3n^3}] + \limit{n}{\infty} [\frac{32n}{3n^3}]$
* $A = \limit{n}{\infty} [\frac{64}{3}] + \limit{n}{\infty} [\frac{96}{3n}] + \limit{n}{\infty} [\frac{32}{3n^2}]$
* $A = \frac{64}{3}$
* Therefore, the signed area for $f(x) = x^2$ over the interval $[0, 4]$ is $\frac{64}{3}$.
* This works for all other approximation methods. (LRAM, MRAM and TrAM)

---

## The Definite Integral

* The signed area between a function $y = f(x)$ and the $x$-axis in the interval $[a, b]$ is equal to the limiting value of the sums of $n$ geometric figures, as $n \to \infty$.
* Using $n$ rectangles of equal width, the width of each rectangle is $\frac{b - a}{n}$.
* Let $\Delta x$ be this width, and let $x_i$ be the $x$ value within the $i^\text{th}$ rectangle where the top of the rectangle is equal to $f(x_i)$.

---

## The Definite Integral, cont.

* The area of the rectangle is $(f(x_i))(\Delta x)$.
* Let's take the sum of these areas: $\displaystyle \sum_{i = 1}^n [(f(x_i))(\Delta x)]$
* And take the limit: $\limit{n}{\infty} \sum_{i = 1}^n [(f(x_i))(\Delta x)]$
* We get $\limit{n}{\infty} \frac{b - a}{n} \sum_{i = 1}^n [(f(x_i))] = \int_a^b f(x) dx$.
* This symbol ($\int_a^b f(x) dx$) is the definite integral of $f$ from $a$ to $b$.

---

## The Fundamental Theorem

* The value of $\int_a^b f(x) dx$ is the accumulated signed area between $f(x)$ and the $x$-axis, over the interval $[a, b]$.
* *Hang on. This looks familiar.* It does.
* We know that for a given function $y = f(x)$, $A(x) = \int f(x)$. 
* Based on this, we can note that $\int_a^b f(x) dx = A(b) - A(a)$.
* This is **The Fundamental Theorem of Calculus**.
* Let's try this out shall we?

---

## Example 1

1. Evaluate $\int_{-1}^5 (x + 1) dx$
    * $\int (x + 1) dx = \frac{1}{2}x^2 + x + C$
    * $A = \eval{\frac{1}{2}x^2 + x + C}{-1}{5} = A(5) - A(-1)$
    * $A = [\frac{1}{2}(5)^2 + (5) + C] - [\frac{1}{2}(-1)^2 + (-1) + C]$
    * $A = \frac{25 + 2(5) - 1 + 2(1)}{2}$
    * $A = 18$

---

## Example 2

2. Evaluate $\int_{-3}^5 (x + 1) dx$
    * $\int (x + 1) dx = \frac{1}{2}x^2 + x + C$
    * $A = \eval{\frac{1}{2}x^2 + x + C}{-3}{5} = A(5) - A(-3)$
    * $A = [\frac{1}{2}(5)^2 + (5) + C] - [\frac{1}{2}(-3)^2 + (-3) + C]$
    * $A = \frac{25}{2} + 8 - \frac{9}{2}$
    * $A = \frac{25 + 16 - 9}{2}$
    * $A = 16$

---

## Example 3

3. Evaluate $\int_{-3}^{-1} (x + 1) dx$
    * $\int (x + 1) dx = \frac{1}{2}x^2 + x + C$
    * $A = \eval{\frac{1}{2}x^2 + x + C}{-3}{-1} = A(-1) - A(-3)$
    * $A = [\frac{1}{2}(-1)^2 + (-1) + C] - [\frac{1}{2}(-3)^2 + (-3) + C]$
    * $A = \frac{1}{2} - 1 - \frac{9}{2} + 3$
    * $A = -2$

---

## Union Property 

* There's actually a different way to calculate Example 2.
* We know that 
    * $\int_{-1}^5 (x + 1) dx = 18$, 
    * $\int_{-3}^{-1} (x + 1) dx = -2$, and
    * $\int_{-3}^5 (x + 1) dx = 16$
* We can combine them to get that $\int_{-1}^5 (x + 1) dx + \int_{-3}^{-1} (x + 1) dx = 16$.
* If we generalize this, we get that $\int_a^b f(x) dx + \int_b^c f(x) dx = \int_a^c f(x) dx$. 

---

## Example 4

4. What is the difference between $\int_{-1}^5 (x + 1) dx$ and $\int_5^{-1} (x + 1) dx$?
    * $\int (x + 1) dx = \frac{1}{2}x^2 + x + C$
    * $\int_{-1}^5 (x + 1) dx$
        * $A = \eval{\frac{1}{2}x^2 + x + C}{-1}{5} = A(5) - A(-1)$
    * $\int_5^{-1} (x + 1) dx$
        * $A = \eval{\frac{1}{2}x^2 + x + C}{-1}{5} = A(-1) - A(5) =$ 
        $-\int_{-1}^5 (x + 1) dx$

---

## Example 5

5. What is the difference between $\int_{-3}^{-1} (x + 1) dx$ and $\int_{-1}^{-3} (x + 1) dx$?
    * $\int (x + 1) dx = \frac{1}{2}x^2 + x + C$
    * $\int_{-1}^{-3} (x + 1) dx$
        * $A = \eval{\frac{1}{2}x^2 + x + C}{-1}{5} = A(-3) - A(-1)$
    * $\int_{-3}^{-1} (x + 1) dx$
        * $A = \eval{\frac{1}{2}x^2 + x + C}{-1}{5} = A(-1) - A(-3) =$ 
        $-\int_{-1}^{-3} (x + 1) dx$

---

## Inverse Property

* We notice that if we switch the endpoints, we get the negative of the non-switched endpoints.
* In Example 5, areas below the $x$-axis can have a positive signed area, if we accumulate area from right to left, rather than left to right.
* In general: $\int_a^b f(x) dx = -\int_b^a f(x) dx$

---

## Applications of Definite Integrals

* A definite integral represents the change in any of its antiderivative functions over a specific interval.
* As such, the definite integral with an integrand representing acceleration would give the change in the object's velocity over the time interval. 
($\int_{t_0}^{t_1} a(t) dt = v(t_1) - v(t_0)$)
* As such, the definite integral with an integrand representing velocity would give the change in displacement. ($\int_{t_0}^{t_1} v(t) dt = s(t_1) - s(t_0)$)

---

## Example 6

6. An object projected upward from the Earth's surface with an initial velocity of $98 \text{m/s}$.
    * What is the change in velocity in the first $3 \text{s}$ of motion?
        * $a(t) = -9.81 \text{m/s}^2$
        * $v(t) = \int_0^3 a(t) dt = \int_0^3 (-9.81) dt$
        * $\int_0^3 (-9.81) dt = \eval{(-9.81t + C)}{0}{3}$
        * $-9.81(3) + 9.81(0)$
        * $-29.43 \text{m/s}$

---

## Example 6, cont.

6. An object projected upward from the Earth's surface with an initial velocity of $98 \text{m/s}$.
    * What is the velocity-time function for the object?
        * $v(0) = 98 \text{m/s}$
        * $v(t) = \int (-9.81) dt = -9.81t + v(0)$
        * $v(t) = -9.81t + 98$


---

## Example 6, cont.

6. An object projected upward from the Earth's surface with an initial velocity of $98 \text{m/s}$.
    * What is the change in displacement in the first $12 \text{s}$ of motion and its distance travelled?
        * $v(t) = -9.81t + 98$
        * $s(t) = \int (v(t)) dt = \int (-9.81t + 98) dt$
        * $s(t) = \int (-9.81t + 98) dt = -4.91t^2 + 98t + C$
        * $s = \int_0^{12} (-9.81t + 98) dt = \eval{(-4.91t^2 + 98t + C)}{0}{12}$
        * $s = [-4.91(12)^2 + 98(12)] + [4.91(0)^2 - 98(0)]$

---

## Example 6, cont.

6. An object projected upward from the Earth's surface with an initial velocity of $98 \text{m/s}$.
    * What is the change in displacement in the first $12 \text{s}$ of motion and its distance travelled?
        * $v(t) = -9.81t + 98$
        * $s(t) = \int (-9.81t + 98) dt = -4.91t^2 + 98t + C$
        * $s = [-4.91(12)^2 + 98(12)] + [4.91(0)^2 - 98(0)]$
        * $s = 469 \text{m}$

---

## Example 6, cont.

6. An object projected upward from the Earth's surface with an initial velocity of $98 \text{m/s}$.
    * What is the change in displacement in the first $12 \text{s}$ of motion and its distance travelled?
        * $v(t) = -9.81t + 98$
        * $s(t) = -4.91t^2 + 98t$
        * $0 = -9.81t + 98$
        * $t = 10 \text{s}$
        * $S = |\int_0^{10} (v(t)) dt| + |\int_{10}^{12} (v(t)) dt|$

---

## Example 6, cont.

6. An object projected upward from the Earth's surface with an initial velocity of $98 \text{m/s}$.
    * What is the change in displacement in the first $12 \text{s}$ of motion and its distance travelled?
        * $v(t) = -9.81t + 98$
        * $s(t) = -4.91t^2 + 98t$
        * $S = |\int_0^{10} (v(t)) dt| + |\int_{10}^{12} (v(t)) dt|$
        * $S = |\int_0^{10} (-9.81t + 98) dt| + |\int_{10}^{12} (-9.81t + 98) dt|$

---

## Example 6, cont.

6. An object projected upward from the Earth's surface with an initial velocity of $98 \text{m/s}$.
    * What is the change in displacement in the first $12 \text{s}$ of motion and its distance travelled?
        * $S = |\int_0^{10} (-9.81t + 98) dt| + |\int_{10}^{12} (-9.81t + 98) dt|$
        * $S = |\eval{[-4.91t^2 + 98t + C]}{0}{10}| + |\eval{[-4.91t^2 + 98t + C]}{10}{12}|$
        * $S = |[-4.91(10)^2 + 98(10)] + [4.91(0)^2 - 98(0)]|$ $+ |[-4.91(12)^2 + 98(12)] + [4.91(10)^2 - 98(10)]|$
        * $S = |489| + |-20|$
        * $S = 509 \text{m}$

---

## Example 7: Functions as Integrals

7. Given $f(x) = 4 - x^2$, 
    * What is the meaning of the function $g$ if $g(x) = \int_1^x (4 - t^2) dt$?
        * Well, $f$ is the integrand of the definite integral.
        * $\therefore g' = f \wedge g = A$, such that $A = \int f(x) dx$.
        * $g$ is a function which accumulates signed area under $f$, from $1$ to some value $x$.

---

## Example 7, cont.

7. Given $f(x) = 4 - x^2$ and $g(x) = \int_1^x (4 - t^2) dt$, 
    * What is the value of $g(1)$, without doing any calculations?
        * $g(1) = \int_1^1 (4 - t^2) dt$
        * $g(1) = \int_1^1 f(t) dt$
        * Note that: $\int_a^a f(x) dx = 0$
        * $\therefore g(1) = 0$.

---

## Example 7, cont.

7. Given $f(x) = 4 - x^2$ and $g(x) = \int_1^x (4 - t^2) dt$, 
    * Evaluate $g(x)$, and use the result to verify the value of $g(1)$
        * $g(x) = \int_1^x (4 - t^2) dt = \eval{(4t - \frac{1}{3} t^3 + C)}{1}{x} = A(x) - A(1)$
        * $g(x) = (4x - \frac{1}{3} x^3 + C) - (4(1) - \frac{1}{3} (1)^3 + C)$
        * $g(x) = -\frac{1}{3} x^3 + 4x - \frac{11}{3}$
        * $g(1) = -\frac{1}{3} (1)^3 + 4(1) - \frac{11}{3}$
        * $g(1) = -\frac{1}{3} + \frac{12}{3} - \frac{11}{3}$
        * $g(1) = 0$

---

## Example 7, cont.

7. Given $f(x) = 4 - x^2$ and $g(x) = \int_1^x (4 - t^2) dt$, 
    * Is the value of $g(0)$ positive or negative?
        * **Theorem**: $g(0) < 0$.
        * **Proof**: Given $g(x) = -\frac{1}{3} x^3 + 4x - \frac{11}{3}$,
        $g(0) = -\frac{1}{3} (0)^3 + 4(0) - \frac{11}{3}$.
        * $g(0) = - \frac{11}{3}$
        * $-\frac{11}{3} < 0 \therefore g(0) < 0 \blacksquare.$

---

## Example 8

8. Determine the area enclosed by the function $f(x) = x^3 - 2x^2 - 5x + 6$ and the $x$-axis in the interval $[-2, 3]$.
    * *Area, not signed area.*
    * Determine the zeros of $f(x)$ in $[-2, 3]$.
        * $f(1) = 0$, so $(x - 1)$ must be a factor.
$$
    \begin{array}{c|rrrr}
        & 1 & -2 & -5 & 6 \\
        x - 1 & \downarrow & -1 & 1 & 6 \\
        \hline
        & 1 & -1 & -6 & 0 \\
    \end{array}
$$

---

## Example 8, cont.

8. Determine the area enclosed by the function $f(x) = x^3 - 2x^2 - 5x + 6$ and the $x$-axis in the interval $[-2, 3]$.
    * Determine the zeros of $f(x)$ in $[-2, 3]$.
        * $f(1) = 0$, so $(x - 1)$ must be a factor.
        * $f(x) = (x - 1)(x^2 - x - 6)$
        * $f(x) = (x - 1)(x + 2)(x - 3)$
        * $x = 1, -2, 3$.

---

## Example 8, cont.

8. Determine the area enclosed by the function $f(x) = x^3 - 2x^2 - 5x + 6$ and the $x$-axis in the interval $[-2, 3]$.
    * $x = 1, -2, 3$ (zeros)
    * $\Sigma A = |\int_{-2}^1 [f(x)] dx| + |\int_1^3 [f(x)] dx|$
    * $\int f(x) dx = \int (x^3 - 2x^2 - 5x + 6) dx$
    * $A(x) = \int (x^3 - 2x^2 - 5x + 6) dx =$ $\frac{1}{4} x^4 - \frac{2}{3} x^3 - \frac{5}{2} x^2 + 6x + C$

---

## Example 8, cont.

8. Determine the area enclosed by the function $f(x) = x^3 - 2x^2 - 5x + 6$ and the $x$-axis in the interval $[-2, 3]$.
    * $A(x) = \frac{1}{4} x^4 - \frac{2}{3} x^3 - \frac{5}{2} x^2 + 6x + C$
    * $\Sigma A = |A(1) - A(-2)| + |A(3) - A(1)|$ 
    * $\Sigma A = |[\frac{1}{4} (1)^4 - \frac{2}{3} (1)^3 - \frac{5}{2} (1)^2 + 6(1) + C]$ $- [\frac{1}{4} (-2)^4 - \frac{2}{3} (-2)^3 - \frac{5}{2} (-2)^2 + 6(-2) + C]|$ $+ |[\frac{1}{4} (3)^4 - \frac{2}{3} (3)^3 - \frac{5}{2} (3)^2 + 6(3) + C]$ $- [\frac{1}{4} (1)^4 - \frac{2}{3} (1)^3 - \frac{5}{2} (1)^2 + 6(1) + C]|$ 

---

## Example 8, cont.

8. Determine the area enclosed by the function $f(x) = x^3 - 2x^2 - 5x + 6$ and the $x$-axis in the interval $[-2, 3]$.
    * $\Sigma A = |[\frac{1}{4} (1)^4 - \frac{2}{3} (1)^3 - \frac{5}{2} (1)^2 + 6(1) + C]$ $- [\frac{1}{4} (-2)^4 - \frac{2}{3} (-2)^3 - \frac{5}{2} (-2)^2 + 6(-2) + C]|$ $+ |[\frac{1}{4} (3)^4 - \frac{2}{3} (3)^3 - \frac{5}{2} (3)^2 + 6(3) + C]$ $- [\frac{1}{4} (1)^4 - \frac{2}{3} (1)^3 - \frac{5}{2} (1)^2 + 6(1) + C]|$ 
    * $\Sigma A = \frac{253}{12} \approx 21.1$

---

## Average Value of a Function

* Consider $f(x) = x + 1$ in the interval $[2, 5]$.
* We know that the heights are $f(2) = 3$ and $f(5) = 6$.
* Since the function is linear, the average value in this interval would be $4.5$ ($\bar{x}(3, 6) = 4.5$).
* The average value and its width can be use to find the signed area of the region.
* In this case, given that $A = w \bar{x}$, where $w$ is the width of the interval, we get $A = (5 - 2)(4.5) = 13.5 \text{u}$.
* This area is also $A = \int_2^5 (x + 1) dx$.

---

## Average Value of a Function

* For $f(x) = x + 1$, this area is also $A = \int_2^5 (x + 1) dx$.
* This means that $\int_2^5 [f(x)] dx = (5 - 2)(4.5) = 13.5 \text{u}$.
* Any continuous function $y = f(x)$ must have some average value that occurs at least once within an interval $[a, b]$.
* $\therefore \int_a^b [f(x)] dx = (b - a)\bar{x}, \bar{x} = \frac{\int_a^b [f(x)] dx}{b - a}$

---

## Example 9

9. Determine the average value of $f(x) = \sec^2 x$ in the interval $[\frac{2\pi}{3}, \frac{5\pi}{6}]$.
    * $\bar{x} = \frac{\int_\frac{2\pi}{3}^\frac{5\pi}{6} [\sec^2 x] dx}{\frac{5\pi}{6} - \frac{2\pi}{3}}$
    * $\bar{x} = \frac{\eval{(\tan x + C)}{\frac{2\pi}{3}}{\frac{5\pi}{6}}}{\frac{\pi}{6}}$
    * $\bar{x} = \frac{6}{\pi} [(\tan \frac{5\pi}{6}) - (\tan \frac{2\pi}{3})]$
    * $\bar{x} = \frac{6}{\pi} [\sqrt{3} - \frac{1}{\sqrt{3}}]$
    * $\bar{x} = \frac{12}{\pi\sqrt{3}} \approx 2.21$

---

## Exercise for Readers

* Approximate signed area of $f(x) = 4 - x^2$, using LRAM with 4 rectangles, in the interval $[0, 4]$
* Evaluate each definite integral:
    * $\int_{-4}^3 (4 - x^2) dx$
    * $\int_\frac{\pi}{2}^\frac{5\pi}{3} (\sin t + \cos t) dt$
    * $\int_2^3 (\frac{1}{x}) dx$
    * $\int_{-1}^3 (e^{2p}) dp$

---

## Exercise for Readers, cont.

* Given $f(x) = x + 1, p(x) = \int_{-2}^x [f(t)] dt$,
    * Evaluate $p(x)$
    * Determine $p(-2), p(3), p(-3)$
* Determine the total area enclosed by $f(x) = \sin x$ in the interval $[\frac{\pi}{6}, \frac{4\pi}{3}]$.
* Evaluate $x$ if $\int_2^x (2t - 3) dt = 12$

---

## Exercise for Readers, cont.

* Determine $\int_2^5 [f(x)] dx$ if $\int_2^4 [f(x)] dx = 10$, and $\int_4^5 [f(x)] dx = -17$
* Determine $\int_2^5 [f(x)] dx$ if $\int_4^2 [f(x)] dx = 10$, and $\int_5^4 [f(x)] dx = -17$

---

# [Next Lesson](Lesson%204)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercise

* Approximate signed area of $f(x) = 4 - x^2$, using LRAM with 4 rectangles, in the interval $[0, 4]$
    * $\displaystyle A = \sum_{i = 0}^4 (4 - i^2) =$ $(4 - 0^2) + (4 - 1^2) + (4 - 2^2) + (4 - 3^2)$
    * $A = 4 + (4 - 1) + (4 - 4) + (4 - 9)$
    * $A = 4 + 3 - 5$
    * $A = 2$

---

## Answers to Exercise, cont.

* Evaluate $\int_{-4}^3 (4 - x^2) dx$
    * $\eval{(4x - \frac{1}{3}x^3)}{-4}{3} = [4(3) - \frac{1}{3}(3)^3] - [4(-4) - \frac{1}{3}(-4)^3]$
    * $\frac{7}{3}$
* Evaluate $\int_\frac{\pi}{2}^\frac{5\pi}{3} (\sin t + \cos t) dt$
    * $\eval{(\sin t - \cos t)}{\frac{\pi}{2}}{\frac{5\pi}{3}} =$ $[\sin (\frac{5\pi}{3}) - \cos (\frac{5\pi}{3})] - [\sin (\frac{\pi}{2}) - \cos (\frac{\pi}{2})]$
    * $-\frac{3 + \sqrt{3}}{2}$

---

## Answers to Exercise, cont.

* Evaluate $\int_2^3 (\frac{1}{x}) dx$
    * $\eval{\ln |x|}{2}{3} = \ln |3| - \ln |2|$
    * $\ln \frac{3}{2}$
* Evaluate $\int_{-1}^3 (e^{2p}) dp$
    * $\eval{\frac{1}{2}e^{2p}}{-1}{3} = [\frac{1}{2}e^{2(3)}] - [\frac{1}{2}e^{2(-1)}]$
    * $\frac{e^8 - 1}{2e^2}$

---

## Answers to Exercise, cont.

* Given $f(x) = x + 1, p(x) = \int_{-2}^x [f(t)] dt$, evaluate $p(x)$
    * $p(x) = \eval{(\frac{1}{2}t^2 + t)}{x}{-2} = [\frac{1}{2}x^2 + x] - [\frac{1}{2}(-2)^2 + (-2)]$
    * $p(x) = \frac{1}{2}x^2 + x$
* Given $f(x) = x + 1, p(x) = \int_{-2}^x [f(t)] dt$, determine $p(-2), p(3), p(-3)$
    * $p(-2) = 0$
    * $p(3) = \frac{15}{2}$
    * $p(-3) = \frac{3}{2}$

---

## Answers to Exercise, cont.

* Determine the total area enclosed by $f(x) = \sin x$ in the interval $[\frac{\pi}{6}, \frac{4\pi}{3}]$.
    * $A = |\int_\frac{\pi}{6}^\frac{4\pi}{3} dx \sin x| = |\eval{(-\cos x)}{\frac{\pi}{6}}{\frac{4\pi}{3}}|$
    * $A = |\eval{(-\cos x)}{\frac{\pi}{6}}{\frac{4\pi}{3}}| = |[-\cos \frac{4\pi}{3}] - [-\cos \frac{\pi}{6}]|$
    * $A = \frac{1 + \sqrt{3}}{2}$
* Evaluate $x$ if $\int_2^x (2t - 3) dt = 12$
    * $\eval{(t^2 - 3t)}{2}{x} = [x^2 - 3x] - [2^2 - 3(2)] = 12$
    * $x^2 - 3x + 2 = 12$
    * $x^2 - 3x - 10 = 0$

---

## Answers to Exercise, cont.

* Evaluate $x$ if $\int_2^x (2t - 3) dt = 12$
    * $x^2 - 3x - 10 = 0$
    * $(x + 2)(x - 5) = 0$
    * $x = -2, 5$
* Determine $\int_2^5 [f(x)] dx$ if $\int_2^4 [f(x)] dx = 10$, and $\int_4^5 [f(x)] dx = -17$
    * $\int_2^5 [f(x)] dx = \int_2^4 [f(x)] dx + \int_4^5 [f(x)] dx$
    * $\int_2^5 [f(x)] dx = 10 - 17$
    * $\int_2^5 [f(x)] dx = -7$

---

## Answers to Exercise, cont.

* Determine $\int_2^5 [f(x)] dx$ if $\int_4^2 [f(x)] dx = 10$, and $\int_5^4 [f(x)] dx = -17$
    * $\int_2^5 [f(x)] dx = \int_4^2 [f(x)] dx + \int_5^4 [f(x)] dx$
    * $-\int_5^2 [f(x)] dx = 10 - 17$
    * $\int_5^2 [f(x)] dx = 7$

---

# [Next Lesson](Lesson%204)