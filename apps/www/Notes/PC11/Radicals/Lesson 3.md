---
marp: true
theme: uncover
class: invert
paginate: true
math: mathjax
---

$\renewcommand{\nrt}[2][]{\sqrt[#1]{#2}}$
$\def\setC{\mathbb{C}}$
$\newcommand{\%}[2][]{#1\mod#2}$

# <!--fit--> Pre-Calculus 11 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2023-->

$\newcommand{\curt}[1]{\sqrt[3]{#1}}$
$\newcommand{\qurt}[1]{\sqrt[4]{#1}}$
$\newcommand{\quad}[3]{\frac{-#2\pm\sqrt{(#2)^2-4(#1)(#2)}}{2(#1)}}$

---

## Lesson 3: Radical Equations

---

## Restrictions

* $\nrt[n]{x} \iff \%[n]{2}=0$
* If $n$ is an even number, we need to state restrictions (like NPVs) on the variable since you cannot have a negative number under a root w/ an even index.
    * $\nrt[n]{-x}, x\in\setC\iff\%[n]{2}=0$
* To get the restrictions, take radicand and solve for variable. (if /-, restrictions flip.)

---

## Example: Solving Restrictions

* $3x+1\geq0$
    * $3x\geq-1$
    * $x\geq-\frac{1}{3}$

---

## Example: Solving an Equation

1) $3+\sqrt{3x+1}=13$
    * State Restrictions: $x\geq-\frac{1}{3}$
2) $\sqrt{3x+1}=10$
    * Remove radical
3) $3x+1=100$
    * Solve for x.
4) $3x=99, x=33$
    * Check answer isn't extraneous
5) $33\geq-\frac{1}{3}$

---

## Example

1) $m-\sqrt{2m+3}=6$
    * State restrictions: $m\geq-\frac{3}{2}$ Flip sides.
2) $m-6=\sqrt{2m+3}$
    * Clear radical
3) $m^2-12m+36=2m+3$
4) $m^2-14m+33=0$
    * Factor
5) $(m-11)(m-3)=0, m=11,3$
    * Verify
6) $m=11, 3(ER)$

---

## Example: Multiple Radicals

1) $\sqrt{3+x}+\sqrt{2x-1}=5$
    * State restrictions: $x\geq-3,\frac{1}{2}$
2) $\sqrt{3+x}=5-\sqrt{2x-1}$
    * Clear Radicals (Only remove one at a time)
3) $3+x=24-10\sqrt{2x-1}+2x$
4) $100(2x+1)=(21+x)^2$
5) $200x+100=x^2+42x+441$
6) $x^2-158x+541=0$

---

## Multiple Radicals, cont.

7) $x=\quad{1}{-158}{541}$
8) $x=\frac{158\pm\sqrt{24964-2164}}{2}$
9) $x=\frac{158\pm\sqrt{22800}}{2}$
10) $x=\frac{158+150.997}{2},\frac{158-150.997}{2}$
11) $x=154.5 (30.1\neq5\text{ER}),3.5$

---

# [Next Unit <i class="fa-solid fa-diagram-next"></i>](../Trigonometry/Lesson%201%20(Grade%2010%20Review).html)

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">