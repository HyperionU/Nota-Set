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

$\newcommand{\opT}[1][\theta]{\mathcal{T}(#1)}$
$\newcommand{\opS}[1][\theta]{\mathcal{S}(#1)}$
$\newcommand{\opC}[1][\theta]{\mathcal{C}(#1)}$
$\newcommand{\ref}{\theta_\mathcal{R}}$

## Lesson 5: Trigonometric Ratios

$\newcommand{\qI}{\mathbb{Q}_\mathfrak{I}}$
$\newcommand{\qII}{\mathbb{Q}_\mathfrak{II}}$
$\newcommand{\qIII}{\mathbb{Q}_\mathfrak{III}}$
$\newcommand{\qIV}{\mathbb{Q}_\mathfrak{IV}}$

---

$\newcommand{\rt}{\sqrt{3}}$
$\newcommand{\setR}{\mathbb{R}}$
$\newcommand{\term}{t(x)}$
## Note:

* All angles are in standard position.
* $r$ (diagonal Distance) $\in\setR^+$
$\newcommand{\sR}[1][\theta]{\opS[#1]=\frac{y}{r}}$
$\newcommand{\cR}[1][\theta]{\opC[#1]=\frac{x}{r}}$
$\newcommand{\tR}[1][\theta]{\opT[#1]=\frac{y}{x}}$

---

## Finding Exact Distance

Using Trig Ratios, we can find the exact distance a point is from the origin and the **exact** ratios for the angle.

Suppose we have an angle with a point $P(x,y)$ somewhere on the terminal arm. Each coordinate represents the horizontal ($x$) and vertical ($y$) distance, combining to result in a diagonal ($r$) distance.

---

## Determining $r$

We can use Pythagoras to solve for the value of $r$ as long as $P$ is on the terminal arm. ($P\in t(x), t(x)$ is terminal arm.)

* Our distance: $r=\sqrt{x^2+y^2}$

---

## Determining Exact Ratios

Assume we had a point $W(-5,-12)$ that is on the terminal arm. What are the exact Ratios?

1) Find $r$
    * $r=\sqrt{5^2+12^2}$
    * $r=\sqrt{169}$
    * $r=13$

---

## Determining Exact Ratios, cont.

2) Determine Ratios
    * Sine
        * $\opS=\frac{-12}{13}$
    * Cosine
        * $\opC=\frac{-5}{13}$
    * Tangent
        * $\opT=\frac{12}{5}$
    
---

## Positivity Rule: CAST

The CAST Law is a rule which states which ratios are positive in each quadrant

<table>
    <tr>
        <th></th>
        <th>C: Q(IV)</th>
        <th>A: Q(I)</th>
        <th>S: Q(II)</th>
        <th>T: Q(III)</th>
    </tr>
    <tr>
        <th>sin(x)</th>
        <th>-</th>
        <th>+</th>
        <th>+</th>
        <th>-</th>
    </tr>
    <tr>
        <th>cos(x)</th>
        <th>+</th>
        <th>+</th>
        <th>-</th>
        <th>-</th>
    </tr>
    <tr>
        <th>tan(x)</th>
        <th>-</th>
        <th>+</th>
        <th>-</th>
        <th>+</th>
    </tr>
</table>

---

## Example 1: Exact Values

Determine the exact value of $\opS[240\deg]$

1) Define Variables
    * let $\theta=240\deg,\ref=60\deg$
        * *why look at $\ref$?* It's our key to finding the answer.
    * let $x=1,y=\rt,\  \therefore r=2$
2) Determine value
    * $\opS[240]=\frac{-\rt}{2}$

---

## Example 2: Completing the Set

Assume $\theta$ is an angle with a terminal arm ($t(x)\in\qIII$) and $\opS[\theta]=\frac{-4}{5}$. Determine exact values of $\opC[\theta]\land\opT[\theta]$.

1) Define variables:
    * let $P(x,y),\opS[\theta]=\frac{-4}{5}$
    * Since $\sR,\ \therefore y=-4,r=5$
    * Using Pythagoras, we can state $x=-3$
---

## Example 2, cont.

2) Complete the Set
    * Cosine
        * $\opC[\theta]=\frac{x}{5}$
        * $\opC[\theta]=\frac{-3}{5}$
    * Tangent
        * $\opT[\theta]=\frac{-4}{x}$
        * $\opT[\theta]=\frac{4}{3}$

---

## Example 3: Range Condition

Solve $\opS=-\frac{1}{\sqrt{2}},\range{\theta}=\{\qI,\qII,\qIII,\qIV|[0\deg,360\deg]\}$
1) Cut the boundary.
    * Since $r\in\setR^+,\ \therefore y\in\setR^-$.
    * This means that the answer must be in $\qIII,\qIV$.
2) Determine $\ref$
    * Since there is a $\sqrt{2},\ \therefore\ref=45\deg$

---

## Example 3, cont.
3) Determine $\theta$
    * Use Reference Formulae
* $\theta=\{225\deg,315\deg|\theta\in\{\qIII,\qIV\}\}$

---

# [Finish <i class="fa-solid fa-flag-checkered"></i>](https://hyperionu.github.io/Nota-Set)

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">