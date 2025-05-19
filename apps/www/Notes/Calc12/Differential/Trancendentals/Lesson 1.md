---
marp: true
theme: uncover
class: invert
math: mathjax
---

$\newcommand\diff[1]{\mathcal{d}_{#1}}$
$\newcommand\dd[2][]{\displaystyle\frac{d#1}{d#2}}$

# <!--fit--> Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2025-->

$\newcommand\limit[2]{\displaystyle\lim_{#1 \to #2}}$

---

# Lesson 1: Limits of Trigonometric Functions

---

<!--paginate: true-->

## Intro

* In the previous unit, you learned how to calculate the **Derivative** for three types of functions:
    - Polynomials
    - Rationals
    - Radicals
* These are sometimes known as *Elementary Functions*. 
* They can be made by a finite number of basic operations ($+, -, \times, /, \circ$), 
* And can be expressed as solutions to polynomial equations w/ polynomial coefficients.

---

## Intro, cont.

* However, in this unit, you'll learn how to calculate the **Derivative** for three types of functions:
    - Trigonometric
    - Exponential
    - Logarithmic
* These are sometimes known as *Transcendental Functions*. 
* They can't be expressed as solutions to polynomial equations w/ polynomial coefficients.

---

## Limits of Trigonometric Functions

* In order to understand the derivatives of trigonometric functions, we need to understand how to evaluate two important limits.
    * $\limit{x}{0} \frac{\sin x}{x}$
    * $\limit{x}{0} \frac{\cos x - 1}{x}$
* Let's start with the first one: $\limit{x}{0} \frac{\sin x}{x}$

---

## Limit of $\sin x / x$

* $\limit{\theta}{0} \frac{\sin \theta}{\theta}$
* Start with a unit circle.
* Let $O$ be the Origin, $A$ be the intersection between the unit circle and the radius, and $D$ be the point $(1,0)$.
* Create another circle inside the circle with a radius of $\cos \theta$.
* Let $B$ be the point $(\cos \theta, 0)$, and $C$ be the intersection between the radius and this smaller circle.

---

## Limit of $\sin x / x$, cont.

* Let $R$ be the radius of the Unit Circle ($1$), and $r$ be the radius of the smaller circle ($\cos \theta$) 
* Given $O, A, B, C, D, R, r, \theta$, we know this:
    * $R = 1$
    * $r = \cos \theta$
    * $0 \le \theta \le \frac{\pi}{2}$
    * $\mathcal{A}(OCB) \le \mathcal{A}(OAB) \le \mathcal{A}(OAD)$
    * $\mathcal{A}(OCB) = \frac{1}{2} r^2\theta$, $\mathcal{A}(OAB) = \frac{1}{2} \cos \theta \sin \theta$, $\mathcal{A}(OAD) = \frac{1}{2} R^2\theta$

---

## Limit of $\sin x / x$, cont.

* We know this:
    * a: $R = 1$
    * b: $r = \cos \theta$
    * c: $0 \le \theta \le \frac{\pi}{2}$
    * d: $\mathcal{A}(OCB) \le \mathcal{A}(OAB) \le \mathcal{A}(OAD)$
    * e: $\mathcal{A}(OCB) = \frac{1}{2} r^2\theta$
    * f: $\mathcal{A}(OAB) = \frac{1}{2} \cos \theta \sin \theta$
    * g: $\mathcal{A}(OAD) = \frac{1}{2} R^2\theta$

---

## Limit of $\sin x / x$, cont.

* From d, e, f, g:
    * $\frac{1}{2} r^2\theta \le \frac{1}{2} \cos \theta \sin \theta \le \frac{1}{2} R^2\theta$
* From a, b:
    * $\frac{1}{2} (\cos \theta)^2\theta \le \frac{1}{2} \cos \theta \sin \theta \le \frac{1}{2} (1)^2 \theta$
    * $\frac{1}{2} (\cos \theta)^2\theta \le \frac{1}{2} \cos \theta \sin \theta \le \frac{1}{2} \theta$
* Divide by $\frac{1}{2}$
    * $(\cos \theta)^2\theta \le \cos \theta \sin \theta \le \theta$
* Divide by $\theta (\cos \theta)$
    * $\cos \theta \le \frac{\sin \theta}{\theta} \le \frac{1}{\cos \theta}$

---

## Limit of $\sin x / x$, cont.
* $\cos x \le \frac{\sin x}{x} \le \frac{1}{\cos x}$
* $\limit{x}{0} [\cos x \le \frac{\sin x}{x} \le \frac{1}{\cos x}]$
* $\limit{x}{0} \cos x \le \limit{x}{0} \frac{\sin x}{x} \le \limit{x}{0} \frac{1}{\cos x}$
* $1 \le \limit{x}{0} \frac{\sin x}{x} \le 1$
* $\therefore \limit{x}{0} \frac{\sin x}{x} \equiv 1$.
* We can now solve limits which can be manipulated to this form.

---

## Example 1

1. Evaluate $\limit{x}{0} \frac{\sin 2x}{x}$
    * $\limit{x}{0} \frac{2 \sin 2x}{2x}$
    * $2 \limit{x}{0} \frac{\sin 2x}{2x}$
    * $2$

---

## Example 2

2. Evaluate $\limit{\theta}{0} \frac{\sin 3\theta}{4 \theta}$
    * $\limit{\theta}{0} \frac{3\sin 3\theta}{(3)4 \theta}$
    * $\limit{\theta}{0} \frac{3}{4}\frac{\sin 3\theta}{3\theta}$
    * $\frac{3}{4} \limit{\theta}{0} \frac{\sin 3\theta}{3\theta}$
    * $\frac{3}{4}$

---

## Example 3

3. Evaluate $\limit{x}{0} \frac{\sin^2 2x}{x}$
    * $\limit{x}{0} \frac{\sin 2x (\sin 2x)}{x}$
    * $\limit{x}{0} \frac{4x \sin 2x (\sin 2x)}{4x^2}$
    * $\limit{x}{0} \frac{4x \sin 2x}{2x} \frac{\sin 2x}{2x}$
    * $\limit{x}{0} 4x\frac{\sin 2x}{2x} \frac{\sin 2x}{2x}$

---

## Example 3, cont.

3. Evaluate $\limit{x}{0} \frac{\sin^2 2x}{x}$
    * $\limit{x}{0} 4x \limit{x}{0} \frac{\sin 2x}{2x} \limit{x}{0} \frac{\sin 2x}{2x}$
    * $\limit{x}{0} 4x$
    * $4(0)$
    * $0$

* Now that you have the hang of this, let's develop the other Important Trigonometric Limit: $\limit{x}{0} \frac{\cos x - 1}{x}$


---

## Limit of $(\cos x - 1) / x$

* $\limit{x}{0} \frac{\cos x - 1}{x}$
* $\limit{x}{0} \frac{(\cos x - 1)(\cos x + 1)}{x(\cos x + 1)}$
* $\limit{x}{0} \frac{\cos^2 x - 1}{x(\cos x + 1)}$
* $\limit{x}{0} \frac{-(1 - \cos^2 x)}{x(\cos x + 1)}$
* $\limit{x}{0} \frac{-\sin^2 x}{x(\cos x + 1)}$

---

## Limit of $(\cos x - 1) / x$, cont.

* $\limit{x}{0} \frac{-\sin^2 x}{x(\cos x + 1)}$
* $-\limit{x}{0} \frac{\sin^2 x}{x(\cos x + 1)}$
* $-\limit{x}{0} \frac{\sin x(\sin x)}{x(\cos x + 1)}$
* $-(\limit{x}{0} \frac{\sin x}{x} \limit{x}{0} \frac{\sin x}{\cos x + 1})$
* $-\limit{x}{0} \frac{\sin x}{\cos x + 1}$

---

## Limit of $(\cos x - 1) / x$, cont.

* $-\limit{x}{0} \frac{\sin x}{\cos x + 1}$
* $-\frac{\sin 0}{\cos 0 + 1}$
* $-\frac{0}{2}$
* $0$
* $\therefore \limit{x}{0} \frac{\cos x - 1}{x} \equiv 0$

* Now, let's try evaluating some like this.

---

## Example 4

4. Evaluate $\limit{x}{0} \frac{2\cos x - 2}{5x}$
    * $\limit{x}{0} \frac{2(\cos x - 1)}{5x}$
    * $\frac{2}{5} \limit{x}{0} \frac{\cos x - 1}{x}$
    * $\frac{2}{5} (0)$
    * $0$

---

## Example 5

5. Evaluate $\limit{x}{0} \frac{x \cos 2x - x}{8x}$
    * $\limit{x}{0} \frac{x (\cos 2x - 1)}{4(2x)}$
    * $\limit{x}{0} \frac{x}{4} \limit{x}{0} \frac{\cos 2x - 1}{2x}$
    * $0 \limit{x}{0} \frac{x}{4}$ 
    * $0$ 

---

## Exercise for Readers

* Evaluate the following:
    * $\limit{x}{0} \frac{\sin 4x}{4x}$
    * $\limit{x}{0} \frac{2 - 2\cos x}{x}$
    * $\limit{\theta}{0} \frac{\sin 4\theta}{\sin 3\theta}$

---

## Exercise for Readers

* Evaluate the following:
    * $\limit{x}{0} \frac{\sin 3x}{3x^2 + x}$
    * $\limit{\theta}{0} \frac{1 - \cos 2\theta}{\theta}$
    * $\limit{x}{0} \frac{5 \tan x - 5 \sin x}{x \cos x}$

---

# [Next Lesson](Lesson%202)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Evaluate $\limit{x}{0} \frac{\sin 4x}{4x}$
    * $1$
* Evaluate $\limit{x}{0} \frac{2 - 2\cos x}{x}$
    * $\limit{x}{0} \frac{2(1 - \cos x)}{x}$
    * $-2 \limit{x}{0} \frac{\cos x - 1}{x} = -2(0)$
    * $0$

---

## Answers to Exercises, cont.

* Evaluate $\limit{\theta}{0} \frac{\sin 4\theta}{\sin 3\theta}$
    * $\limit{\theta}{0} \frac{(4\theta)(3\theta)\sin 4\theta}{(4\theta)(3\theta) \sin 3\theta}$
    * $\limit{\theta}{0} \frac{\sin 4\theta}{4\theta} \limit{\theta}{0} \frac{4\theta}{3\theta} \limit{\theta}{0} \frac{3\theta}{\sin 3\theta}$
    * $\frac{4}{3}$

---

## Answers to Exercises, cont.

* Evaluate $\limit{x}{0} \frac{\sin 3x}{3x^2 + x}$
    * $\limit{x}{0} \frac{\sin 3x}{x(3x + 1)}$
    * $\limit{x}{0} \frac{3\sin 3x}{3x(3x + 1)}$
    * $\limit{x}{0} \frac{3}{3x + 1} \limit{x}{0} \frac{\sin 3x}{3x}$
    * $\limit{x}{0} \frac{3}{3x + 1}$

---

## Answers to Exercises, cont.

* Evaluate $\limit{x}{0} \frac{\sin 3x}{3x^2 + x}$
    * $\limit{x}{0} \frac{3}{3x + 1}$
    * $\frac{3}{3(0) + 1}$
    * $\frac{3}{1}$
    * $3$


---

## Answers to Exercises, cont.

* Evaluate $\limit{\theta}{0} \frac{1 - \cos 2\theta}{\theta}$
    * $\limit{\theta}{0} \frac{2(1 - \cos 2\theta)}{2\theta}$
    * $-2\limit{\theta}{0} \frac{\cos 2\theta - 1}{2\theta} = -2(0)$
    * $0$

---

## Answers to Exercises, cont.

* Evaluate $\limit{x}{0} \frac{5 \tan x - 5 \sin x}{x \cos x}$
    * $\limit{x}{0} \frac{5 (\tan x - \sin x)}{x \cos x}$
    * $\limit{x}{0} \frac{5\sin x (\sec x - 1)}{x \cos x}$
    * $5\limit{x}{0} \frac{\sin x}{\cos x} \limit{x}{0} \frac{\sec x - 1}{x}$
    * $5\frac{\sin 0}{\cos 0} \limit{x}{0} (\frac{1}{\cos x} - 1) / x$, $\sin 0 = 0$, $\cos 0 = 1$
    * $0$

---

# [Next Lesson](Lesson%202)
