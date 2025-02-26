---
marp: true
theme: uncover
class: invert
math: mathjax
---

# <!--fit--> Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2025-->

---

# Lesson 9: Trigonometric Identities

---

<!--paginate: true-->

## Intro

* Identities are equations that are true for all values of the variable where both sides are defined.
* These identities are important to know:
    * Quotient
    * Reciprocal
    * Pythagorean
    * Sum / Difference
    * Double Angle

---

## Basic Identities

* Quotient
    * $\tan x = \frac{\sin x}{\cos x}, x \ne \frac{\pi}{2} + \pi n, n \in \mathbb{Z}$
    * $\cot x = \frac{\cos x}{\sin x}, x \ne \pi n, n \in \mathbb{Z}$
* Reciprocal
    * $\sec x = \frac{1}{\cos x}, x \ne \frac{\pi}{2} + \pi n, n \in \mathbb{Z}$
    * $\csc x = \frac{1}{\sin x}, x \ne \pi n, n \in \mathbb{Z}$
    * $\cot x = \frac{1}{\tan x}, x \ne \frac{\pi}{2} + \pi n, x \ne \pi n, n \in \mathbb{Z}$

---

## Significant Identities

* Pythagorean
    * $\sin^2{x} + \cos^2{x} = 1$
    * $\sec^2{x} = \tan^2{x} + 1,  x \ne \frac{\pi}{2} + \pi n, n \in \mathbb{Z}$
    * $\csc^2{x} = \cot^2{x} + 1, x \ne \pi n, n \in \mathbb{Z}$
* Sum / Difference
    * $\sin(A \pm B) = \sin A \cos B \pm \cos A \sin B$
    * $\cos(A \pm B) = \cos A \cos B \mp \sin A \sin B$

---

## Double Angle: The Most Important

* $\sin 2x = 2\sin x \cos x$
* $\cos 2x = \cos^2{x} - \sin^2 x$
* $\cos 2x = 2 \cos^2{x} - 1$
* $\cos 2x = 1 - 2 \sin^2 x$

---

## Simplification

1. Simplify $\sin x \cot x \sec x$
    * $(\sin x)(\frac{\cos x}{\sin x})(\frac{1}{\cos x}), x \ne n\pi, x \ne \frac{\pi}{2} + n\pi, n \in \mathbb{Z}$
    * $1, x \ne n\pi, x \ne \frac{\pi}{2} + n\pi, n \in \mathbb{Z}$

* Simplify $\cos x \tan x$ (ex. for reader)
* Simplify $\sec x \csc x \sin 2x$ (ex. for reader)
* Simplify $\cos^2 x - \sin^2 x - \cos 2x$ (ex. for reader)
* Simplify $(\sin x + \cos x)^2 - \sin 2x$ (ex. for reader)

---

## Proving Identities

2. Prove $2(1 + \frac{1 - \cos^2 x}{\cos^2 x}) = 2 \sec^2 x$
$$
    \begin{array}{c | c}
        2(1 + \frac{1 - \cos^2 x}{\cos^2 x}) & 2 \sec^2 x \\
        \hline
        2(1 + \frac{\sin^2 x}{\cos^2 x}) & \\
        2(1 + \tan^2 x) & \\
        2\sec^2 x & 2\sec^2 x\\
    \end{array}
$$

* Prove $\sin(x + \pi) = -\sin x$ (ex. for reader)

---

## Complex Proofs

3. Prove $\frac{\tan x + \cot x}{2}(\sin 2x) = 1$
$$
    \begin{array}{c | c}
        \frac{\tan x + \cot x}{2}(\sin 2x) & 1 \\
        \hline
        \frac{\frac{\sin x}{\cos x} + \frac{\cos x}{\sin x}}{2}(2 \sin x \cos x) & \\
        (\frac{\sin x}{\cos x} + \frac{\cos x}{\sin x})(\sin x \cos x) & \\
        (\frac{\sin^2 x + \cos^2 x}{\sin x \cos x})(\sin x \cos x) & \\
        \sin^2 x + \cos^2 x & \\
        1 & 1 \\
    \end{array}
$$

---

## Exercise

* Prove $\cos(\frac{\pi}{2} + x) = -\sin x$ (ex. for reader)
* Prove $\frac{1 + \sin x}{\cos x} = \frac{\cos x}{1 - \sin x}$ (ex. for reader)
* Prove $\frac{1}{1 + \sin x} + \frac{1}{1 - \sin x} = 2 \sec^2 x$ (ex. for reader)

---

# [Next Unit](../Limits/Lesson%201)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercise

* Simplify $\cos x \tan x$
    * $\cos x \frac{\sin x}{\cos x}, x \ne \frac{\pi}{2} + n\pi, x \in \mathbb{Z}$
    * $\sin x, x \ne \frac{\pi}{2} + n\pi, x \in \mathbb{Z}$
* Simplify $\sec x \csc x \sin 2x$
    * $\frac{1}{\cos x}(\frac{1}{\sin x})(2\sin x \cos x), x \ne \frac{\pi}{2} + n\pi, x \ne n\pi, x \in \mathbb{Z}$
    * $2, x \ne \frac{\pi}{2} + n\pi, x \ne n\pi, x \in \mathbb{Z}$

---

## Answers to Exercise, cont.

* Simplify $\cos^2 x - \sin^2 x - \cos 2x$
    * $\cos 2x - \cos 2x$
    * $0$
* Simplify $(\sin x + \cos x)^2 - \sin 2x$
    * $\sin^2 x + 2\sin x \cos x + \cos^2 x - \sin 2x$
    * $\sin^2 x + \cos^2 x + \sin 2x - \sin 2x$
    * $\sin^2 x + \cos^2 x$
    * $1$

---

## Answers to Exercise, cont.

* Prove $\sin(x + \pi) = -\sin x$

$$
    \begin{array}{c | c}
        \sin(x + \pi) & -\sin x \\
        \hline
        \sin x \cos \pi + \sin \pi \cos x & \\
        \sin x (-1) + (0) \cos x & \\
        -\sin x & -\sin x\\
    \end{array}
$$

---

## Answers to Exercise, cont.

* Prove $\cos(\frac{\pi}{2} + x) = -\sin x$

$$
    \begin{array}{c | c}
        \cos(\frac{\pi}{2} + x) & -\sin x \\
        \hline
        \cos x \cos \frac{\pi}{2} - \sin \frac{\pi}{2} \sin x & \\
        0\cos x - 1\sin x & \\
        -\sin x & -\sin x\\
    \end{array}
$$

---

## Answers to Exercise, cont.

* Prove $\frac{1 + \sin x}{\cos x} = \frac{\cos x}{1 - \sin x}$

$$
    \begin{array}{c | c}
        \frac{1 + \sin x}{\cos x} & \frac{\cos x}{1 - \sin x} \\
        \hline
        & \frac{\cos x}{1 - \sin x}(\frac{1 + \sin x}{1 + \sin x}) \\
        & \frac{\cos x(1 + \sin x)}{1 - \sin^2 x} \\
        & \frac{\cos x(1 + \sin x)}{\cos^2 x} \\
        \frac{1 + \sin x}{\cos x} & \frac{1 + \sin x}{\cos x} \\
    \end{array}
$$

---

## Answers to Exercise, cont.

* Prove $\frac{1}{1 + \sin x} + \frac{1}{1 - \sin x} = 2 \sec^2 x$

$$
    \begin{array}{c | c}
        \frac{1}{1 + \sin x} + \frac{1}{1 - \sin x} & 2 \sec^2 x \\
        \hline
        \frac{1 - \sin x}{(1 + \sin x)(1 - \sin x)} + \frac{1 + \sin x}{(1 - \sin x)(1 + \sin x)} & \\
        \frac{1 - \sin x + 1 + \sin x}{(1 + \sin x)(1 - \sin x)} & \\
        \frac{1 + 1}{1 - \sin^2 x} & \\
        \frac{2}{\cos^2 x} & \\
        2\sec^2 x & 2 \sec^2 x \\
    \end{array}
$$

---

# [Next Unit](../Limits/Lesson%201)