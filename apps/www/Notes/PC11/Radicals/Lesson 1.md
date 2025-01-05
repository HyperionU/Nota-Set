---
marp: true
theme: uncover
class: invert
paginate: true
math: mathjax
---

$\newcommand{\and}[2]{#1 \land #2}$
$\newcommand{\setN}{\mathbb{N}}$
$\renewcommand{\nrt}[2][]{\sqrt[#1]{#2}}$

# <!--fit--> Pre-Calculus 11 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2023-->

$\newcommand{\setR}{\mathbb{R}}$
$\newcommand{\curt}[1]{\sqrt[3]{#1}}$
$\newcommand{\qurt}[1]{\sqrt[4]{#1}}$

---

## Lesson 1: Working with Radicals

---

## What is a Radical?

* Radicals ($\sqrt{}$) can be treated very much like fractions. They can be simplified into lower terms, and this is how we **ALWAYS** want to present our answers.
* Example Radical: $\sqrt[n]{x}=y$
    * $n$: Index ($y^n=x$, number of times $y$ is multiplied by itself to get $x$)
    * $x$: Radicand (value when $y$ is multiplied by itself $n$ times)
    * $\sqrt[n]{x}$: Radical (The full expression)

---

## Key Property: Radical Multiplication

* $\sqrt[n]{ab}=\sqrt[n]{a}\times\sqrt[n]{b}\iff\and{n\in\setN}{a,b\in\setR}$
* $\sqrt[n]{ab}=\sqrt[n]{a}\times\sqrt[n]{b}$ if $n$ is a natural number, and $a$ & $b$ are real numbers.

---

## Converting Entire to Mixed

* Example: $\sqrt{45}$
    * $x\times y=45, \sqrt{x}\in\setN$
    * *What are 45's factors, one of which is a perfect square?*
        * *$9\times 5$? That works.*
    * $\sqrt{9\times 5}=\sqrt{9}\sqrt{5}$
    * $\sqrt{9}=3 \therefore\sqrt{45}=3\sqrt{5}$ 
* This even works for higher indices.

---

## Example: Entire to Mixed

* $\curt{192}$
    * $\curt{64\times 3}$
    * $\curt{64}\curt{3}$
    * $\curt{64}=4\therefore\curt{192}=4\curt{3}$

---

## Examples: Entire $\rightarrow$ Mixed

* Simplify $\sqrt{n^5}$
    * *How many groups of $n^2$'s are there?*
    * $\sqrt{n^4\times n}$
    * $\sqrt{n^4}\sqrt{n}$
    * $\sqrt{n^4}=n^2\therefore\sqrt{n^5}=n^2(\sqrt{n})$
* Simplify $\curt{x^{11}}$
    * *How many groups of $n^3$'s are there?*
    * $\curt{x^9}\curt{x^2}$
    * $\curt{x^9}=x^3\therefore\curt{x^{11}}=x^3(\curt{x^2})$

---

## Converting Mixed $\rightarrow$ Entire

* Example: $6\sqrt{3}$
    * $\sqrt{6^2\times3}$
    * $\sqrt{36\times3}$
    * $\sqrt{108}$
* Also works for higher indices.
* Example: $4\qurt{5}$
    * $\qurt{4^4\times5}$
    * $\qurt{256\times5}$
    * $\qurt{1280}$

---

## Examples: Mixed $\rightarrow$ Entire

* $y^3\sqrt{y}$
    * $\sqrt{(y^3)^2\times y}$
    * $\sqrt{y^6\times y}$
    * $\sqrt{y^7}$
* $3x^4\curt{x^2}$
    * $\curt{(3x^4)^3\times x^2}$
    * $\curt{27x^12\times x^2}$
    * $\curt{27x^{14}}$

---

## Adding / Subtracting Radicals

* Summary: **Combine Like Terms!**
    * $\sqrt{3}=3\sqrt{3}$
* Whenever we add radicals, we need a common denominator. We need to convert into mixed radicals with the same radicand, then add / subtract the whole numbers out front.

---

## Examples: Adding / Subtracting

* $4\sqrt{3}+7\sqrt{3}$
    * $(4+7)\sqrt{3}$
    * $11\sqrt{3}$
* $\sqrt{24}+\sqrt{6}$
    * $2\sqrt{6}+\sqrt{6}$
    * $3\sqrt{6}$
* $-\sqrt{27}+3\sqrt{5}-\sqrt{80}-2\sqrt{12}$
    * $-3\sqrt{3}+3\sqrt{5}-4\sqrt{5}-4\sqrt{3}$
    * $(-3\sqrt{3}-4\sqrt{3})+(3\sqrt{5}-4\sqrt{5})$
    * $-7\sqrt{3}-\sqrt{5}$

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%202%20(Multiplying%20+%20Dividing).html) 

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">