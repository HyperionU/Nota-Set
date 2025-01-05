---
marp: true
theme: uncover
class: invert
math: mathjax
---

# <!--fit--> Pre-Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2024-->

---

<!--paginate: true-->

# Lesson 1: Definitions

---

## Solutions

If you were asked to solve $\sin x = 1$, you would use the general solution.

For $\sin x = 1$, you'd get $x = \frac{\pi}{2} \pm 2\pi n, n \in \mathbb{N}$

---

## Identities

How about $\tan x = \frac{\sin x}{\cos x}$?

You would get $\forall x(\tan x = \frac{\sin x}{\cos x}, \cos x \not = 0)$. 
This is called an Identity. And already, you know some of them.

---

## The Basic Identites (Quotient / Reciprocal)

1. $\tan x = \frac{\sin x}{\cos x}, \cos x \not = 0$

2. $\csc x = \frac{1}{\sin x}, \sin x \not = 0$

3. $\sec x = \frac{1}{\cos x}, \cos x \not = 0$

4. $\cot x = \frac{1}{\tan x}, \sin x \not = 0$

5. $\cot x = \frac{\cos x}{\sin x}, \sin x \not = 0$

---

## Simplification

Simplify the following:

1. $\cot x \sin x$
2. $\frac{\sec^2 x \cos x}{\csc x}$
3. $\frac{\csc x}{\tan x + \cot x}$

Here's some tips: 

* Convert to $\sin x$ and $\cos x$
* Reduce from there.

---

## Simplification, cont.

1. $\cot x \sin x$
    * $\frac{\cos x}{\sin x} \sin x$
    * $\cos x$
2. $\frac{\sec^2 x \cos x}{\csc x}$
    * $\frac{1 / \cos^2 x \cos x}{1 / \sin x}$
    * $\frac{1 / \cos x}{1 / \sin x}$
    * $\frac{\sin x}{\cos x} = \tan x$

---

## Simplification, cont.

3. $\frac{\csc x}{\tan x + \cot x}$
    * $\frac{1 / \sin x}{\sin x / \cos x + \cos x / \sin x}$
    * $\frac{\cos x}{\sin^2 x + \cos^2 x}$
    * $\cos x$ 
    * *Wait. How?* You'll see.

---

## Factoring

Factor the Following:
1. $3 \csc^2 x - 6 \csc x$
    * $3 \csc x(\csc x - 2)$
2. $4 \cos^2 x - 9 \sin^2 x$
    * $(2 \cos x + 3 \sin x)(2 \cos x - 3 \sin x)$
3. $3 \tan^2 x + \tan x - 2$
    * $(3 \tan x - 2)(\tan x + 1)$

---

## Reduction

Write as a single term:

1. $\frac{1}{\sin x} + \frac{1}{\cos x}$
    * $\frac{\cos x + \sin x}{\sin x \cos x}$
2. $\frac{1}{1 + \sin x} - \frac{3}{1 - \sin x}$
    * $\frac{1 - \sin x - (3 + 3\sin x)}{(1 + \sin x)(1 - \sin x)}$
    * $\frac{-4 \sin x - 2 \sin x}{1 - \sin^2 x}$
    * $\frac{-2(2 \sin x - 1)}{1 - \sin x}$

---

## Reduction, cont.

3. $\frac{4}{3 \sin x} + \frac{1}{\sin x \cos^2 x}$
    * $\frac{4 \cos^2 x + 3}{3 \sin x \cos^2 x}$

---

## Determining Values

Given that an angle $\theta$ terminates in $\mathfrak{Q}_3 \text{ and } \sin \theta = -\frac{5}{8}$, determine the value of $\cos \theta$.

* $x^2 + 5^2 = 8^2$
* $x^2 + 25 = 64$
* $x^2 = 39$
* $x = \pm \sqrt{39}$
* $\cos \theta = \frac{- \sqrt{39}}{8}$

---

## Determining Restrictions

Determine the restrictions for the following:
1. $\frac{\tan x}{1 - \sin x}$
    * $\frac{\sin x / \cos x}{1 - \sin x}$
    * $\cos x \not = 0, \sin x \not = 1$
2. $\frac{\csc x - 2}{2 - 3 \cos x}$
    * $\frac{1}{\sin x} - 2 / 2 - 3 \cos x$
    * $\sin x \not = 0, \cos x \not = \frac{2}{3}$

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%202%20(Pythagorean).html)

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">