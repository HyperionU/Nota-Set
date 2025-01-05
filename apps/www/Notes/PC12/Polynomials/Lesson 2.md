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

# Lesson 2: Substitution and Remainder Theorem

---

<!--paginate: true-->

## Substitution

If $f(x) = 3x^3 + 2x^2 - 4x - 5$, what is the value of $f(2)$?

* $f(2) = 3(2)^3 + 2(2)^2 - 4(2) - 5$
* $f(2) = 24 + 8 - 8 - 5$
* $f(2) = 24 - 5$
* $f(2) = 19$

---

## Division

Determine the remainder when $3x^3 + 2x^2 - 4x - 5$ is divided by $(x - 2)$

$$
    \begin{array}{c|rrrr}
        & 3 & 2 & -4 & -5 \\
        2 & \downarrow & 6 & 16 & 24 \\
        \hline
        & 3 & 8 & 12 & \fbox{19} \\
    \end{array}
$$

* *Wait, it's the value of f(2)*
* *Yep. This means that* $f(a) = f(x) \mod (x - a)$

---

## Comparison

<div class = "columns">
<div>
    
If $f(x) = x^2 + x - 5$, what is the value of $f(1)$? (Substitution)

* $f(1) = (1)^2 + (1) - 5$
* $f(1) = 2 - 5$
* $f(1) = -3$

</div>  
<div>

What is the remainder of $x^2 + x - 5 / (x - 1)$? (Synthetic Division)

$$
    \begin{array}{c|rrr}
        & 1 & 1 & -5 \\
        1 & \downarrow & 1 & 2 \\
        \hline
        & 1 & 2 & \fbox{-3} \\
    \end{array}
$$

</div>
</div>

They look the exact same!

---

## Remainder / Modulus Theorem

$\textbf{Theorem:}$ *let* $P(x)$ *be a polynomial. For* $P(x) / (x - a),\ P(x) \mod (x-a) = P(a)$ 

* In plain terms, The remainder when dividing a polynomial by $(x - a)$ is equal to the value of the polynomial evaluated at $a$.
* This means Synthetic Substitution is equivalent to Synthetic Division.

---

## Example

Use the remainder theorem to determine the remainder of $P(x) = 3x^3 - 2x^2 + 5x - 7$ divided by $(x + 1)$.
* $x = -1$

<div class = "columns">
<div>

* $P(-1) = 3x^3 - 2x^2 + 5x - 7$
* $P(-1) = -3 - 2 - 5 - 7$
* $P(-1) = -17$

</div>  
<div>

$$
    \begin{array}{c|rrrr}
        & 3 & 2 & 5 & -7 \\
        -1 & \downarrow & -3 & 1 & -6 \\
        \hline
        & 3 & -1 & 6 & \fbox{-17} \\
    \end{array}
$$

</div>
</div>

---

## Q and R

Find the quotient and remander when $P(x) = 2x^3 + 3x^2 - 4x + 15$ divided by $(x + 3)$

$$
    \begin{array}{c|rrrr}
        & 2 & 3 & -4 & 15 \\
        -3 & \downarrow & -6 & 9 & -15 \\
        \hline
        & 2 & -3 & 5 & \fbox{0} \\
    \end{array}

$$

* If the remainder is zero: The divisor divides evenly, which means it's a factor. (you'll see more later.)

---

## Finding Coefficients

Find $a$ and $b$ if 
* $P(x) = x^3 + ax^2 - bx - 15$
* $P(x) \mod (x - 2) = 7, P(2) = 7$
* $P(x) \mod (x + 4) = 13, P(-4) = 13$

Here's the process:

---

## Finding Coefficients: Step 1

1. Evaluate $P(x)$ for each.
    * $(2)^3 + a(2)^2 - 2b - 15 = 7$
    * $4a - 2b - 7 = 7$
    * $4a - 2b = 14$
    * $(-4)^3 + a(-4)^2 + 4b - 15 = 13$
    * $16a + 4b - 79 = 13$
    * $16a + 4b = 92$

---

## Finding Coefficients: Step 2

2. Solve this system.
    $4a - 2b = 14$
    $16a + 4b = 92$
* We'll solve for $a$ first.
    $2(4a - 2b) + 16a + 4b = 28 + 92$
    $24a = 120, a = 5$
* Now, solve for $b$.
    $20 - 2b = 14$
    $-2b = -6, b = 3$

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%203%20(Factor%20Theorem).html) 

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">