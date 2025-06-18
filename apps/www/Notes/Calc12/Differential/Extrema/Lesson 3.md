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

# Lesson 3: Local Extrema and Increasing / Decreasing Intervals

---

<!--paginate: true-->

## Intro 

* A *Local Extremum* occurs at a point on a function if the value at that point is either larger or smaller than the values in the near vicinity of that point.
* These can be between an increasing and decreasing interval (Local Maximum), or between a decreasing and increasing interval (Local Minimum).

---

## Intro, cont.

* Let's assume some function $f(x)$, which is increasing on the intervals $(1,3)$ and $(5,8)$, and decreasing on $(3,5)$.
* This function has end points $(1,1)$ and $(8,7)$.
* Since $f(x)$ isn't increasing or decreasing at $x = 3$ and $x = 5$, these are critical values and may be potential extrema.

---

## Intro, cont.

* Based on the information given, we know this:
    * $f(x)$ is increasing at $x < 3$, and decreasing for $x > 3$. $x = 3$ is a local maximum with a value of 5.
    * $f(x)$ is decreasing at $x < 5$, and decreasing for $x > 5$. $x = 5$ is a local minimum with a value of 0.
    * $f(x)$'s greatest value is 7, at the point $(8, 7)$, an absolute maximum of 7 occurs at $x = 8$.
    * $f(x)$'s least value is 0, at the point $(5, 0)$, an absolute minimum of 0 occurs at $x = 5$.

---

## Intro, cont.

* The range value of 7 is a local and absolute maximum of this function.
* The range value of 0 is a local and absolute minimum of this function.
* The range value of 1 is a local minimum, but not an absolute minimum of this function.
* The endpoints must be considered when dealing with a restricted domain.

---

## Determining Local Extrema

* The derivative of a function represents the instantaneous rate of change of that function.
* The sign of the derivative indicates whether the function is increasing or decreasing as follows:
    * $f'(x) > 0$ means that $y = f(x)$ is increasing in that interval.
    * $f'(x) < 0$ means that $y = f(x)$ is decreasing in that interval.
    * $f'(x) = 0$ or $f'(x)$ is undefined means that $y = f(x)$ may have a local extremum. $x$ is a critical value.

---

## Example 1

1. Find the intervals and local extrema values for $f(x) = x^3 - 3x^2 - 24x + 2$
    * $\diff{x} f(x) = \diff{x} (x^3 - 3x^2 - 24x + 2)$
    * $\diff{x} f(x) = \diff{x} (x^3) - \diff{x} (3x^2) - \diff{x} (24x) + \diff{x} (2)$
    * $f'(x) = 3x^2 - 6x - 24$ (*Where does $f'(x) = 0$*?)
    * $3x^2 - 6x - 24 = 0$
    * $3(x^2 - 2x - 12) = 0$
    * $3(x - 4)(x + 2) = 0$
    * CV: $x = 4, -2$

---

## Example 1, cont.

1. Find the intervals and local extrema values for $f(x) = x^3 - 3x^2 - 24x + 2$
    * $f'(x) = 3(x - 4)(x + 2)$
    * CV: $x = 4, -2$

$$
    \begin{array}{ccccc}
        \hline
        (-\infty, -2) & | &  (-2, 4) & | & (4, \infty) \\
        I/D & -2 & I/D & 4 & I/D
    \end{array}
$$

---

## Example 1, cont.

1. Find the intervals and local extrema values for $f(x) = x^3 - 3x^2 - 24x + 2$
    * $f'(x) = 3(x - 4)(x + 2)$
    * $f'(-3) = 3((-3) - 4)((-3) + 2)$
    * $f'(-3) = +(-)(-)$
    * $f'(-3) = +$

$$
    \begin{array}{ccccc}
        \hline
        (-\infty, -2) & | &  (-2, 4) & | & (4, \infty) \\
        I & -2 & I/D & 4 & I/D
    \end{array}
$$

---

## Example 1, cont.

1. Find the intervals and local extrema values for $f(x) = x^3 - 3x^2 - 24x + 2$
    * $f'(x) = 3(x - 4)(x + 2)$
    * $f'(0) = 3(0 - 4)(0 + 2)$
    * $f'(0) = +(-)(+)$
    * $f'(0) = -$

$$
    \begin{array}{ccccc}
        \hline
        (-\infty, -2) & | &  (-2, 4) & | & (4, \infty) \\
        I & -2 & D & 4 & I/D
    \end{array}
$$

---

## Example 1, cont.

1. Find the intervals and local extrema values for $f(x) = x^3 - 3x^2 - 24x + 2$
    * $f'(x) = 3(x - 4)(x + 2)$
    * $f'(5) = 3(5 - 4)(5 + 2)$
    * $f'(5) = +(+)(+)$
    * $f'(5) = +$

$$
    \begin{array}{ccccc}
        \hline
        (-\infty, -2) & | &  (-2, 4) & | & (4, \infty) \\
        I & -2 (\text{Max}) & D & 4 (\text{Min}) & I
    \end{array}
$$

---

## Example 1, cont.

1. Find the intervals and local extrema values for $f(x) = x^3 - 3x^2 - 24x + 2$
    * Inc: $(-\infty, -2) \cup (4, \infty)$
    * Dec: $(-2, 4)$
    * Maximum: 
        * $f(-2) = (-2)^3 - 3(-2)^2 - 24(-2) + 2$
        * $f(-2) = - 8 - 12 + 48 + 2$
        * $f(-2) = 50 - 8 - 12$
        * $f(-2) = 42 - 12$
        * $f(-2) = 30$

---

## Example 1, cont.

1. Find the intervals and local extrema values for $f(x) = x^3 - 3x^2 - 24x + 2$
    * Inc: $(-\infty, -2) \cup (4, \infty)$
    * Dec: $(-2, 4)$
    * Maximum: $(-2, 30)$
    * Minimum:
        * $f(4) = (4)^3 - 3(4)^2 - 24(4) + 2$
        * $f(4) = 64 - 48 - 96 + 2$
        * $f(4) = -78$

---

## Example 1, cont.

1. Find the intervals and local extrema values for $f(x) = x^3 - 3x^2 - 24x + 2$
    * Inc: $(-\infty, -2) \cup (4, \infty)$
    * Dec: $(-2, 4)$
    * Maximum: $(-2, 30)$
    * Minimum: $(4, -78)$

---

## Example 2

2. Find the intervals and local extrema values for $f(x) = 2x^3 + \frac{x^2}{2} - 2x + 7$
    * $\diff{x} f(x) = \diff{x} (2x^3 + \frac{x^2}{2} - 2x + 7)$
    * $\diff{x} f(x) = \diff{x} (2x^3) + \diff{x} (\frac{x^2}{2}) - \diff{x} (2x) + \diff{x} (7)$
    * $f'(x) = 6x^2 + x - 2$
    * $6x^2 + x - 2 = 0$
    * $(3x + 2)(2x - 1) = 0$
    * CV: $x = -\frac{2}{3}, \frac{1}{2}$
    
---

## Example 2, cont.

2. Find the intervals and local extrema values for $f(x) = 2x^3 + \frac{x^2}{2} - 2x + 7$
    * $f'(x) = (3x + 2)(2x - 1)$
    * CV: $x = -\frac{2}{3}, \frac{1}{2}$

$$
    \begin{array}{ccccc}
        \hline
        (-\infty, -\frac{2}{3}) & | &  (-\frac{2}{3}, \frac{1}{2}) & | & (\frac{1}{2}, \infty) \\
        I/D & -\frac{2}{3} & I/D & \frac{1}{2} & I/D
    \end{array}
$$

---

## Example 2, cont.

2. Find the intervals and local extrema values for $f(x) = 2x^3 + \frac{x^2}{2} - 2x + 7$
    * $f'(x) = (3x + 2)(2x - 1)$
    * $f'(-1) = (3(-1) + 2)(2(-1) - 1)$
    * $f'(-1) = (-)(-)$
    * $f'(-1) = +$

$$
    \begin{array}{ccccc}
        \hline
        (-\infty, -\frac{2}{3}) & | &  (-\frac{2}{3}, \frac{1}{2}) & | & (\frac{1}{2}, \infty) \\
        I & -\frac{2}{3} & I/D & \frac{1}{2} & I/D
    \end{array}
$$

---

## Example 2, cont.

2. Find the intervals and local extrema values for $f(x) = 2x^3 + \frac{x^2}{2} - 2x + 7$
    * $f'(x) = (3x + 2)(2x - 1)$
    * $f'(0) = (3(0) + 2)(2(0) - 1)$
    * $f'(0) = (+)(-)$
    * $f'(0) = -$

$$
    \begin{array}{ccccc}
        \hline
        (-\infty, -\frac{2}{3}) & | &  (-\frac{2}{3}, \frac{1}{2}) & | & (\frac{1}{2}, \infty) \\
        I & -\frac{2}{3} & D & \frac{1}{2} & I/D
    \end{array}
$$

---

## Example 2, cont.

2. Find the intervals and local extrema values for $f(x) = 2x^3 + \frac{x^2}{2} - 2x + 7$
    * $f'(x) = (3x + 2)(2x - 1)$
    * $f'(1) = (3 + 2)(2 - 1)$
    * $f'(1) = (+)(+)$
    * $f'(1) = +$

$$
    \begin{array}{ccccc}
        \hline
        (-\infty, -\frac{2}{3}) & | &  (-\frac{2}{3}, \frac{1}{2}) & | & (\frac{1}{2}, \infty) \\
        I & -\frac{2}{3} & D & \frac{1}{2} & I
    \end{array}
$$

---

## Example 2, cont.

2. Find the intervals and local extrema values for $f(x) = 2x^3 + \frac{x^2}{2} - 2x + 7$
    * Inc: $(-\infty, -\frac{2}{3}) \cup (\frac{1}{2}, \infty)$
    * Dec: $(-\frac{2}{3}, \frac{1}{2})$
    * Maximum:
        * $f(-\frac{2}{3}) = 2(-\frac{2}{3})^3 + \frac{(\frac{2}{3})^2}{2} - 2(-\frac{2}{3}) + 7$
        * $f(-\frac{2}{3}) = \frac{2}{3^2} + \frac{4}{3} + 7 - \frac{16}{3^3}$
        * $f(-\frac{2}{3}) = \frac{6 + 4(9) + 7(27) - 16}{27}$
        * $f(-\frac{2}{3}) = \frac{215}{27}$

---

## Example 2, cont.

2. Find the intervals and local extrema values for $f(x) = 2x^3 + \frac{x^2}{2} - 2x + 7$
    * Inc: $(-\infty, -\frac{2}{3}) \cup (\frac{1}{2}, \infty)$
    * Dec: $(-\frac{2}{3}, \frac{1}{2})$
    * Maximum: $(-\frac{2}{3}, \frac{215}{27})$
    * Minimum:
        * $f(\frac{1}{2}) = 2(\frac{1}{2})^3 + \frac{(\frac{1}{2})^2}{2} - 2(\frac{1}{2}) + 7$
        * $f(\frac{1}{2}) = \frac{1}{2^2} + \frac{1}{2^3} - 1 + 7$
        * $f(\frac{1}{2}) = \frac{51}{8}$

---

## Example 2, cont.

2. Find the intervals and local extrema values for $f(x) = 2x^3 + \frac{x^2}{2} - 2x + 7$
    * Inc: $(-\infty, -\frac{2}{3}) \cup (\frac{1}{2}, \infty)$
    * Dec: $(-\frac{2}{3}, \frac{1}{2})$
    * Maximum: $(-\frac{2}{3}, \frac{215}{27})$
    * Minimum: $(\frac{1}{2}, \frac{51}{8})$

---

## Example 3

3. Find the intervals and local extrema values for $f(x) = \sin^2 x$, $x \in (0, 2\pi]$
    * $y = u^2$
    * $u = \sin x$
    * $\diff{x} f(x) = \diff{u} u^2 (\diff{x} \sin x)$
    * $f'(x) = 2(\sin x)(\cos x)$
    * $2(\sin x)(\cos x) = 0$
    * CV: $x = \frac{n\pi}{2}, 1 \le n \le 4$
    
    
---

## Example 3, cont.

3. Find the intervals and local extrema values for $f(x) = \sin^2 x$, $x \in (0, 2\pi]$
    * $f'(x) = 2(\sin x)(\cos x)$
    * CV: $x = \frac{n\pi}{2}, 1 \le n \le 4$

$$
    \begin{array}{cccccccc}
        \hline
        (0, \frac{\pi}{2}) & | & (\frac{\pi}{2}, \pi) & | & (\pi, \frac{3\pi}{2}) & | & (\frac{3\pi}{2}, 2\pi) & | \\
        I/D & \frac{\pi}{2} & I/D & \pi & I/D & \frac{3\pi}{2} & I/D & 2\pi
    \end{array}
$$

---

## Example 3, cont.

3. Find the intervals and local extrema values for $f(x) = \sin^2 x$, $x \in (0, 2\pi]$

$$
    \begin{array}{cccccccc}
        \hline
        (0, \frac{\pi}{2}) & | & (\frac{\pi}{2}, \pi) & | & (\pi, \frac{3\pi}{2}) & | & (\frac{3\pi}{2}, 2\pi) & | \\
        I & \frac{\pi}{2} & D & \pi & I & \frac{3\pi}{2} & D & 2\pi
    \end{array}
$$

---

## Example 3, cont.

3. Find the intervals and local extrema values for $f(x) = \sin^2 x$, $x \in (0, 2\pi]$
    * Inc: $(0, \frac{\pi}{2}) \cup (\pi, \frac{3\pi}{2})$
    * Dec: $(\frac{\pi}{2}, \pi) \cup (\frac{3\pi}{2}, 2\pi)$
    * Maxima:
        * $f(\frac{\pi}{2}) = \sin^2 \frac{\pi}{2}$
        * $f(\frac{\pi}{2}) = 1$
        * $f(\frac{3\pi}{2}) = \sin^2 \frac{3\pi}{2}$
        * $f(\frac{3\pi}{2}) = 1$

---

## Example 3, cont.

3. Find the intervals and local extrema values for $f(x) = \sin^2 x$, $x \in (0, 2\pi]$
    * Inc: $(0, \frac{\pi}{2}) \cup (\pi, \frac{3\pi}{2})$
    * Dec: $(\frac{\pi}{2}, \pi) \cup (\frac{3\pi}{2}, 2\pi)$
    * Maxima: $(\frac{\pi}{2}, 1), (\frac{3\pi}{2}, 1)$
    * Minima: $(\pi, 0), (2\pi, 0)$

---

## Example 4

* A Local Extremum can exist at a domain value where the first derivative is undefined.
4. Find the intervals and local extrema values for $f(x) = x^\frac{2}{3}$
    * The function obviously has a local minimum at the point $(0,0)$. *But why?*
    * $\diff{x} f(x) = \diff{x} (x^\frac{2}{3})$
    * $f'(x) = \frac{2}{3}(x^{-\frac{1}{3}})$
    * $f'(x) = \frac{2}{3\sqrt[3]{x}}$

---

## Example 4, cont.

4. Find the intervals and local extrema values for $f(x) = x^\frac{2}{3}$
    * $f'(0)$ isn't defined, but $f(x)$ is defined at $x = 0$.
    * $f'(x) < 0$ in the interval $(-\infty, 0)$, meaning $f(x)$ is decreasing in this interval.
    * $f'(x) > 0$ in the interval $(0, \infty)$, meaning $f(x)$ is increasing in this interval.
    * Since the sign of the derivative changes across $x = 0$ and $f(x)$ is defined at $x = 0$, the original function reached a local minimum at the point $(0,0)$.

---

## Exercise for Readers

* State the intervals and determine the local extrema values for the following:
    * $y = 2x^2 - 16x + 39$
    * $f(x) = \frac{2}{x - 3}$
    * $f(x) = 3 \sin x + 2$, $x \in [0, 2\pi]$
    * $y = 2 \cos^2 (2x)$, $x \in (0, \frac{3\pi}{4})$

---

# [Next Lesson](Lesson%204)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* State the intervals and determine the local extrema values for $y = 2x^2 - 16x + 39$
    * $\diff{x} y = \diff{x} (2x^2 - 16x + 39)$
    * $\diff{x} y = \diff{x} (2x^2) - \diff{x} (16x) + \diff{x} (39)$
    * $\dd[y]{x} = 4x - 16$
    * $4(x - 4) = 0$
    * CV: $x = 4$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $y = 2x^2 - 16x + 39$
    * $\dd[y]{x} = 4(x - 4)$
    * CV: $x = 4$
    * $\dd[y]{x}(0) = -$

$$
    \begin{array}{ccc}
        \hline
        (-\infty, 4) & | & (4, \infty) \\
        D & 4 & I/D
    \end{array}
$$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $y = 2x^2 - 16x + 39$
    * $\dd[y]{x} = 4(x - 4)$
    * CV: $x = 4$
    * $\dd[y]{x}(5) = +$

$$
    \begin{array}{ccc}
        \hline
        (-\infty, 4) & | & (4, \infty) \\
        D & 4 & I
    \end{array}
$$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $y = 2x^2 - 16x + 39$
    * Inc: $(4, \infty)$
    * Dec: $(-\infty, 4)$
    * Minimum:
        * $y = 2(4)^2 - 16(4) + 39$
        * $y = 32 - 64 + 39$
        * $y = 7$
        * $P(4, 7)$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $f(x) = \frac{2}{x - 3}$
    * $f(x) = 2(x - 3)^{-1}$
    * $y = 2u^{-1}$
    * $u = x - 3$
    * $\diff{x} f(x) = \diff{u} 2u^{-1} [\diff{x} (x - 3)]$
    * $\diff{x} f(x) = \diff{u} 2u^{-1} [\diff{x} (x) - \diff{x} (3)]$
    * $f'(x) = -\frac{2}{(x - 3)^2}$
    * $x - 3 \ne 0$
    * CV: $x = 3$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $f(x) = \frac{2}{x - 3}$
    * $f'(x) = -\frac{2}{(x - 3)^2}$
    * CV: $x = 3$
    * $f'(0) = -$
    * $f'(4) = -$

$$
    \begin{array}{ccc}
        \hline
        (-\infty, 3) & | & (3, \infty) \\
        D & 3 & D
    \end{array}
$$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $f(x) = \frac{2}{x - 3}$
    * Inc: $\emptyset$
    * Dec: $(-\infty, 3) \cup (3, \infty)$
    * Minimum: 
        * $f(3^-) = \frac{2}{(3^-) - 3}$
        * $f(3^-) = \frac{2}{0^-}$
        * $f(3^-) = -\infty$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $f(x) = \frac{2}{x - 3}$
    * Inc: $\emptyset$
    * Dec: $(-\infty, 3) \cup (3, \infty)$
    * Minimum: $(3, -\infty)$
    * Maximum: 
        * $f(3^+) = \frac{2}{(3^+) - 3}$
        * $f(3^+) = \frac{2}{0^+}$
        * $f(3^+) = \infty$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $f(x) = \frac{2}{x - 3}$
    * Inc: $\emptyset$
    * Dec: $(-\infty, 3) \cup (3, \infty)$
    * Minimum: $(3, -\infty)$
    * Maximum: $(3, \infty)$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $f(x) = 3 \sin x + 2$, $x \in [0, 2\pi]$
    * $\diff{x} f(x) = \diff{x} (3 \sin x + 2)$
    * $\diff{x} f(x) = \diff{x} (3 \sin x) + \diff{x} (2)$
    * $f'(x) = 3 \cos x$
    * $3 \cos x = 0$
    * CV: $x = 0, \frac{\pi}{2}, \frac{3\pi}{2}, 2\pi$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $f(x) = 3 \sin x + 2$, $x \in [0, 2\pi]$
    * $f'(x) = 3 \cos x$
    * CV: $x = 0, \frac{\pi}{2}, \frac{3\pi}{2}, 2\pi$
    * $f'(\frac{\pi}{4}) = 3 \cos \frac{\pi}{4} = +$
    * $f'(\frac{5\pi}{4}) = 3 \cos \frac{5\pi}{4} = +$
    * $f'(\pi) = 3 \cos \pi = -$

$$
    \begin{array}{cccccccc}
        \hline
        | & (0, \frac{\pi}{2}) & | & (\frac{\pi}{2}, \frac{3\pi}{2}) & | & (\frac{3\pi}{2}, 2\pi) & | \\
        0 & I & \frac{\pi}{2} & D & \frac{3\pi}{2} & I & 2\pi
    \end{array}
$$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $f(x) = 3 \sin x + 2$, $x \in [0, 2\pi]$
    * Inc: $(0, \frac{\pi}{2}) \cup (\frac{3\pi}{2}, 2\pi)$
    * Dec: $(\frac{\pi}{2}, \frac{3\pi}{2})$
    * Minimum: 
        * $f(\frac{3\pi}{2}) = 3 \sin \frac{3\pi}{2} + 2$
        * $f(\frac{3\pi}{2}) = 2 - 3$
        * $f(\frac{3\pi}{2}) = -1$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $f(x) = 3 \sin x + 2$, $x \in [0, 2\pi]$
    * Inc: $(0, \frac{\pi}{2}) \cup (\frac{3\pi}{2}, 2\pi)$
    * Dec: $(\frac{\pi}{2}, \frac{3\pi}{2})$
    * Minimum: $(\frac{3\pi}{2}, -1)$
        * $f(0) = 3 \sin 0 + 2$
        * $f(0) = 2$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $f(x) = 3 \sin x + 2$, $x \in [0, 2\pi]$
    * Inc: $(0, \frac{\pi}{2}) \cup (\frac{3\pi}{2}, 2\pi)$
    * Dec: $(\frac{\pi}{2}, \frac{3\pi}{2})$
    * Minimum: $(\frac{3\pi}{2}, -1)$, $(0, 2)$
    * Maximum: 
        * $f(\frac{\pi}{2}) = 3 \sin \frac{\pi}{2} + 2$
        * $f(\frac{\pi}{2}) = 3 + 2$
        * $f(\frac{\pi}{2}) = 5$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $f(x) = 3 \sin x + 2$, $x \in [0, 2\pi]$
    * Inc: $(0, \frac{\pi}{2}) \cup (\frac{3\pi}{2}, 2\pi)$
    * Dec: $(\frac{\pi}{2}, \frac{3\pi}{2})$
    * Minimum: $(\frac{3\pi}{2}, -1)$, $(0, 2)$
    * Maximum: $(\frac{\pi}{2}, 5)$
        * $f(2\pi) = 3 \sin 2\pi + 2$
        * $f(2\pi) = 2$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $f(x) = 3 \sin x + 2$, $x \in [0, 2\pi]$
    * Inc: $(0, \frac{\pi}{2}) \cup (\frac{3\pi}{2}, 2\pi)$
    * Dec: $(\frac{\pi}{2}, \frac{3\pi}{2})$
    * Minimum: $(\frac{3\pi}{2}, -1)$, $(0, 2)$
    * Maximum: $(\frac{\pi}{2}, 5)$, $(2\pi, 2)$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $y = 2 \cos^2 (2x)$, $x \in (0, \frac{3\pi}{4})$
    * $y = 2u^2$
    * $u = \cos v$
    * $v = 2x$
    * $\diff{x} y = [\diff{u} (2u^2)][\diff{v} (\cos v)][\diff{x} (2x)]$
    * $\dd[y]{x} = (4\cos 2x)(-\sin 2x)(2)$
    * $\dd[y]{x} = -8 \cos 2x \sin 2x$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $y = 2 \cos^2 (2x)$, $x \in (0, \frac{3\pi}{4})$
    * $\dd[y]{x} = -8 \cos 2x \sin 2x$
    * $-8 \cos 2x \sin 2x = 0$
    * CV: $x = \frac{n\pi}{4}$, $0 < n < 3$

$$
    \begin{array}{cccccccc}
        \hline
        | & (0, \frac{\pi}{4}) & | & (\frac{\pi}{4}, \frac{\pi}{2}) & | & (\frac{\pi}{2}, \frac{3\pi}{4}) & | \\
        0 & I/D & \frac{\pi}{4} & I/D & \frac{\pi}{2} & I/D & \frac{3\pi}{4}
    \end{array}
$$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $y = 2 \cos^2 (2x)$, $x \in (0, \frac{3\pi}{4})$
    * $\dd[y]{x} = -8 \cos 2x \sin 2x$
    * $\dd[y]{x}(\frac{\pi}{8}) = -$

$$
    \begin{array}{cccccccc}
        \hline
        | & (0, \frac{\pi}{4}) & | & (\frac{\pi}{4}, \frac{\pi}{2}) & | & (\frac{\pi}{2}, \frac{3\pi}{4}) & | \\
         & D & \frac{\pi}{4} & I/D & \frac{\pi}{2} & I/D & 
    \end{array}
$$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $y = 2 \cos^2 (2x)$, $x \in (0, \frac{3\pi}{4})$
    * $\dd[y]{x} = -8 \cos 2x \sin 2x$
    * $\dd[y]{x}(\frac{3\pi}{8}) = +$

$$
    \begin{array}{cccccccc}
        \hline
        | & (0, \frac{\pi}{4}) & | & (\frac{\pi}{4}, \frac{\pi}{2}) & | & (\frac{\pi}{2}, \frac{3\pi}{4}) & | \\
        & D & \frac{\pi}{4} & I & \frac{\pi}{2} & I/D & 
    \end{array}
$$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $y = 2 \cos^2 (2x)$, $x \in (0, \frac{3\pi}{4})$
    * $\dd[y]{x} = -8 \cos 2x \sin 2x$
    * $\dd[y]{x}(\frac{5\pi}{8}) = -$

$$
    \begin{array}{cccccccc}
        \hline
        | & (0, \frac{\pi}{4}) & | & (\frac{\pi}{4}, \frac{\pi}{2}) & | & (\frac{\pi}{2}, \frac{3\pi}{4}) & | \\
        & D & \frac{\pi}{4} & I & \frac{\pi}{2} & D &
    \end{array}
$$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $y = 2 \cos^2 (2x)$, $x \in (0, \frac{3\pi}{4})$
    * Inc: $(\frac{\pi}{4}, \frac{\pi}{2})$
    * Dec: $(0, \frac{\pi}{4}) \cup (\frac{\pi}{2}, \frac{4\pi}{4})$
    * Minima:
        * $y = 2 \cos^2 (2\frac{\pi}{4})$
        * $y = 2 \cos^2 (\frac{\pi}{2})$
        * $y = 2 (0)$
        * $y = 0$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $y = 2 \cos^2 (2x)$, $x \in (0, \frac{3\pi}{4})$
    * Inc: $(\frac{\pi}{4}, \frac{\pi}{2})$
    * Dec: $(0, \frac{\pi}{4}) \cup (\frac{\pi}{2}, \frac{4\pi}{4})$
    * Minima: $(\frac{\pi}{4}, 0)$
        * $y = 2 \cos^2 (2\frac{3\pi}{4})$
        * $y = 2 \cos^2 (\frac{3\pi}{2})$
        * $y = 2 (0)$
        * $y = 0$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $y = 2 \cos^2 (2x)$, $x \in (0, \frac{3\pi}{4})$
    * Inc: $(\frac{\pi}{4}, \frac{\pi}{2})$
    * Dec: $(0, \frac{\pi}{4}) \cup (\frac{\pi}{2}, \frac{4\pi}{4})$
    * Minimum: $(\frac{\pi}{4}, 0)$
    * Maximum:
        * $y = 2 \cos^2 (2\frac{\pi}{2})$
        * $y = 2 \cos^2 (\pi)$
        * $y = 2 (1)$
        * $y = 2$

---

## Answers to Exercises, cont.

* State the intervals and determine the local extrema values for $y = 2 \cos^2 (2x)$, $x \in (0, \frac{3\pi}{4})$
    * Inc: $(\frac{\pi}{4}, \frac{\pi}{2})$
    * Dec: $(0, \frac{\pi}{4}) \cup (\frac{\pi}{2}, \frac{4\pi}{4})$
    * Minimum: $(\frac{\pi}{4}, 0)$
    * Maximum: $(\frac{\pi}{2}, 2)$

---

# [Next Lesson](Lesson%204)