---
marp: true
theme: uncover
class: invert
paginate: true
math: mathjax
---

$\newcommand{\cL}{\mathcal{cL}}$
$\newcommand{\cLn}[1][]{\mathcal{cL}(#1)}$
$\newcommand{\sid}[1]{\overline{#1}}$

# <!--fit--> Pre-Calculus 11 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2023-->

$\newcommand{\cA}{\mathcal{cA}}$
$\newcommand{\cAn}[1][]{\mathcal{cA}(#1)}$
$\newcommand{\ang}[1]{\angle #1}$

---

$\newcommand{\opT}[1][]{\mathcal{T}(#1)}$
$\newcommand{\opS}[1][]{\mathcal{S}(#1)}$
$\newcommand{\opC}[1][]{\mathcal{C}(#1)}$

## Lesson 3: Cosine Law

$\newcommand{\ioT}[1][]{\mathcal{T}^{-1}(#1)}$
$\newcommand{\ioS}[1][]{\mathcal{S}^{-1}(#1)}$
$\newcommand{\ioC}[1][]{\mathcal{C}^{-1}(#1)}$

---

## What is Cosine Law?

Similar to the triangle used for Sine Law (see lesson 2), The Cosine Law uses the same triangle, with a bit of a different formula.
With Cosine Law, you can have all three sides & find an angle **OR** have two sides and one angle, but no complete pair.
Formula:
$a^2=b^2+c^2-2bc\ \opC[A]$

---

## Notes & Notation

* $x^2=y^2+z^2-2yz\opC[\theta]$
    * For some sides & angle $x,y,z,\theta$.
* Notation
    * $\cLn$ for side, $\cAn$ for angle.
        * $\cL$: Cosine Length Determinant (Cosine Law)
        * $\cA$: Cosine Angle Determinant (Cosine Law)

---

## Example 1: Side ($\cL$)

* Determine the length of $\sid{BC}$.
1) Define Variables:
    * let $\ang{A}=48,\sid{AC}=9,\sid{AB}=5,\sid{BC}=x$
2) $\cLn[x]=x^2=9^2+5^2-2(9\times5)\opC[48]$
    * $9^2+5^2=106, 2(9\times5)=90$
3) $\cLn[x]=106-90\opC[48]$
    * $\opC[48]=0.669,90\times\opC[48]=60.221$
4) $\cLn[x]=106-60.221$
    * $106-60.221=45.778$

---

## Example 1, cont.

5) $\cLn[x]=45.778$
    * Square root both sides.
6) $\cLn[x]=6.77$

---

## Example 2: Angle ($\cA$)

* Determine the measure of $\ang{W}$.
1) Define Variables
    * let $\sid{WX}=23,\ \sid{XY}=18,\ \sid{WY}=25,\ \ang{W}=\theta$
2) $\cAn[\theta]=[18^2-(25^2+23^2)]-2(25\times23)\opC[\theta]$
    * $25^2+23^2=1154,\ 2(25\times23)=1150,\ 18^2=324$
3) $\cAn[\theta]=[324-1154]-1150\opC[\theta]$
    * $324-1154=-830,\ -830/-1150=\frac{83}{115}$
4) $\cAn[\theta]=\opC[\theta]=\frac{83}{115}$
    * Inverse Cosine both sides.


---

## Example 2, cont.

5) $\cAn[\theta]=\ioC[\frac{83}{115}]$
    * $\ioC[\frac{83}{115}]=43.8^\circ$
6) $\cAn[\theta]=43.8^\circ$

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%204%20(Angles%20and%20Special%20Triangles).html) 

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">