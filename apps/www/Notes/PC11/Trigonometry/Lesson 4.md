---
marp: true
theme: uncover
class: invert
paginate: true
math: mathjax
---

$\newcommand{\deg}{^\circ}$

# <!--fit--> Pre-Calculus 11 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2023-->

$\newcommand{\range}[1]{\mathcal{R}(#1)}$

---

$\newcommand{\opT}[1][]{\mathcal{T}(#1)}$
$\newcommand{\opS}[1][]{\mathcal{S}(#1)}$
$\newcommand{\opC}[1][]{\mathcal{C}(#1)}$
$\newcommand{\ref}{\theta_\mathcal{R}}$

## Lesson 4: Angles & Special Triangles

$\newcommand{\qI}{\mathbb{Q}_\mathfrak{I}}$
$\newcommand{\qII}{\mathbb{Q}_\mathfrak{II}}$
$\newcommand{\qIII}{\mathbb{Q}_\mathfrak{III}}$
$\newcommand{\qIV}{\mathbb{Q}_\mathfrak{IV}}$

---

$\newcommand{\half}{\frac{1}{2}}$
$\newcommand{\rt}{\sqrt{3}}$

## 4.1: Angles in Standard Position

$\newcommand{\rth}{\frac{\sqrt{3}}{2}}$
$\newcommand{\irt}{\frac{1}{\sqrt{3}}}$

---

## Angles in Standard Position

When dealing with angles, special cases emerge. To investigate, we need to use a Cartesian Plane ($x,y$ graph).

---

## Terminology:

* Initial Arm
    * Start position; always lays along the $+x$-axis
* Terminal Arm
    * Final position; location after rotation around the origin.
* Angle in Standard Position
    * Initial arm **must** be positive
    * Origin is vertex. $(0,0)$
    * Measured between initial & terminal arms
    * Always positive when drawn anti-clockwise

---

## Angular Range

Since any angle in standard position must always be positive, we know the range of possible answers per quadrant.

* $\range\qI=(0\deg,90\deg)$
* $\range\qII=(90\deg,180\deg)$
* $\range\qIII=(180\deg,270\deg)$
* $\range\qIV=(270\deg,360\deg/0\deg)$

---

## Reference Angle: $\ref$

* An acute angle ($\lt90\deg$)
* Vertex is origin $(0,0)$
* Formed between terminal arm & $x$-axis
* Identified by $\ref$

---

## Reference Angle Formulae

1) $\theta=\ref, \theta\in\qI$
2) $\ref=180\deg-\theta, \theta\in\qII$
3) $\ref=\theta-180\deg,\theta\in\qIII$
4) $\ref=360\deg-\theta, \theta\in\qIV$

Based on the quadrant, the formula changes. It's a challenge when you have a reference angle (i.e. $\ref=20\deg$), you can actually have 4 different angles that satisfy the reference angle: $\theta=\{20\deg,160\deg,200\deg,340\deg|\ref=20\deg\}$, 

---

## 4.2: Special Triangles

---

## Special Right Triangles

Certan angles we encounter allow us to determine the **exact** value of Trigonometric ratios.
These triangles have angles: $\theta=\{30\deg,45\deg,60\deg|\angle A+\angle B+\angle C=180\deg\}$
Let's look at specific cases.

---

## 45-45-90 Triangle, defined

If there is a right triangle with an angle of $45\deg$, the other (non-right) angle is also $45\deg$.
If the side lengths of the legs equal $1$ unit, the hypotenuse will be equal to $\sqrt{2}$.

---

## 45-45-90 Triangle, part 2

![](https://dcvp84mxptlac.cloudfront.net/diagrams2/MATH10-11-2-X-A4.png)

---

## Ratios: 45-45-90

Using this special triangle, we can determine **exact** trigonometric ratios for each case:

* Sine
    * $\opS[45\deg]=\frac{1}{\sqrt{2}}$
* Cosine
    * $\opC[45\deg]=\opS[45\deg]$
* Tangent
    * $\opT[45\deg]=\frac{1}{1}=1$

---

## Application 1: Exact Values

* Find **exact** values for $x,y$
    * $\ell=4,\theta=45\deg, x=h, y=O$
* Since $\ell=4,\ \therefore\ y=4$
    * We can define $\opC[45\deg]=\frac{4}{x}$
* We have a proportion: $\frac{1}{\sqrt{2}}=\frac{4}{x}$
    * By cross multiplying & dividing:
* $x=4\sqrt{2}$

---

## 30-60-90 Triangle, defined

If we draw a triangle with an angle of $30\deg$, the other (non-right) angle must be $60\deg$. This triangle is half of an equilateral triangle with side length $2$.
If we use Pythagoras to find the height, we get an exact value of $\sqrt{3}$, which is always opposite the $60\deg$ angle.

---

## 30-60-90 Triangle, part 2

![w:600](https://www.varsitytutors.com/assets/vt-hotmath-legacy/hotmath_help/topics/30-60-90-triangles/triangle1.gif)

---

## Ratios: 30-60-90

* Sine
    * $\opS[30\deg]=\half,\opS[60\deg]=\rth$
* Cosine
    * $\opC[30\deg]=\rth,\opC[60\deg]=\half$
* Tangent
    * $\opT[30\deg]=\irt,\opT[60\deg]=\rt$

---

## Applications 2: Exact Values

* Find **exact** values for $x,y$
    * $z=8,\theta_1=30\deg,\theta_2=60\deg$
* $\opS[60]=\frac{8}{x}$ / $\opT[60]=\frac{8}{y}$
    * Each can be rewritten as proportions:
* $\rth=\frac{8}{x}$ / $\frac{\rt}{1}=\frac{8}{y}$
    * Cross multiplying & dividing gives $x,y$
* $x=\frac{16}{\rt},y=\frac{8}{\rt}$

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%205%20(Trigonometric%20Ratios).html) 

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">