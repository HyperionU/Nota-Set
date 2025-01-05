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

# Lesson 4: Laws of Logs II

---

## Previously

1. The Product Law: $\log_b MN = \log_b M + \log_b N$
2. The Quotient Law: $\log_b M/N = \log_b M - \log_b N$
3. The Power Law: $\log_b M^P = P \log_b M$
4. The Identity Law: $\log_b 1 = 0$
* But, what if you need a single log, and they aren't all logs?

---

## Combining Complex Logs

Rewrite as one log:

* $1 + \log_5 x$
    * $\log_5 5 + \log_5 x$
    * $\log_5(5x)$
* $\log_2(x^3) - 3$
    * $\log_2 x^3 - \log_2 8$
    * $\log_2(\frac{x^3}{8})$

---

## The Idea of Basis

* Logs have a 'basis', which is the base of the exponential. 
* On most calculators, there is no way to find logs for other bases. 
    * *So, how do we solve it then?*
5) Change of Basis Law: $\log_b a = \frac{\log_c a}{\log_c b}$

---

## Using Change of Basis

* $\log_9 27$
    * $\frac{\log_3 27}{\log_3 9}$
    * $\frac{3}{2}$
* $\log_7 200$
    * $\frac{\log 200}{\log 7}$
    * $\frac{\log 2 + \log 100}{\log 7}$
    * $\frac{\log(2) + 3}{\log 7}$
    * $2.723$

---

## Easier Simplification

To simplify easier, we have another law:

6) Inverse Laws:
    * $\log_b b^x = x \log_b b = x$
    * $b^{\log_b x} = x$
    * $\log_b b = 1$
* For example: $25^{\log_5 x}$
    * $5^{2\log_5 x} = 5^{\log_5 x^2}$
    * $x^2$

---

## Substitution Questions

If $x = \log_4 5$ and $y = \log_4 3$, express the following in terms of x and y:

<div class = "columns">
<span>

* $\log_4 15$
    * $\log_4 (5\cdot 3)$
    * $\log_4 5 + \log_4 3$
    * $x + y$

</span>
<span>

* $\log_4 225$
    * $\log_4 (15^2)$
    * $2 \log_4 15$
    * $2(x + y)$

</span>
</div>

---

## Substitutions, cont.

If $a = \log_3 4$ and $b = \log_5 49$, express the following in terms of a and b:

* $\log_9 4$
    * $\frac{\log_3 4}{\log_3 9} = \frac{a}{2}$
* $\log_5 7$
    * $\log_5 49^\frac{1}{2}$
    * $\frac{1}{2} \log_5 49 = \frac{b}{2}$

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%205%20(Logarithmic%20Equations).html)

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">