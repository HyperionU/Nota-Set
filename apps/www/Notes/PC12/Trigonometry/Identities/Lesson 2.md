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

# Lesson 2: Pythagorean Identities

---

## The Pythagorean Identities

6. $\sin^2 x + \cos^2 x = 1$
    * $\cos^2 x = 1 - \sin^2 x$
    * $\sin^2 x = 1 - \cos^2 x$
7. $1 + \tan^2 x = \sec^2 x$
    * $\tan^2 x = \sec^2 x - 1$
    * $1 = \sec^2 x - \tan^2 x$
8. $1 + \cot^2 x = \csc^2 x$
    * $\cot^2 x = \csc^2 x - 1$
    * $1 = \csc^2 x - \cot^2 x$

---

## Verify

Verify means plug in an angle to see if it works.

Verify that $\tan x (\tan x + \cot x) = \sec^2 x$ using $x = \frac{\pi}{6}$

$\tan^2 x + \cot x \tan x = \sec^2 x$
$(\frac{1}{\sqrt{3}})^2 + 1 = (\frac{2}{\sqrt{3}})^2$
$\frac{1}{3} + \frac{3}{3} = \frac{4}{3}$
$\frac{4}{3} = \frac{4}{3}$

---

## Proving Using Identities

Prove means substituting identities until both sides are equal.

$\tan x (\tan x + \cot x) = \sec^2 x$

$$
    \begin{array}{c|c}
        \hline
        \tan x (\tan x + \cot x) & \sec^2 x \\
        \tan^2 x + \tan x \cot x & \\
        \tan^2 x + 1 & \\
        \sec^2 x & \sec^2 x
    \end{array}
$$

---

## More Proofs

$\tan x + \cot x = \sec x \csc x$

$$
    \begin{array}{c|c}
        \hline
        \tan x + \cot x & \sec x \csc x \\
        \frac{\sin^2 x + \cos^2 x}{\cos x \sin x} & \frac{1}{\cos x \sin x}  \\
        \frac{1}{\cos x \sin x} & \frac{1}{\cos x \sin x}
    \end{array}
$$

---

## More Proofs, cont

$2 \csc^2 x = \frac{1}{1 + \cos x} + \frac{1}{1 - \cos x}$

$$
    \begin{array}{c|c}
        \hline
        2 \csc^2 x & \frac{1}{1 + \cos x} + \frac{1}{1 - \cos x} \\
        \frac{2}{\sin^2 x} & \frac{2}{1 - \cos^2 x} \\
        \frac{2}{\sin^2 x} & \frac{2}{\sin^2 x}
    \end{array}
$$

---

## Proofs, cont.

$\frac{\sec x - \cos x}{\tan x} = \sin x$

$$
    \begin{array}{c|c}
        \hline
        \frac{\sec x - \cos x}{\tan x} & \sin x \\
        \frac{\frac{1}{\cos x} - \cos x}{\frac{\sin x}{\cos x}} & \\
        \frac{1 - \cos^2 x}{\sin x} & \\
        \frac{\sin^2 x}{\sin x} & \\
        \sin x & \sin x
    \end{array}
$$

---

## Rules of Proofs

* **NEVER** cross the equal sign
* Work vertically

---

## Hints
* Change to $\sin x$ and $\cos x$
* Common Denominator
* Factoring
* "Glaring Identities" (Identities 1-5)
* Complex Fractions
* Conjugates
* Aim for the denominator you want

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%203%20(Sum%20and%20Difference).html)

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">