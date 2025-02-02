---
marp: true
theme: uncover
class: invert
math: mathjax
---

# <!--fit--> Pre-Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2024-->

---
<!--paginate: true-->

# Lesson 3: Stretches

---

## Vertical Stretch

* A transformation that changes the distance of the point from the x-axis ($y = 0$). This **does** change the shape of the graph.
* $a$ Scale Factor: the value $y$ is multiplied by to change the distance.
    * Case I: $a \in (0,1)$, compresses the values.
    * Case II: $a > 1$, stretches the values.
    * Case III: $a = 1$, no stretch.

---

## On $a > 0$
* This means a vertical stretch by a factor of $a$.

$y = f(x) \mapsto y = af(x)$ or $\frac{y}{a} = f(x)$

---

## Example:

For the graph $y = f(x)$, sketch $y = 2f(x)$ and $2y = f(x)$.

Values:
| = | $(x,y)$ | $(x,2y)$ | $(x,y/2)$ |
|---|---------|----------|-----------|
| A |$(-6,4)$ | $(-6,8)$ |  $(-6,2)$ |
| B |$(-2,0)$ | $(-2,0)$ |  $(-2,0)$ |
| C | $(0,2)$ |  $(0,4)$ |  $(0,1)$  |
| D | $(2,0)$ |  $(2,0)$ |  $(2,0)$  |
| E | $(6,4)$ |  $(6,8)$ |  $(6,2)$  |

---

## Invariant Points

* Like reflections, stretches have Invariant Points as well.
* For Vertical Stretches, $\forall (x,y), y = 0$ are invariant.
* In the previous Example, B and D are invariant.

---

## Horizontal Stretch

* A transformation that changes the distance of the point from the y-axis ($x = 0$). This **does** change the shape of the graph.
* $b$ Scale Factor: the value $y$ is multiplied by to change the distance.
    * Case I: $b \in (0,1)$, stretches the values.
    * Case II: $b > 1$, compresses the values.
    * Case III: $b = 1$, no stretch.
* *So it's opposite of $a$?* Yes!

---

## On $b > 0$
* This means a vertical stretch by a factor of $\frac{1}{b}$.

$y = f(x) \mapsto y = f(bx)$

---

## Example:

For the graph $y = f(x)$, sketch $y = f(2x)$ and $y = f(\frac{x}{2})$.

Values:
| = | $(x,y)$ | $(x/2,y)$ | $(2x,y)$ |
|---|---------|-----------|----------|
| A |$(-4,3)$ | $(-2,3)$  | $(-8,3)$ |
| B |$(-2,1)$ | $(-1,1)$  | $(-4,1)$ |
| C | $(2,2)$ |  $(1,2)$  | $(4,2)$  |
| D | $(4,-2)$|  $(2,-2)$ | $(8,-2)$ |

---

## Invariant Points

* For Horizontal Stretches, $\forall (x,y), x = 0$ are invariant.
* In the previous Example, the y-intercept is Invariant.

---

## Notes on Shorthand:

* $HS(n)$: Horizontal Stretch
* $VS(n)$: Vertical Stretch
* $HR$ and $VR$: Reflections
* $\leftarrow n$ and $\rightarrow n$: Horizontal Translation
* $\uparrow n$ and $\downarrow n$: Vertical Translation

---

## Mapping Notation:

* Determine the Mapping Notation of $y = f(x)$ for these cases:
    * $HS(3),VS(\frac{1}{4})$
    * $y = f(x) \mapsto 3y = f(5x)$
    * General form?

---

## Answers:

* $(x,y) \mapsto (x/3, \frac{y}{4})$
* $(x,y) \mapsto (\frac{x}{5}, \frac{y}{3})$
* $(x,y) \mapsto (\frac{x}{b},ay)$

---

## Going Backwards

* Determine an equation for $y = g(x)$ in terms of $y = f(x)$ (form: $f(x) \mapsto g(x)$)
1. $(-4,3) \mapsto (-4,1)$, $(2,0)$ is Invariant.
2. $f(x) = x^3$, $(1,1) \mapsto (3,1)$

---

# Answers:

1. $g(x) = \frac{1}{3} f(x)$
2. $g(x) = f(\frac{x}{3}) \therefore g(x) = (\frac{x}{3})^3$

---

# Challenge:

What would the following functions look like if they have been $HS(3), VS(\frac{1}{2})$?
* $y = f(x)$
* $y = \sqrt{x}$
* $y = \log x$

---

## Answers:

* $y = \frac{1}{2} f(\frac{x}{3})$
* $\frac{y}{2} = \sqrt{\frac{x}{3}}$
* $\frac{y}{2} = \log(\frac{x}{3})$

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%204%20(Composition%20of%20Transformations).html) 

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">