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

$\newcommand\dd[3][]{\displaystyle\frac{d^{#1}#2}{d#3^{#1}}}$

---

# Lesson 4: Concavity and Inflection Points

---

<!--paginate: true-->

## Intro 

* In the same way the first derivative tells us about a function increasing or decreasing, 
* the second derivative tells us about the first derivative increasing or decreasing.
* This then tells us about the change in a function's *rate* of increase or decrease.
* This change is identified as concavity.

---

## Concavity

* A function is concave upward in an interval if its first derivative is increasing in that interval.
* A function is concave downward in an interval if its first derivative is decreasing in that interval.

---

## Concavity, cont.

* We can also think of this in terms of the slopes of the tangents as we move across the function.
* A function is concave upward if the slopes of the tangents are increasing in that interval.
* A function is concave downward if the slopes of the tangents are decreasing in that interval.

---

## Concavity and Inflection Points

* In terms of derivatives:
    * If $f''(x) > 0$ in an interval, then $f(x)$ is concave up, and $f'(x)$ is increasing in that interval.
    * If $f''(x) < 0$ in an interval, then $f(x)$ is concave down, and $f'(x)$ is decreasing in that interval.
    * If $f''(c) = 0$ or undefined, an inflection point *may* exist at $x = c$. 
    * This is the point where the concavity changes.

---

## Concavity and Inflection Points, cont.

* In order to confirm the existence of an inflection point at $x = c$, we must:
    * Use the second derivative to check the confavity of the intervals before and after $x = c$,
    * The function must exist at $x = c$, and
    * The $\text{sign}(f''(x))$ must change before and after $x = c$.

---

## Example 1

1. Find concavity intervals and inflection points of $y = x^3 + 2x^2 - 3x + 1$
    * Step 1: Determine second derivative and CV.
    * $\diff{x}^2 y = \diff{x}^2 (x^3 + 2x^2 - 3x + 1)$
    * $\diff{x}(\diff{x} y) = \diff{x} [\diff{x} (x^3) + \diff{x} (2x^2) - \diff{x} (3x) + \diff{x} (1)]$
    * $\diff{x}(\dd{y}{x}) = \diff{x} (3x^2) + \diff{x} (4x) - \diff{x} (3)$
    * $\dd[2]{y}{x} = 6x + 4$
    * CV: $x = -\frac{2}{3}$

---

## Example 1, cont.

1. Find concavity intervals and inflection points of $y = x^3 + 2x^2 - 3x + 1$
    * $\dd[2]{y}{x} = 6x + 4$
    * CV: $x = -\frac{2}{3}$
    * Step 2: Check Values.
    * $f''(-1) = -$ 

$$
    \begin{array}{ccc}
        \hline
        (-\infty, -\frac{2}{3}) & | &  (-\frac{2}{3}, \infty) \\
        CCD & -\frac{2}{3} & CCU/CCD
    \end{array}
$$

---

## Example 1, cont.

1. Find concavity intervals and inflection points of $y = x^3 + 2x^2 - 3x + 1$
    * $\dd[2]{y}{x} = 6x + 4$
    * CV: $x = -\frac{2}{3}$
    * Step 2: Check Values.
    * $f''(0) = +$ 

$$
    \begin{array}{ccc}
        \hline
        (-\infty, -\frac{2}{3}) & | &  (-\frac{2}{3}, \infty) \\
        CCD & -\frac{2}{3} & CCU
    \end{array}
$$

---

## Example 1, cont.

1. Find concavity intervals and inflection points of $y = x^3 + 2x^2 - 3x + 1$
    * CCU: $(-\frac{2}{3}, \infty)$
    * CCD: $(-\infty, -\frac{2}{3})$
    * Inflection Point:
        * $y = (-\frac{2}{3})^3 + 2(-\frac{2}{3})^2 - 3(-\frac{2}{3}) + 1$
        * $y = -\frac{8}{3^3} + \frac{8}{3^2} + 2 + 1$
        * $y = \frac{3(8)+ 3^4 - 8}{3^3}$
        * $y = \frac{97}{27}$

---

## Example 1, cont.

1. Find concavity intervals and inflection points of $y = x^3 + 2x^2 - 3x + 1$
    * CCU: $(-\frac{2}{3}, \infty)$
    * CCD: $(-\infty, -\frac{2}{3})$
    * Inflection Point: $(-\frac{2}{3}, \frac{97}{27})$

---

## Example 2

2. Find concavity intervals and inflection points of $f(x) = \frac{1}{4}x^4 - x^3 - 2x + 5$
    * Step 1: Determine second derivative and CV.
       * $\diff{x}^2 f(x) = \diff{x}^2 (\frac{1}{4}x^4 - x^3 - 2x + 5)$ 
       * $\diff{x} (\diff{x} f(x)) = \diff{x} [\diff{x} (\frac{1}{4}x^4) - \diff{x} (x^3) - \diff{x} (2x) + \diff{x} (5)]$
       * $\diff{x} f'(x) = \diff{x} (x^3 - 3x^2 - 2)$
       * $\diff{x} f'(x) = \diff{x} (x^3) - \diff{x} (3x^2) - \diff{x} (2)$
       * $f''(x) = 3x^2 - 6x$
       * $3x(x - 2) = 0$
       * CV: $x = 0, 2$

---

## Example 2, cont.

2. Find concavity intervals and inflection points of $f(x) = \frac{1}{4}x^4 - x^3 - 2x + 5$
    * $f''(x) = 3x^2 - 6x$
    * CV: $x = 0, 2$
    * Step 2: Check Values.
    * $f''(-1) = +$ 

$$
    \begin{array}{ccc}
        \hline
        (-\infty, 0) & | &  (0, 2) & | & (2, \infty) \\
        CCU & 0 & CCU/CCD & 2 & CCU/CCD
    \end{array}
$$

---

## Example 2, cont.

2. Find concavity intervals and inflection points of $f(x) = \frac{1}{4}x^4 - x^3 - 2x + 5$
    * $f''(x) = 3x^2 - 6x$
    * CV: $x = 0, 2$
    * Step 2: Check Values.
    * $f''(1) = -$ 

$$
    \begin{array}{ccc}
        \hline
        (-\infty, 0) & | &  (0, 2) & | & (2, \infty) \\
        CCU & 0 & CCD & 2 & CCU/CCD
    \end{array}
$$

---

## Example 2, cont.

2. Find concavity intervals and inflection points of $f(x) = \frac{1}{4}x^4 - x^3 - 2x + 5$
    * $f''(x) = 3x^2 - 6x$
    * CV: $x = 0, 2$
    * Step 2: Check Values.
    * $f''(3) = +$ 

$$
    \begin{array}{ccc}
        \hline
        (-\infty, 0) & | &  (0, 2) & | & (2, \infty) \\
        CCU & 0 & CCD & 2 & CCU
    \end{array}
$$

---

## Example 2, cont.

2. Find concavity intervals and inflection points of $f(x) = \frac{1}{4}x^4 - x^3 - 2x + 5$
    * CCU: $(-\infty, 0) \cup (2, \infty)$
    * CCD: $(0, 2)$
    * Inflection Points:
        * $f(0) = \frac{1}{4}(0)^4 - (0)^3 - 2(0) + 5$
        * $f(0) = 5$

---

## Example 2, cont.

2. Find concavity intervals and inflection points of $f(x) = \frac{1}{4}x^4 - x^3 - 2x + 5$
    * CCU: $(-\infty, 0) \cup (2, \infty)$
    * CCD: $(0, 2)$
    * Inflection Points: $(0, 5)$
        * $f(2) = \frac{1}{4}(2)^4 - (2)^3 - 2(2) + 5$
        * $f(2) = \frac{16}{4} - 8 - 4 + 5$
        * $f(2) = 4 - 8 - 4 + 5$
        * $f(2) = -3$

---

## Example 2, cont.

2. Find concavity intervals and inflection points of $f(x) = \frac{1}{4}x^4 - x^3 - 2x + 5$
    * CCU: $(-\infty, 0) \cup (2, \infty)$
    * CCD: $(0, 2)$
    * Inflection Points: $(0, 5)$, $(2, -3)$

---

## Example 3

3. Find concavity intervals and inflection points of $y = x - \cos x$, $x \in (0, 2\pi)$
    * $\diff{x}^2 y = \diff{x}^2 (x - \cos x)$
    * $\diff{x} (\diff{x} y) = \diff{x} [\diff{x} (x) - \diff{x} (\cos x)]$
    * $\diff{x} (\dd{y}{x}) = \diff{x} [1 + \sin x]$
    * $\diff{x} (\dd{y}{x}) = \diff{x} (1) + \diff{x} (\sin x)$
    * $\dd[2]{y}{x} = \cos x$

---

## Example 3, cont.

3. Find concavity intervals and inflection points of $y = x - \cos x$, $x \in (0, 2\pi)$
    * $\dd[2]{y}{x} = \cos x$
    * $\cos x = 0$
    * CV: $x = \frac{\pi}{2}, \frac{3\pi}{2}$

---

## Example 3, cont.

3. Find concavity intervals and inflection points of $y = x - \cos x$, $x \in (0, 2\pi)$
    * $\dd[2]{y}{x} = \cos x$
    * CV: $x = \frac{\pi}{2}, \frac{3\pi}{2}$
    * $\dd[2]{y}{x}(\frac{\pi}{3}) = +$

$$
    \begin{array}{ccc}
        \hline
        (0, \frac{\pi}{2}) & | &  (\frac{\pi}{2}, \frac{3\pi}{2}) & | & (\frac{3\pi}{2}, 2\pi) \\
        CCU & \frac{\pi}{2} & CC U/D & \frac{3\pi}{2} & CC U/D
    \end{array}
$$

---

## Example 3, cont.

3. Find concavity intervals and inflection points of $y = x - \cos x$, $x \in (0, 2\pi)$
    * $\dd[2]{y}{x} = \cos x$
    * CV: $x = \frac{\pi}{2}, \frac{3\pi}{2}$
    * $\dd[2]{y}{x}(\frac{5\pi}{3}) = +$

$$
    \begin{array}{ccc}
        \hline
        (0, \frac{\pi}{2}) & | &  (\frac{\pi}{2}, \frac{3\pi}{2}) & | & (\frac{3\pi}{2}, 2\pi) \\
        CCU & \frac{\pi}{2} & CC U/D & \frac{3\pi}{2} & CCU
    \end{array}
$$

---

## Example 3, cont.

3. Find concavity intervals and inflection points of $y = x - \cos x$, $x \in (0, 2\pi)$
    * $\dd[2]{y}{x} = \cos x$
    * CV: $x = \frac{\pi}{2}, \frac{3\pi}{2}$
    * $\dd[2]{y}{x}(\pi) = -$

$$
    \begin{array}{ccc}
        \hline
        (0, \frac{\pi}{2}) & | &  (\frac{\pi}{2}, \frac{3\pi}{2}) & | & (\frac{3\pi}{2}, 2\pi) \\
        CCU & \frac{\pi}{2} & CCD & \frac{3\pi}{2} & CCU
    \end{array}
$$

---

## Example 3, cont.

3. Find concavity intervals and inflection points of $y = x - \cos x$, $x \in (0, 2\pi)$
    * CCU: $(0, \frac{\pi}{2}) \cup (\frac{3\pi}{2}, 2\pi)$
    * CCD: $(\frac{\pi}{2}, \frac{3\pi}{2})$
    * Inflection Points:
        * $y = \frac{\pi}{2} - \cos \frac{\pi}{2}$
        * $y = \frac{\pi}{2}$
        * $y = \frac{3\pi}{2} - \cos \frac{3\pi}{2}$
        * $y = \frac{3\pi}{2}$

---

## Example 3, cont.

3. Find concavity intervals and inflection points of $y = x - \cos x$, $x \in (0, 2\pi)$
    * CCU: $(0, \frac{\pi}{2}) \cup (\frac{3\pi}{2}, 2\pi)$
    * CCD: $(\frac{\pi}{2}, \frac{3\pi}{2})$
    * Inflection Points: $(\frac{\pi}{2}, \frac{\pi}{2})$, $(\frac{3\pi}{2}, \frac{3\pi}{2})$

---

## Example 4

4. Find concavity intervals and inflection points of $y = \sqrt[3]{x}$
    * Inflection Point: $(0, 0)$
    * $\diff{x}^2 y = \diff{x}^2 x^\frac{1}{3}$
    * $\diff{x} (\diff{x} y) = \diff{x} (\diff{x} x^\frac{1}{3})$
    * $\diff{x} (\dd{y}{x}) = \diff{x} (\frac{1}{3}x^{-\frac{2}{3}})$
    * $\dd[2]{y}{x} = -\frac{2}{9}x^{-\frac{5}{3}}$

---

## Example 4, cont.

4. Find concavity intervals and inflection points of $y = \sqrt[3]{x}$
    * $\dd[2]{y}{x} = -\frac{2}{9}x^{-\frac{5}{3}}$
    * $\dd[2]{y}{x} = -\frac{2}{9\sqrt[3]{x^5}}$
    * $\dd[2]{y}{x}(0)$ is undefined, but is defined for the original function.

---

## Example 4, cont.

4. Find concavity intervals and inflection points of $y = \sqrt[3]{x}$
    * $\dd[2]{y}{x} = -\frac{2}{9\sqrt[3]{x^5}}$
    * $\dd[2]{y}{x} > 0$ in $(-\infty, 0)$
    * $\dd[2]{y}{x} < 0$ in $(0, \infty)$
    * Inflection Point: $(0, 0)$

---

# Lesson 4b: Sketching Curves

---

## Graphs

* In general, for continuous polynomial functions:
    * $f'(x) > 0$ when $f(x)$ is increasing
    * $f'(x) < 0$ when $f(x)$ is decreasing
    * $f'(x) = 0$ when $f(x)$ has an extremum
    * $f''(x) > 0$ when $f'(x)$ is increasing
    * $f''(x) < 0$ when $f'(x)$ is decreasing
    * $f''(x) = 0$ when $f(x)$ has an inflection point
    * $f''(x) > 0$ when $f(x)$ is concave up
    * $f''(x) < 0$ when $f(x)$ is concave down

---

## Example 1

1. Sketch the graph of $f(x) = 2x^2 - 9x - 5$ by examining:
    * Intervals of Increase / Decrease
    * Local Extrema
    * Concavity Intervals
    * Inflection Points
    * Intercepts

---

## Example 1, cont.

1. Sketch the graph of $f(x) = 2x^2 - 9x - 5$
    * $\diff{x} f(x) = \diff{x} (2x^2 - 9x - 5)$
    * $\diff{x} f(x) = \diff{x} (2x^2) - \diff{x} (9x) - \diff{x} (5)$
    * $f'(x) = 4x - 9$
    * $\diff{x} f'(x) = \diff{x} (4x - 9)$
    * $\diff{x} f'(x) = \diff{x} (4x) - \diff{x} (9)$
    * $f''(x) = 4$

---

## Example 1, cont.

1. Sketch the graph of $f(x) = 2x^2 - 9x - 5$
    * $f'(x) = 4x - 9$
    * $f''(x) = 4$
    * CV1: $x = \frac{9}{4}$
    * $f'(0) = -$ (Decreasing)
    * $f'(3) = +$ (Increasing)
    * CV1 is a minimum.
    * Minimum: $(\frac{9}{4}, f(\frac{9}{4}))$

---

## Example 1, cont.

1. Sketch the graph of $f(x) = 2x^2 - 9x - 5$
    * Minimum: 
        * $f(\frac{9}{4}) = 2(\frac{9}{4})^2 - 9(\frac{9}{4}) - 5$
        * $f(\frac{9}{4}) = 2(\frac{81}{(2^2)^2}) - \frac{81}{4} - 5$
        * $f(\frac{9}{4}) = \frac{81}{2^3} - \frac{81}{4} - 5$
        * $f(\frac{9}{4}) = \frac{81 - 2(81) - 5(8)}{8}$
        * $f(\frac{9}{4}) = -\frac{121}{8}$

---

## Example 1, cont.

1. Sketch the graph of $f(x) = 2x^2 - 9x - 5$
    * $y$-intercept
        * $f(0) = 2(0)^2 - 9(0) - 5$
        * $f(0) = - 5$
    * $x$-intercept
        * $0 = 2x^2 - 9x - 5$
        * $(2x + 1)(x - 5) = 0$
        * $x = 5, -\frac{1}{2}$

---

## Example 1, cont.

1. Sketch the graph of $f(x) = 2x^2 - 9x - 5$ by examining:
    * Intervals of Increase / Decrease
        * Inc: $(\frac{9}{4}, \infty)$
        * Dec: $(-\infty, \frac{9}{4})$
    * Local Extrema:
        * Minimum: $(\frac{9}{4}, -\frac{121}{8})$

---

## Example 1, cont.

1. Sketch the graph of $f(x) = 2x^2 - 9x - 5$ by examining:
    * Concavity Intervals:
        * Up: $(-\infty, \infty)$
    * Intercepts
        * $x$: $(-\frac{1}{2}, 0)$, $(5, 0)$
        * $y$: $(0, -5)$

---

## Example 2

2. Sketch the graph of $f(x) = 2x^3 - 3x^2 - 72x + 24$ by examining:
    * Intervals of Increase / Decrease
    * Local Extrema
    * Concavity Intervals
    * Inflection Points
    * $y$-Intercept

---

## Example 2, cont.

2. Sketch the graph of $f(x) = 2x^3 - 3x^2 - 72x + 24$
    * $\diff{x} f(x) = \diff{x} (2x^3 - 3x^2 - 72x + 24)$
    * $\diff{x} f(x) = \diff{x} (2x^3) - \diff{x} (3x^2) - \diff{x} (72x) + \diff{x} (24)$
    * $f'(x) = 6x^2 - 6x - 72$
    * $\diff{x} f'(x) = \diff{x} (6x^2 - 6x - 72)$
    * $\diff{x} f'(x) = \diff{x} (6x^2) - \diff{x} (6x) - \diff{x} (72)$
    * $f''(x) = 12x - 6$
    
---

## Example 2, cont.

2. Sketch the graph of $f(x) = 2x^3 - 3x^2 - 72x + 24$
    * $f'(x) = 6x^2 - 6x - 72$
    * $6(x^2 - x - 12) = 0$
    * $6(x + 3)(x - 4) = 0$
    * CV1: $x = 4, -3$
    * $f''(x) = 12x - 6$
    * $6(2x - 1) = 0$
    * CV2: $x = \frac{1}{2}$

---

## Example 2, cont.

2. Sketch the graph of $f(x) = 2x^3 - 3x^2 - 72x + 24$
    * $f'(x) = 6(x + 3)(x - 4)$
    * CV1: $x = 4, -3$
    * $f'(-5) = +$ (Increasing)
    * $f'(0) = -$ (Decreasing)
    * $f'(5) = +$ (Increasing)
    * $f''(x) = 6(2x - 1)$
    * CV2: $x = \frac{1}{2}$
    * $f''(0) = -$ (Concave Down)
    * $f''(1) = +$ (Concave Up)

---

## Example 2, cont.

2. Sketch the graph of $f(x) = 2x^3 - 3x^2 - 72x + 24$ by examining:
    * Intervals of Increase / Decrease
        * Inc: $(-\infty, -3) \cup (4, \infty)$
        * Dec: $(-3, 4)$
    * Local Extrema
        * Minimum: $(4, f(4))$
        * Maximum: $(-3, f(-3))$

---

## Example 2, cont.

2. Sketch the graph of $f(x) = 2x^3 - 3x^2 - 72x + 24$ by examining:
    * Concavity Intervals
        * Up: $(\frac{1}{2}, \infty)$
        * Down: $(-\infty, \frac{1}{2})$
    * Inflection Point:
        * $(\frac{1}{2}, f(\frac{1}{2}))$
    * $y$-intercept: $(0, 24)$

---

## Example 2, cont.

2. Sketch the graph of $f(x) = 2x^3 - 3x^2 - 72x + 24$
    * Minimum: $(4, f(4))$
        * $f(4) = 2(4)^3 - 3(4)^2 - 72(4) + 24$
        * $f(4) = 128 - 48 - 288 + 24$
        * $f(4) = -184$
    * Maximum: $(-3, f(-3))$
        * $f(-3) = 2(-3)^3 - 3(-3)^2 - 72(-3) + 24$
        * $f(-3) = -54 - 27 + 216 + 24$
        * $f(-3) = 159$

---

## Example 2, cont.

2. Sketch the graph of $f(x) = 2x^3 - 3x^2 - 72x + 24$
    * Inflection Point: $(\frac{1}{2}, f(\frac{1}{2}))$
        * $f(\frac{1}{2}) = 2(\frac{1}{2})^3 - 3(\frac{1}{2})^2 - 72(\frac{1}{2}) + 24$
        * $f(\frac{1}{2}) = 2(\frac{1}{2^3}) - 3(\frac{1}{2^2}) - 72(\frac{1}{2}) + 24$
        * $f(\frac{1}{2}) = \frac{1}{2^2} - \frac{3}{2^2} - \frac{72}{2} + 24$
        * $f(\frac{1}{2}) = \frac{1 - 3 - 72(2) + 24(4)}{4}$
        * $f(\frac{1}{2}) = \frac{1 - 3 - 144 + 96}{4}$
        * $f(\frac{1}{2}) = -\frac{50}{4}$

---

## Example 2, cont.

2. Sketch the graph of $f(x) = 2x^3 - 3x^2 - 72x + 24$ by examining:
    * Intervals of Increase / Decrease
        * Inc: $(-\infty, -3) \cup (4, \infty)$
        * Dec: $(-3, 4)$
    * Local Extrema
        * Minimum: $(4, -184)$
        * Maximum: $(-3, 159)$

---

## Example 2, cont.

2. Sketch the graph of $f(x) = 2x^3 - 3x^2 - 72x + 24$ by examining:
    * Concavity Intervals
        * Up: $(\frac{1}{2}, \infty)$
        * Down: $(-\infty, \frac{1}{2})$
    * Inflection Point:
        * $(\frac{1}{2}, -\frac{50}{4})$
    * $y$-intercept: $(0, 24)$

---

## Exercise for Readers

* Find the concavity intervals and inflection points for the following:
    * $f(x) = x^2 - 8x$
    * $f(x) = 5x^3 - 5x^2 + 8$
    * $f(x) = \frac{x^2 - 1}{x}$
    * $f(x) = 5 \cos (2x) - x$, $x \in (0, \pi)$

---

## Exercise for Readers, cont.

* Sketch the graph of $f(x) = 4x^3 - 3x^2 - 36x + 12$ by examining:
    * Intervals of Increase / Decrease
    * Local Extrema
    * Concavity Intervals
    * Inflection Points
    * $y$-Intercept

---

# [Next Lesson](Lesson%205)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Find the concavity intervals and inflection points for $f(x) = x^2 - 8x$
    * $\diff{x}^2 f(x) = \diff{x}^2 (x^2 - 8x)$
    * $\diff{x} (\diff{x} f(x)) = \diff{x} (\diff{x} (x^2) - \diff{x} (8x))$
    * $\diff{x} f'(x) = \diff{x} (2x - 8)$
    * $\diff{x} f'(x) = \diff{x} (2x) - \diff{x} (8)$
    * $f''(x) = 2$

---

## Answers to Exercises, cont.

* Find the concavity intervals and inflection points for $f(x) = x^2 - 8x$
    * Concavity:
        * Up: $(-\infty, \infty)$
        * Down: $\emptyset$
    * Inflection Points: None

---

## Answers to Exercises, cont.

* Find the concavity intervals and inflection points for $f(x) = 5x^3 - 5x^2 + 8$
    * $\diff{x}^2 f(x) = \diff{x}^2 (5x^3 - 5x^2 + 8)$
    * $\diff{x} (\diff{x} f(x)) = \diff{x} (\diff{x} (5x^3) - \diff{x} (5x^2) + \diff{x} (8))$
    * $\diff{x} f'(x) = \diff{x} (15x^2 - 10x)$
    * $\diff{x} f'(x) = \diff{x} (15x^2) - \diff{x} (10x)$
    * $f''(x) = 30x - 10$
    * CV: $10(3x - 1) = 0$
    * CV: $x = \frac{1}{3}$

---

## Answers to Exercises, cont.

* Find the concavity intervals and inflection points for $f(x) = 5x^3 - 5x^2 + 8$
    * $f''(x) = 10(3x - 1)$
    * CV: $x = \frac{1}{3}$
    * $f''(0) = 10(3(0) - 1)$
    * $f''(0) = -$ (Concave Down)
    * $f''(1) = 10(3(1) - 1)$
    * $f''(1) = +(+)$
    * $f''(1) = +$ (Concave Up)

---

## Answers to Exercises, cont.

* Find the concavity intervals and inflection points for $f(x) = 5x^3 - 5x^2 + 8$
    * Inflection Point: $x = \frac{1}{3}$
        * $f(\frac{1}{3}) = 5(\frac{1}{3})^3 - 5(\frac{1}{3})^2 + 8$
        * $f(\frac{1}{3}) = \frac{5}{3^3} - \frac{5}{3^2} + 8$
        * $f(\frac{1}{3}) = \frac{5}{3^3} - \frac{5(3)}{3^3} + \frac{8(3^3)}{3^3}$
        * $f(\frac{1}{3}) = \frac{5 - 5(3) + 8(3^3)}{3^3}$
        * $f(\frac{1}{3}) = \frac{5 - 15 + 216}{3^3}$
        * $f(\frac{1}{3}) = \frac{206}{27}$

---

## Answers to Exercises, cont.

* Find the concavity intervals and inflection points for $f(x) = 5x^3 - 5x^2 + 8$
    * Concavity:
        * Up: $(\frac{1}{3}, \infty)$
        * Down: $(-\infty, \frac{1}{3})$
    * Inflection Points: $(\frac{1}{3}, \frac{206}{27})$

---

## Answers to Exercises, cont.

* Find the concavity intervals and inflection points for $f(x) = \frac{x^2 - 1}{x}$
    * $\diff{x}^2 f(x) = \diff{x}^2 (\frac{x^2 - 1}{x})$
    * $\diff{x} (\diff{x} f(x)) = \diff{x} [\frac{(x) (\diff{x} (x^2 - 1)) - (x^2 - 1) (\diff{x} x)}{(x)^2}]$
    * $\diff{x} (\diff{x} f(x)) = \diff{x} [\frac{(x) (\diff{x} (x^2) - \diff{x} (1)) - (x^2 - 1) (\diff{x} x)}{(x)^2}]$
    * $\diff{x} f'(x) = \diff{x} [\frac{2x^2 - x^2 + 1}{x^2}]$
    * $\diff{x} f'(x) = \diff{x} [\frac{x^2 + 1}{x^2}]$
    * $\diff{x} f'(x) = \diff{x} [1 + \frac{1}{x^2}]$

---

## Answers to Exercises, cont.

* Find the concavity intervals and inflection points for $f(x) = \frac{x^2 - 1}{x}$
    * $\diff{x} f'(x) = \diff{x} [1 + \frac{1}{x^2}]$
    * $\diff{x} f'(x) = \diff{x} (1) + \diff{x} (x^{-2})$
    * $f''(x) = -2(x^{-3})$
    * $f''(x) = -\frac{2}{x^3}$

---

## Answers to Exercises, cont.

* Find the concavity intervals and inflection points for $f(x) = \frac{x^2 - 1}{x}$
    * Concavity:
        * Up: $(-\infty, 0)$
        * Down: $(0, \infty)$
    * Inflection Points: None

---

## Answers to Exercises, cont.

* Find the concavity intervals and inflection points for $f(x) = 5 \cos (2x) - x$, $x \in (0, \pi)$
    * $\diff{x}^2 f(x) = \diff{x}^2 (5 \cos (2x) - x)$
    * $\diff{x} (\diff{x} f(x)) = \diff{x} (\diff{x} (5 \cos 2x) - \diff{x} (x))$
    * $u = 2x$
    * $\diff{x} (\diff{x} f(x)) = \diff{x} (\diff{u} (5 \cos u) (\diff{x} 2x)) - \diff{x} (x))$
    * $\diff{x} f'(x) = \diff{x} (-10 \sin 2x) - \diff{x} (1)$
    * $\diff{x} f'(x) = (\diff{u} -10 \sin u (\diff{x} 2x)) - \diff{x} (1)$
    * $f''(x) = -20 \cos 2x$

---

## Answers to Exercises, cont.

* Find the concavity intervals and inflection points for $f(x) = 5 \cos (2x) - x$, $x \in (0, \pi)$
    * $f''(x) = -20 \cos 2x$
    * $-20 \cos 2x = 0$
    * CV: $x = \frac{\pi}{4}, \frac{3\pi}{4}$
    * $f''(\frac{\pi}{6}) = -$ (Concave Down)
    * $f''(\frac{\pi}{2}) = +$ (Concave Up)
    * $f''(\frac{5\pi}{6}) = -$ (Concave Down)

---

## Answers to Exercises, cont.

* Find the concavity intervals and inflection points for $f(x) = 5 \cos (2x) - x$, $x \in (0, \pi)$
    * Concavity:
        * Up: $(\frac{\pi}{4}, \frac{3\pi}{4})$
        * Down: $(0, \frac{\pi}{4}) \cup (\frac{3\pi}{4}, \pi)$
    * Inflection Points: $(\frac{\pi}{4}, -\frac{\pi}{4})$, $(\frac{3\pi}{4}, -\frac{3\pi}{4})$

---

## Answers to Exercises, cont.

* Sketch the graph of $f(x) = 4x^3 - 3x^2 - 36x + 12$ by examining:
    * Intervals of Increase / Decrease
    * Local Extrema
    * Concavity Intervals
    * Inflection Points
    * $y$-Intercept: $(0, 12)$

---

## Answers to Exercises, cont.

* Sketch the graph of $f(x) = 4x^3 - 3x^2 - 36x + 12$
    * $\diff{x} f(x) = \diff{x} (4x^3 - 3x^2 - 36x + 12)$
    * $\diff{x} f(x) = \diff{x} (4x^3) - \diff{x} (3x^2) - \diff{x} (36x) + \diff{x} (12)$
    * $f'(x) = 12x^2 - 6x - 36$
    * $6(2x^2 - x - 6) = 0$
    * $6(2x + 3)(x - 2) = 0$
    * CV1: $x = 2, -\frac{3}{2}$

---

## Answers to Exercises, cont.

* Sketch the graph of $f(x) = 4x^3 - 3x^2 - 36x + 12$
    * $\diff{x} f'(x) = \diff{x} (12x^2 - 6x - 36)$
    * $\diff{x} f'(x) = \diff{x} (12x^2) - \diff{x} (6x) - \diff{x} (36)$
    * $f''(x) = 24x - 6$
    * $6(4x - 1) = 0$
    * CV2: $x = \frac{1}{4}$

---

## Answers to Exercises, cont.

* Sketch the graph of $f(x) = 4x^3 - 3x^2 - 36x + 12$
    * $f'(x) = 6(2x + 3)(x - 2)$
    * CV1: $x = 2, -\frac{3}{2}$
        * $f'(-2) = +$ (Increasing)
        * $f'(0) = -$ (Decreasing)
        * $f'(3) = +$ (Increasing)
    * $f''(x) = 6(4x - 1)$
    * CV2: $x = \frac{1}{4}$
        * $f''(0) = -$ (Concave Down)
        * $f''(1) = +$ (Concave Up)

---

## Answers to Exercises, cont.

* Sketch the graph of $f(x) = 4x^3 - 3x^2 - 36x + 12$ by examining:
    * Intervals of Increase / Decrease
        * Increase: $(-\infty, -\frac{3}{2}) \cup (2, \infty)$
        * Decrease: $(-\frac{3}{2}, 2)$
    * Local Extrema: 
        * Maximum: $x = -\frac{3}{2}$
        * Minimum: $x = 2$

---

## Answers to Exercises, cont.

* Sketch the graph of $f(x) = 4x^3 - 3x^2 - 36x + 12$
    * Local Minimum:
        * $f(2) = 4(2)^3 - 3(2)^2 - 36(2) + 12$
        * $f(2) = 32 - 12 - 72 + 12$
        * $f(2) = -40$
    * Local Maximum
        * $f(-\frac{3}{2}) = 4(-\frac{3}{2})^3 - 3(-\frac{3}{2})^2 - 36(-\frac{3}{2}) + 12$
        * $f(-\frac{3}{2}) = -\frac{27}{2} - \frac{27}{4} + 54 + 12$
        * $f(-\frac{3}{2}) = \frac{237}{4}$

---

## Answers to Exercises, cont.

* Sketch the graph of $f(x) = 4x^3 - 3x^2 - 36x + 12$ by examining:
    * Concavity Intervals
        * Up: $(\frac{1}{4}, \infty)$
        * Down: $(-\infty, \frac{1}{4})$
    * Inflection Points: $x = \frac{1}{4}$
        * $f(\frac{1}{4}) = 4(\frac{1}{4})^3 - 3(\frac{1}{4})^2 - 36(\frac{1}{4}) + 12$
        * $f(\frac{1}{4}) = \frac{1}{16} - \frac{3}{16} - 9 + 12$
        * $f(\frac{1}{4}) = \frac{23}{8}$

---

## Answers to Exercises, cont.

* Sketch the graph of $f(x) = 4x^3 - 3x^2 - 36x + 12$ by examining:
    * Intervals of Increase / Decrease
        * Increase: $(-\infty, -\frac{3}{2}) \cup (2, \infty)$
        * Decrease: $(-\frac{3}{2}, 2)$
    * Local Extrema: 
        * Maximum: $(-\frac{3}{2}, \frac{237}{4})$
        * Minimum: $(2, -40)$

---

## Answers to Exercises, cont.

* Sketch the graph of $f(x) = 4x^3 - 3x^2 - 36x + 12$ by examining:
    * Concavity Intervals
        * Up: $(\frac{1}{4}, \infty)$
        * Down: $(-\infty, \frac{1}{4})$
    * Inflection Points: $(\frac{1}{4}, \frac{23}{8})$
    * $y$-Intercept: $(0, 12)$

---

# [Next Lesson](Lesson%205)