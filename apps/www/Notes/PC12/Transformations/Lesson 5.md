---
marp: true
theme: uncover
class: invert
math: mathjax
---

$\def\itr{\mathfrak{T}_\mathcal{I}}$

# <!--fit--> Pre-Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2024-->

$\newcommand\inv[1]{f^{-1}(#1)}$

---
<!--paginate: true-->

# Lesson 5: Inverse of A Relation

---

## The Inverse

To **Inverse** is to undo or reverse a position, order or effect.
* A Transformation $\itr (f(x)) := (x,y) \mapsto (y,x)$
* Graph is the reflection along the line $y = x$
* Domain: Range of $\itr$, Range: Domain of $\itr$
* If $\itr$ is also a function, we can use the notation $\inv{x}\ \text{or } f(y) = x$

---

## Graphing an inverse

| $(x,y)$ | $(y,x)$ |
|---------|---------|
|$(-6,4)$ |$(4,-6)$ |
|$(-4,6)$ |$(6,-4)$ |
| $(0,6)$ | $(6,0)$ |
| $(2,2)$ | $(2,2)$ |
| $(4,2)$ | $(2,4)$ |
| $(6,0)$ | $(0,6)$ |

---

## Invariant Points

* Like other transformations, the Inverse may have Invariant points.
* Any point $P(x,y) \text{ s.t. } y = x$ are Invariant.
* In the previous example: $(2,2)$ is invariant.

---

## Domain and Range

* For the previous example:
    * Domain of $f$: $[-6, 6]$
    * Range of $f$: $[0, 6]$
* The inverse flips the points.
    * Domain of $y$: $[0, 6]$
    * Range of $x$: $[-6, 6]$

---

## The Important Thing

* In the previous example, was the inverse a function? 
    * *No!* The inverse fails the VLT.
* In order to be a function: if a vertical line passes through two values *at any point* on a curve, it is not a function.
    * This is the Vertical Line Test.
* Likewise, if a horizontal line passes through two values *at any point* on a function, the inverse is not a function.
    * This is the Horizontal Line Test.

---

## Restrictions

For example, take $y = (x - 3)^2$, and graph its inverse.
* Is it a function? 
    * *No!* The original failed the HLT.
* We need to restrict the domain so that the inverse is a function.
* There's really one main choice: $x \leq n$ or $x \geq n$, $n \geq 3$
* *hmm... this looks familiar.* 

---

## Determining Equations

1. $y = 3x + 6$
2. $y = x^2 - 4$
3. $y = (x-2)^3$
4. $y = \frac{3 + 2x}{x - 1}$

---

## Answers:

1. $\inv{x} = \frac{x}{3} - 2$
2. $\inv{x} = \pm\sqrt{x + 4}$
3. $\inv{x} = 2 + \sqrt[3]{x}$
4. $\inv{x} = \frac{x + 3}{x - 2}$

---

# [Next Unit <i class="fa-solid fa-diagram-next"></i>](../Polynomials/Lesson%201%20(Division).html)

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">