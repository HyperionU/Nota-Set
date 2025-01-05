---
marp: true
theme: uncover
class: invert
math: mathjax
style: |
  .columns {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1rem;
  }
---

# <!--fit--> Pre-Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2024-->

---

<!--paginate: true-->

# Lesson 1: Solving Exponential Equations

---

## On Exponents

You should be familiar with powers of integers:

$2^n = 2, 4, 8, 16, 32, \cdots$
$3^n = 3, 9, 27, 81, 243, \cdots$
$4^n = 4, 16, 64, 256, \cdots$
$5^n = 5, 25, 125, 625, \cdots$
$6^n = 6, 36, 216, \cdots$

---

## Exponent Rules

<div class = "columns">
<span>

* Identity
    * $x^0 = 1$
* Product
    * $x^m \cdot x^n = x^{m + n}$
* Quotient
    * $\frac{x^m}{x^n} = x^{m - n}$
* Power
    * $(x^m)^n = x^{mn}$
* Distributive Product
    * $(xy)^m = x^m y^m$

</span>
<span>

* Distributive Quotient
    * $(\frac{x}{y})^m = \frac{x^m}{y^m}$
* Inverse
    * $x^{-n} = \frac{1}{x^n}$
* Reciprocal
    * $(\frac{x}{y})^{-n} = (\frac{y}{x})^n$
* Fractional
    * $x^\frac{m}{n} = \sqrt[n]{x^m} = (\sqrt[n]{x})^m$


</span>
</div>

---

## On Exponent Rules

* They all deal with multiplication and division.
* Must have **SAME** base to combine
* Fractional Exponents are radicals in disguise.
* Quite often, you'll convert radicals to rational exponents instead

---

## Solving Exponential Equations

Strategy: if $b^x = b^y, x = y$

When Solving:
* Get the same base
* set exponents equal to each other

1. $8^{3x - 2} = 16^{x + 1}$
    * $(2^3)^{3x - 2} = (2^4)^{x + 1}$
    * $2^{9x - 6} = 2^{4x + 4}$
    * $9x - 6 = 4x + 4$
    * $5x = 10, x = 2$ 

---

## Solving Exponentials

2. $27^{x + 3} = (\frac{1}{9})^{2x - 5}$
    * $3^{3(x + 3)} = 3^{-2(2x - 5)}$
    * $3^{3x + 9} = 3^{10 - 4x}$
    * $3x + 9 = 10 - 4x$
    * $7x = 1, x = \frac{1}{7}$

---

## Solving Exponentials, cont.

3. $\frac{8^{x + 6}}{16^{2x - 1}} = 32^{3x - 4}$
    * $2^{3(x + 6)} / 2^{4(2x - 1)} = 2^{5(3x - 4)}$
    * $2^{3x + 18} / 2^{8x - 4} = 2^{15x - 20}$
    * $(3x + 18) - (8x - 4) = 15x - 20$
    * $22 - 5x = 15x - 20$
    * $20x = 42, x = \frac{21}{10}$

---

## Solving, cont.

<div class="columns">
<span>

4. $4^{2x - 1} = 1$
    * Identity Law: $x^0 = 1$
    * $4^{2x - 1} = 4^0$
    * $2x - 1 = 0$
    * $2x = 1, x = \frac{1}{2}$

</span>
<span>

5. $2^{x + 4} - 3 = 1$
    * Isolate the exponential
    * $2^{x + 4} = 4$
    * $2^{x + 4} = 2^2$
    * $x + 4 = 2, x = -2$

</span>
</div>

---

## Solving, cont.

6. $5(9)^{x + 2} = 15$
    * Isolate the exponential
    * $9^{x + 2} = 3$
    * $3^{2(x + 2)} = 3^1$
    * $2x + 4 = 1$
    * $2x = -3, x = \frac{-3}{2}$

---

## Simplifying

<div class = "columns">

<span>
Solving is very different from simplifying. The big difference is that solving has an = sign. 
Make sure to check whether to simplify or solve.
</span>

<span>

$$
    \frac{3^{x + 4} \cdot 27^{2x + 1}}{9^{3x - 4}}
$$

$$
    \frac{3^{x + 4} \cdot 3^{3(2x + 1)}}{3^{2(3x - 4)}}
$$

$3^{x + 4} \times 3^{6x + 3} / 3^{6x - 8}$

$3^{7x + 7} / 3^{6x - 8}$

$3^{(7x + 7) - (6x - 8)} = 3^{x + 15}$

</span>
</div>

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%202%20(Graphing%20Exponentials).html)

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">