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

# Lesson 2: Limits & Tangent Lines

---

<!--paginate: true-->

## Intro

* Now that we have established a basic understanding of limits, let's summarize some basic properties:
    * $\limit{x}{a} cf(x) = c \limit{x}{a} f(x)$, where $c$ is a constant.
    * $\limit{x}{a} [f(x) + g(x)] = \limit{x}{a} f(x) + \limit{x}{a} g(x)$
    * $\limit{x}{a} f(x)g(x) = \limit{x}{a} f(x) \limit{x}{a} g(x)$
    * $\limit{x}{a} \frac{f(x)}{g(x)} = \frac{\limit{x}{a} f(x)}{ \limit{x}{a} g(x)}$
* Previous examples have used these properties.

---

## Secant Lines

* Consider the curve $f(x) = x^2$ with points $P(1,1) \text{ and } Q(2,4)$
* A straight line through $P$ and $Q$ is called a *secant line*. They intersect the curve in at least two points.
* The slope ($m$) is the same slope formula you're familiar with: $m = \frac{y_2 - y_1}{x_2 - x_1}$
* In this example, we get that $m = \frac{3}{1}$
* As such, we get that $m = \frac{y_2 - y_1}{h}$, where $h$ represents a change in $x$.

---

## General Slope Form

* Take two points on a curve:
    * $P(x_1, y_1) = P(x, f(x))$
    * $Q(x_2, y_2) = Q(x + h, f(x + h))$
* We get that the slope is as follows:
    * $m_\overline{PQ} = \frac{f(x + h) - f(x)}{(x + h) - x}$
    * $m_\overline{PQ} = \frac{f(x + h) - f(x)}{h}$
* This is the *Mean Rate of Change* of the function over that interval.

---

## Tangent Line

* Note that $m_{\overline{PQ}} = \frac{f(x + h) - f(x)}{h}$
    * As $Q \to P$, the secant line becomes a Tangent Line.
    * Meaning, as $Q \to P,\ h \to 0$.
    * $\therefore m_P = \limit{h}{0} \frac{f(x + h) - f(x)}{h}$
* This is the *Instantaneous Rate Of Change* of the function at $P$.
* Take note, you'll need it for later!
* Here, let's do an example.

---

## Example

1. Given $f(x) = x^2 - x - 6$, find the slope of the tangent at $P(2, -4)$
    * Let $Q(2 + h, f(2 + h))$. 
    * Since $f(2 + h) = (2 + h)^2 - (2 + h) - 6$, and $m_P = \limit{h}{0} \frac{f(x + h) - f(x)}{h}$
    * $m_P = \limit{h}{0} \frac{f(2 + h) - f(2)}{h}$
    * $m_P = \limit{h}{0} \frac{(2 + h)^2 - (2 + h) - 6 - (-4)}{h}$

---

## Example, cont.

* $m_P = \limit{h}{0} \frac{(2 + h)^2 - (2 + h) - 6 - (-4)}{h}$
    * $m_P = \limit{h}{0} \frac{(4 + 4h + h^2) - (2 + h) - 6 + 4}{h}$
    * $m_P = \limit{h}{0} \frac{h^2 + 3h}{h}$
    * $m_P = 3$
* Find the slope of the tangent to the function $f(x) = x^2 - x - 12,\ x = 4$ (ex. for reader)

---

## Rational Example

2. Find the slope of the tangent to the function $f(x) = \frac{1}{x},\ x = 4$
    * Let $Q(4 + h, f(4 + h))$, $P(4, \frac{1}{4})$
    * $m_P = \limit{h}{0} \frac{f(4 + h) - f(4)}{h}$
    * $m_P = \limit{h}{0} \frac{\frac{1}{4 + h} - \frac{1}{4}}{h}$
    * $m_P = \limit{h}{0} \frac{\frac{4}{4(4 + h)} - \frac{4 + h}{4(4 + h)}}{h}$

---

## Example, cont.

* $m_P = \limit{h}{0} \frac{\frac{4}{4(4 + h)} - \frac{4 + h}{4(4 + h)}}{h}$
    * $m_P = \limit{h}{0} \frac{4 - (4 + h)}{4(4 + h)} / h$
    * $m_P = \limit{h}{0} \frac{h}{4h(4 + h)}$
    * $m_P = \limit{h}{0} \frac{1}{4(4 + h)}$
    * $m_P = \frac{1}{16}$

---

## Exercises for Readers

* Find the slope of the tangent to $f(x) = x^2 + 4$, at:
    * $x = 5$
    * $x = -3$
* Find the slope of the tangent to $f(x) = 3x - 4$, at:
    * $x = 2$
    * $x = 5$
* Find the slope of the tangent to $f(x) = \frac{x + 1}{x - 2}$, at $x = 5$
* Find the slope of the tangent to $f(x) = \frac{x - 5}{x}$, at $x = 3$
* Find the slope of the tangent to $f(x) = x^3 - 3$, at $x = 4$

---

# [Next Unit](../Differential/Derivatives/Lesson%201)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Find the slope of the tangent to the function $f(x) = x^2 - x - 12$ at $x = 4$
    * Let $P(4, f(4))$, $Q(4 + h, f(4 + h))$
    * $m_P = \limit{h}{0} \frac{f(4 + h) - f(4)}{h}$
    * $m_P = \limit{h}{0} \frac{(4 + h)^2 - (4 + h) - 12 - (4^2 - 4 - 12)}{h}$
    * $m_P = \limit{h}{0} \frac{(4 + h)^2 - (4 + h) - 12}{h}$

---

## Answers to Exercises, cont.

* Find the slope of the tangent to the function $f(x) = x^2 - x - 12$ at $x = 4$
    * $m_P = \limit{h}{0} \frac{(4 + h)^2 - (4 + h) - 12}{h}$
    * $m_P = \limit{h}{0} \frac{h^2 + 8h + 16 - 4 - h - 12}{h}$
    * $m_P = \limit{h}{0} \frac{h^2 + 7h}{h}$
    * $m_P = 7$ 
    * $m_P = 2x - 1$ *Hmm...*


---

## Answers to Exercises, cont.

* Find the slope of the tangent to $f(x) = x^2 + 4$ at $x = 5$
    * Let $P(5, f(5))$, $Q(5 + h, f(5 + h))$
    * $m_P = \limit{h}{0} \frac{f(5 + h) - f(5)}{h}$
    * $m_P = \limit{h}{0} \frac{(5 + h)^2 + 4 - (5^2 + 4)}{h}$
    * $m_P = \limit{h}{0} \frac{(5 + h)^2 + 4 - 29}{h}$
    * $m_P = \limit{h}{0} \frac{h^2 + 10h + 25 + 4 - 29}{h}$

---

## Answers to Exercises, cont.

* Find the slope of the tangent to $f(x) = x^2 + 4$ at $x = 5$
    * $m_P = \limit{h}{0} \frac{h^2 + 10h}{h}$
    * $m_P = 10$
    * $m_P = 2x$ *Hmm...*

---

## Answers to Exercises, cont.

* Find the slope of the tangent to $f(x) = x^2 + 4$ at $x = -3$
    * Let $P(-3, f(-3))$, $Q(-3 + h, f(-3 + h))$
    * $m_P = \limit{h}{0} \frac{f(-3 + h) - f(-3)}{h}$
    * $m_P = \limit{h}{0} \frac{(-3 + h)^2 + 4 - [(-3)^2 + 4]}{h}$
    * $m_P = \limit{h}{0} \frac{(-3 + h)^2 + 4 - 13}{h}$

---

## Answers to Exercises, cont.

* Find the slope of the tangent to $f(x) = x^2 + 4$ at $x = -3$
    * $m_P = \limit{h}{0} \frac{h^2 - 6h}{h}$
    * $m_P = -6$
    * $m_P = 2x$ *Hmm...*
* *Does it work for any other function?*

---

## Answers to Exercises, cont.

* Find the slope of the tangent to $f(x) = 3x - 4$, at:
    * $x = 2$
        * $m_P = 3$
    * $x = 5$
        * $m_P = 3$
* *It does!*

---

## Answers to Exercises, cont.

* Find the slope of the tangent to $f(x) = \frac{x + 1}{x - 2}$, at $x = 5$
    * Let $P(5, f(5))$, $Q(5 + h, f(5 + h))$
    * $m_P = \limit{h}{0} \frac{f(5 + h) - f(5)}{h}$
    * $m_P = \limit{h}{0} \frac{\frac{(5 + h) + 1}{(5 + h) - 2} - \frac{5 + 1}{5 - 2}}{h}$
    * $m_P = \limit{h}{0} \frac{\frac{6 + h}{3 + h} - \frac{6}{3}}{h}$

---

## Answers to Exercises, cont.

* Find the slope of the tangent to $f(x) = \frac{x + 1}{x - 2}$, at $x = 5$
    * $m_P = \limit{h}{0} \frac{\frac{6 + h}{3 + h} - \frac{6}{3}}{h}$
    * $m_P = \limit{h}{0} \frac{3(6 + h) - 6(3 + h)}{3(3 + h)} / h$
    * $m_P = \limit{h}{0} \frac{-3h}{3h(3 + h)}$
    * $m_P = -\frac{1}{3}$

---

## Answers to Exercises, cont.

* Find the slope of the tangent to $f(x) = \frac{x - 5}{x}$, at $x = 3$
    * Let $P(3, f(3))$, $Q(3 + h, f(3 + h))$
    * $m_P = \limit{h}{0} \frac{f(3 + h) - f(3)}{h}$
    * $m_P = \limit{h}{0} \frac{\frac{(3 + h) - 5}{3 + h} - \frac{3 - 5}{3}}{h}$
    * $m_P = \limit{h}{0} \frac{\frac{h - 2}{3 + h} - \frac{-2}{3}}{h}$

---

## Answers to Exercises, cont.

* Find the slope of the tangent to $f(x) = \frac{x - 5}{x}$, at $x = 3$
    * $m_P = \limit{h}{0} \frac{3(h - 2) + 2(3 + h)}{3h(3 + h)}$
    * $m_P = \limit{h}{0} \frac{3h + 2h}{3h(3 + h)}$
    * $m_P = \limit{h}{0} \frac{5h}{3h(3 + h)}$
    * $m_P = \frac{5}{9}$


---

## Answers to Exercises, cont.

* Find the slope of the tangent to $f(x) = x^3 - 3$, at $x = 4$
    * $m_P = 48 = 3x^2$?
    * Let $P(4, f(4))$, $Q(4 + h, f(4 + h))$
    * $m_P = \limit{h}{0} \frac{f(4 + h) - f(4)}{h}$
    * $m_P = \limit{h}{0} \frac{(4 + h)^3 - 3 - (4^3 - 3)}{h}$
    * $m_P = \limit{h}{0} \frac{(4 + h)^3 - 3 - 61}{h}$
    
---

## Answers to Exercises, cont.

* Find the slope of the tangent to $f(x) = x^3 - 3$, at $x = 4$
    * $m_P = 48 = 3x^2$?
    * $m_P = \limit{h}{0} \frac{(4 + h)^3 - 64}{h}$
    * $m_P = \limit{h}{0} \frac{h^3 + 12h^2 + 48h}{h}$
    * $m_P = \limit{h}{0} h^2 + 12h + 48$
    * $m_P = 48$

---

# [Next Unit](../Differential/Derivatives/Lesson%201)