---
marp: true
theme: uncover
class: invert
paginate: true
math: mathjax
---

# <!--fit--> Pre-Calculus 11 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2023-->

---

## Lesson 4: Solving Quadratics - Formula

---

## Terms

* Nature of the Roots: Number of solutions.
* Discriminant ($\Delta$): $\Delta=b^2-4ac$
* Exact answer: an answer w/o a decimal
* Approximate answer: an answer w/ a decimal

---

## Why Quadratic Formula?

* Sometimes, there are equations that are too difficult to solve by factoring or graphing.
* When this occurs, it is best to use the formula:
## $x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}$ 
* All thats needed is a quadratic equation in standard form.

---

## Example: Comparing Factoring and Quadratic Formula

$f(x)=x^2+3x-10$

* Factoring
    * $(x+5)(x-2)$
    * $x=\{-5,2\}$

---

## Example, cont.

$f(x)=x^2+3x-10$

* Quadratic Formula
    * $x=\frac{-3\pm\sqrt{3^2-4(-10)}}{2}$
    * $x=\frac{-3\pm\sqrt{9+40}}{2}$
    * $x=\frac{-3\pm\sqrt{49}}{2}$
    * $x=\frac{-3\pm7}{2}$
    * $x=\{-5,2\}$

---

## Note:

1) We get the same answer whether we factor or use the formula.
2) Using the formula takes longer than factoring.
    * This is because the formula was intended for the equations where factoring by hand is near-impossible.
It is just another tool in our toolkit to solve quadratic equations.

---

## Example 2
* Find the **exact** zeros of $2m^2-7=-4m$
    * $2m^2+4m-7=0$
    * $m=\frac{-4\pm\sqrt{4^2-4(2*7)}}{2(2)}$
    * $m=\frac{-4\pm\sqrt{16+56}}{4}$
    * $m=\frac{-4\pm\sqrt{72}}{4}$
    * $m=\frac{-4\pm6\sqrt{2}}{4}$
    * $m=\frac{-2\pm6\sqrt{2}}{2}$

---

## Example 3
* Find the x-intercepts of $6x^2-7x-20$
    * $x=\frac{-(-7)\pm\sqrt{6^2-4(6*-20)}}{2(6)}$
    * $x=\frac{7\pm\sqrt{36+480}}{12}$
    * $x=\frac{7\pm\sqrt{529}}{12}$
    * $x=\frac{7\pm23}{12}$
    * $x=\{\frac{30}{12},\frac{-16}{12}\}$ 
    * $x=\{\frac{5}{2},\frac{-4}{3}\}$

---

## Exceptions: 0 Real Roots
* Sometimes, the formula doesn't always "keep it real".
* Example: Solve $3x^2-4x+2=0$
    * $x=\frac{-(-4)\pm\sqrt{(-4)^2-4(3*2)}}{2(3)}$
    * $x=\frac{4\pm\sqrt{16-24}}{6}$
    * $x=\frac{4\pm\sqrt{-8}}{6}$
        * $\sqrt{-8}\in\mathbb{C}$
* This means that there are no real roots.

---

## Exceptions: 1 Distinct Real Root
* Or it has a matching root.
* Example: Solve $x^2-4x+4=0$
    * $x=\frac{-(-4)\pm\sqrt{(-4)^2-4(4)}}{2}$
    * $x=\frac{4\pm\sqrt{16-16}}{2}$
    * $x=\frac{4\pm\sqrt{0}}{2}$
    * $x=\frac{4}{2}$
    * $x=2$
* This means there is one real root.

---

## Discriminant and Nature of The Roots

* The expression $b^2-4ac$ (under the radical sign) is the **Discriminant** ($\Delta$).
* This allows us to determine the **Nature of The Roots** for a quadratic equation without solving the equation.

---

## Discriminant ($\Delta$) Rules

* If $\Delta>0$, there are $2$ Distinct real roots.
* If $\Delta=0$, there is $1$ Distinct real root or $2$ equal real roots.
* If $\Delta<0, x\in\mathbb{C}$
* Which can be written like this:
* $$ \begin{equation} \Delta=\begin{cases}\{a,b\}\in\mathbb{R}& \text{if } \Delta>0\\ \{x\}\lor\{a,a\}\in\mathbb{R}& \text{if }\Delta=0\\ x\in\mathbb{C}&\text{if }\Delta<0\end{cases}\end{equation} $$

---

## Example: Nature of the Roots

* Determine the nature of the roots for $3x^2-5x=-9$. **DO NOT SOLVE**.
    * $3x^2-5x+9=0$
    * $\Delta=(-5)^2-4(3*9)$
    * $\Delta=25-108$
    * $\Delta=-83,\Delta<0$ $\therefore x\in\mathbb{C}$

---

# [Next Unit <i class="fa-solid fa-diagram-next"></i>](../Applications/Lesson%201%20(Applications%20Part%201).html)

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">