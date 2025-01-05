---
marp: true
theme: uncover
class: invert
paginate: true
math: mathjax
---

$\newcommand{\ipB}{\frac{b}{\opS[B]}}$
$\newcommand{\ipC}{\frac{c}{\opS[C]}}$
$\newcommand{\sL}{\mathcal{sL}}$
$\newcommand{\sid}[1]{\overline{#1}}$

# <!--fit--> Pre-Calculus 11 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2023-->

$\newcommand{\deg}{^\circ}$
$\newcommand{\ipA}{\frac{a}{\opS[A]}}$
$\newcommand{\sA}{\mathcal{sA}}$
$\newcommand{\ang}[1]{\angle #1}$

---

$\newcommand{\opT}[1][]{\mathcal{T}(#1)}$
$\newcommand{\opS}[1][]{\mathcal{S}(#1)}$
$\newcommand{\ioS}[1][]{\mathcal{S}^{-1}(#1)}$
$\newcommand{\opC}[1][]{\mathcal{C}(#1)}$
$\newcommand{\sLN}[1][N]{\mathcal{sL}(#1)}$

## Lesson 2: Sine Law

$\newcommand{\pA}{\frac{\opS[A]}{a}}$
$\newcommand{\pB}{\frac{\opS[B]}{b}}$
$\newcommand{\pC}{\frac{\opS[C]}{c}}$
$\newcommand{\sAN}[1][N]{\mathcal{sA}(#1)}$
$\newcommand{\ref}{\theta_R}$

---

$\newcommand{\ipN}[2]{\frac{#1}{\opS[#2]}}$

## What is Sine Law?

Up until this point when we have used the primary trig ratios ($\opS,\opC,\opT$), it has only been with right triangles ($\angle A=90\deg$). However, Trigonometry is not limited to only Right Triangles.
### The Sine Law
* $\pA=\pB=\pC$ / $\ipA=\ipB=\ipC$

$\newcommand{\pN}[2]{\frac{\opS[#1]}{#2}}$

---

## Notes / Notation:

* $\pA=\pB=\pC$
    * Find an angle.
* $\ipA=\ipB=\ipC$
    * Find a side.
* Only use two proportions when solving
* **Must** be one full proportion
* Notation: $\sLN$ for side, $\sAN$ for angle.
    * $\sL$: Sine Length Determinant (Sine Law)
    * $\sA$: Sine Angle Determinant (Sine Law)

---

## Example 1: Side ($\sL$)

* Determine the length of $\sid{AB}$.
1) Define variables.
    * $\sid{AB}=c,\ang{A}=48\deg,\sid{AC}=14=b,\ang{C}=29$
        * We can determine that $\ang{B}=103$
    * We now have a full proportion.
2) $\sLN[c]=\ipC=\ipB$
    * $\sLN[c]=\ipN{c}{29}=\ipN{14}{103}$
3) $\times\opS[29]$ both sides.
    * $\sLN[c]=c=\ipN{14\opS[29]}{103}$

---

## Example 1, cont.

4) Solve
    * $\sLN[c]=\ipN{14\opS[29]}{103}$
        * $14\opS[29]=6.787,\opS[103]=0.974$
    * $\sLN[c]=\frac{6.787}{0.974}$
    * $\sLN[c]=6.97$

---

## Example 2: Angle ($\sA$)

* Determine $\theta$
1) Define variables.
    * $\sid{WX}=23=y,\ang{W}=\theta,\sid{XY}=18=w,\ang{Y}=72\deg$
    * We have a full proportion.
2) $\sAN[\theta]=\pN{72}{23}=\pN{\theta}{18}$
3) $\times18$ both sides.
    * $\sAN[\theta]=18\pN{72}{23}$

---

## Example 2, cont.
4) Solve.
    * $\sAN[\theta]=\ioS[0.744]$
    * $\sAN[\theta]=48.1\deg$

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%203%20(Cosine%20Law).html) 

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">