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

$\newcommand{\wfr}[1]{\frac{#1}{1}}$

---

## Lesson 2:  Adding & Subtracting Rationals

---

## Adding & Subtracting

* Since we're dealing with fractions, the same rules apply. One of the fundamental rules is that when adding or subtracting fractions, there must be a common denominator.
* Example: $\frac{2x}{3y}+\frac{6x}{3y}$
    * $\frac{8x}{3y}, y\neq0$.
* Example: $\frac{10m-1}{4m-3}-\frac{8-2m}{4m-3}$
    * $\frac{12m-9}{4m-3}, m\neq\frac{3}{4}$
    * $3,m\neq\frac{3}{4}$

---

## Finding a Common Denominator

* Finding a common denominator with variables is very similar to what you have already done.
* Example: $\frac{5}{a}+\frac{7}{b}$
    * $\frac{5b}{ab}+\frac{7a}{ab}, a,b\neq0$
    * $\frac{5b+7a}{ab},a,b\neq0$

---

## Example 4: Addition

1) $\frac{y^2-20}{y^2-4}+\frac{y-2}{y+2}$
    * We have two $y^2$ we'll need to factor early on.
2) $\frac{y^2-20}{(y+2)(y-2)}+\frac{y-2}{y+2}$
    * Next, state the NPVs: $y\neq\pm2$, and determine LCD: $(y-2)(y+2)$
3) $\frac{y^2-20}{(y-2)(y+2)}+\frac{(y-2)^2}{(y-2)(y+2)}$
    * FOIL $(y-2)^2$: $y^2-4y+4$
4) $\frac{y^2-20}{(y-2)(y+2)}+\frac{y^2-4y+4}{(y-2)(y+2)}$
    * Rewrite the rational.

---

## Example 4, cont.

5) $\frac{(y^2-20)+(y^2-4y+4)}{(y-2)(y+2)}$
    * Combine like terms.
6) $\frac{2y^2-4y-16}{(y-2)(y+2)}$
    * Simplify numerator (Factor!)
7) $\frac{2(y-4)(y+2)}{(y-2)(y+2)}$
    * Simplify like terms.
8) $\frac{2(y-4)}{y-2},y\neq\pm2$

---

## Example 5: Subtraction

1) $\frac{x+3}{x-5}-\frac{x-7}{x-2}$
    * Determine common denominator: $(x-5)(x-2)$
2) $\frac{(x+3)(x-2)}{(x-5)(x-2)}-\frac{(x-7)(x-5)}{(x-2)(x-5)}$
    * State NPVs: $x\neq2,5$ and FOIL
3) $\frac{x^2+x-6}{(x-5)(x+2)}-\frac{x^2-12x+35}{(x-5)(x+2)}$
    * Rewrite the Rational
4) $\frac{(x^2+x-6)-(x^2-12x+35)}{(x-5)(x+2)}$
    * Rewrite the Subtraction

---

## Example 5, cont.

5) $\frac{(x^2+x-6)+(-x^2+12x-35)}{(x-5)(x+2)}$
    * Combine like terms
6) $\frac{13x-41}{(x-5)(x-2)}$
    * If possible, simplify.
        * 13 is prime, so we can't.
7) $\frac{13x-41}{(x-5)(x-2)}, x\neq2,5$

---

## Example 6: Recursion

1) $\frac{2-\frac{4}{y}}{y-\frac{4}{y}}$
    * The bar means division, so rewrite horizontally.
2) $[\wfr{2}-\frac{4}{y}]/[\wfr{y}-\frac{4}{y}]$
    * State NPVs: $y\neq0$ & Determine Common Denominator for each set: $y$.
3) $\frac{2y-4}{y}/\frac{y^2-4}{y}$
    * Kiss and Flip, add another NPV: $y\neq\pm2$.
        * *Why another NPV? Keep NPVs Up to Date. Any new denominator = new NPVs.*

---

## Example 6, cont.

4) $\frac{2y-4}{y}\times\frac{y}{(y-2)(y+2)}$
    * Old Denominators cross-cancel.
5) $\frac{2y-4}{(y-2)(y+2)}$
    * Factor as needed.
6) $\frac{2(y-2)}{(y-2)(y+2)}$
    * Combine like terms.
7) $\frac{2}{y+2}, y\neq0,\pm2$

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%203%20(Multipling%20+%20Dividing).html) 

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">