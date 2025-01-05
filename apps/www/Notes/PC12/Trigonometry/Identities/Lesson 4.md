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

# Lesson 4: Double Angle Identities

---

## Sine Double Angle

Let's derive it:

$\sin 2x = \sin(x + x)$
$\sin(x + x) = \sin x \cos x + \cos x \sin x$
$2(\sin x) 2(\cos x)$
$2\sin x \cos x$

12. $\sin 2x = 2 \sin x \cos x$

---

## Sine Identities

12. $\sin 2x = 2 \sin x \cos x$

* $\sin 4x = 2 \sin 2x \cos 2x$
* $\sin 10\theta = 2 \sin 5\theta \cos 5\theta$
* $\sin 12x = 2 \sin 6x \cos 6x$
* $2 \sin 3B \cos 3B = \sin 6B$
* $\sin 4x \cos 4x = \frac{\sin 8x}{2}$

---

## Cosine Double Angle

Let's derive it:

$\cos 2x = \cos(x + x)$
$\cos(x + x) = \cos x (\cos x) - \sin x (\sin x)$
$\cos^2 x - \sin^2 x$

13. $\cos 2x = \cos^2 x - \sin^2 x$

---

## First Cosine Identity

13. $\cos 2x = \cos^2 x - \sin^2 x$

* $\cos 8x = \cos^2 4x - \sin^2 4x$
* $\cos^2 5B - \sin^2 5B = \cos 10B$

---

## Cosine Double Angles, part I

Starting from 13: $\cos 2x = \cos^2 x - \sin^2 x$, we can get the other two cosine double angle identities.

$\cos 2x = \cos^2 x - \sin^2 x$
$\cos^2 x = 1 - \sin^2 x$
$\cos 2x = 1 - \sin^2 x - \sin^2 x$
$\cos 2x = 1 - 2 \sin^2 x$

14. $\cos 2x = 1 - 2 \sin^2 x$
* $\cos 10 x = 1 - 2 \sin^2 5x$

---

## Cosine Double Angles, part II

Starting from 13: $\cos 2x = \cos^2 x - \sin^2 x$, we can get the other two cosine double angle identities.

$\cos 2x = \cos^2 x - \sin^2 x$
$\sin^2 x = 1 - \cos^2 x$
$\cos 2x = 1 - \cos^2 x - \cos^2 x$
$\cos 2x = 1 - 2 \cos^2 x$

15. $\cos 2x = 2 \cos^2 x - 1$
* $\cos 8 x = 2 \cos^2 4x - 1$

---

## Cosine Double Angles

Here are our 3 identities for $\cos 2x$

13. $\cos 2x = \cos^2 x - \sin^2 x$ for both sine and cosine.
14. $\cos 2x = 1 - 2 \sin^2 x$ for only sine.
15. $\cos 2x = 2 \cos^2 x - 1$ for only cosine.

---

## Tangent Double Angle

Last is for $\tan 2x$. Let's derive it:

$\tan 2x = \tan(x + x)$
$\tan(x + x) = \frac{\tan x + \tan x}{1 - \tan x \tan x}$
$\frac{2 \tan x}{1 - \tan^2 x}$

16. $\tan 2x = \frac{2 \tan x}{1 - \tan^2 x}$
* $\tan 8x = \frac{2 \tan 4x}{1 - \tan^2 4x}$

---

## Proving w/ Double Angle

Besides simplifying double angles to single angles, you will use them to prove identities. Like this one: 
$\frac{\sin 2x}{2 \sin^2 x} = \cot x$

$$
    \begin{array}{c|c}
        \hline
        \frac{\sin 2x}{2 \sin^2 x} & \cot x \\
        \frac{\not2 \sin x \cos x}{\not2 \sin^2 x} & \frac{\cos x}{\sin x} \\
        \frac{\cos x}{\sin x} & \frac{\cos x}{\sin x}
    \end{array}
$$

---

## More Proofs

$\cos 2\theta = \frac{\cot^2 \theta - 1}{\csc^2 \theta}$

$$
    \begin{array}{c|c}
        \hline
        \cos 2\theta & \frac{\cot^2 \theta - 1}{\csc^2 \theta} \\
        & \frac{\cos^2 \theta}{\sin^2 \theta} - 1 / \frac{1}{\sin^2 \theta} \\
        & \cos^2 \theta - \sin^2 \theta \\
        \cos 2\theta & \cos 2\theta
    \end{array}
$$

How about a challenge?

---

$\cos 3x = 4 \cos^3 x - 3 \cos x$

$$
    \begin{array}{c|c}
        \hline
        \cos 3x & 4 \cos^3 x - 3 \cos x \\
        \cos(2x + x) & \\
        \cos 2x \cos x - \sin 2x \sin x & \\
        (2 \cos^2 x - 1)\cos x - \sin x (2 \sin x \cos x) & \\
        [2 \cos^3 x - \cos x] - 2 \sin^2 x \cos x & \\
        (2 \cos^3 x - \cos x) - 2 \cos x (1 - \cos^2 x) & \\
        (2 \cos^3 x - \cos x) + (-2 \cos x + 2 \cos^3 x) & \\
        4 \cos^3 x - 3 \cos x & 4 \cos^3 x - 3 \cos x
    \end{array}
$$

---

# [Next Unit <i class="fa-solid fa-diagram-next"></i>](../../Exponentials/Lesson%201%20(Solving%20Exponentials).html)

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">