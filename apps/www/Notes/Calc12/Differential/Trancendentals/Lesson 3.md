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
$\newcommand\pfrac[1]{\frac{\pi}{#1}}$

---

# Lesson 3: Trigonometric Differentiation II

---

<!--paginate: true-->

## Intro

* For this unit, all six of the previous rules (Constant, Power, Sum / Difference, Product, Quotient and Chain) are used in the same way as elementary functions.
* The only additional rules needed are the derivatives for specific transcendental functions.
* We started by deriving rules 7 and 8: The Sine and Cosine Rules.
* Now, let's derive the remaining Trigonometric functions.

---

## Derivative of $\tan x$

* Consider $f(x) = \tan x$
* $f(x) = \frac{\sin x}{\cos x}$
    * $g(x) = \sin x$
    * $h(x) = \cos x$
    * $\diff{x} f(x) = \frac{(\cos x)(\diff{x} (\sin x)) - (\sin x) (\diff{x} \cos(x))}{(\cos x)^2}$
    * $f'(x) = \frac{(\cos x)(\cos x) - (\sin x)(-\sin(x))}{\cos^2 x}$
    * $f'(x) = \frac{\cos^2 x + \sin^2 x}{\cos^2 x}$
    * $f'(x) = \frac{1}{\cos^2 x}$
* $f'(x) = \sec^2 x$

---

## Derivative of $\cot x$

* Consider $f(x) = \cot x$
* $f(x) = \frac{\cos x}{\sin x}$
    * $g(x) = \cos x$
    * $h(x) = \sin x$
    * $\diff{x} f(x) = \frac{(\sin x)(\diff{x} (\cos x)) - (\cos x) (\diff{x} \sin(x))}{(\sin x)^2}$
    * $f'(x) = \frac{(\sin x)(-\sin x) - (\cos x)(\cos x)}{\sin^2 x}$
    * $f'(x) = \frac{- \sin^2 x - \cos^2 x}{\sin^2 x}$
    * $f'(x) = -\frac{1}{\sin^2 x}$
* $f'(x) = -\csc^2 x$

---

## Derivative of $\sec x$

* Consider $f(x) = \sec x$
* $f(x) = \frac{1}{\cos x} = (\cos x)^{-1}$
    * $y = u^{-1}$
    * $u = \cos x$
    * $\diff{x} f(x) = \diff{u} u^{-1} (\diff{x} \cos x)$
    * $f'(x) = -(\cos x)^{-2} (-\sin x)$
    * $f'(x) = \frac{\sin x}{\cos^2 x}$
    * $f'(x) = \frac{\sin x}{\cos x}\sec x$
* $f'(x) = \tan x \sec x$

---

## Derivative of $\csc x$

* Consider $f(x) = \csc x$
* $f(x) = \frac{1}{\sin x} = (\sin x)^{-1}$
    * $y = u^{-1}$
    * $u = \sin x$
    * $\diff{x} f(x) = \diff{u} u^{-1} (\diff{x} \sin x)$
    * $f'(x) = -(\sin x)^{-2} (\cos x)$
    * $f'(x) = -\frac{\cos x}{\sin^2 x}$
    * $f'(x) = -\frac{\cos x}{\sin x}\csc x$
* $f'(x) = -\cot x \csc x$

---

## Trigonometric Derivatives

* Here's all of the trigonometric derivatives:
    * Sine: $\diff{x} \sin x = \cos x$
    * Cosine: $\diff{x} \cos x = \sin x$
    * Tangent: $\diff{x} \tan x = \sec^2 x$
    * Cotangent: $\diff{x} \cot x = -\csc^2 x$
    * Secant: $\diff{x} \sec x = \tan x \sec x$
    * Cosecant: $\diff{x} \csc x = -\cot x \csc x$
* While the first two are the only fundamental ones, all six should be known at the very least. 
* Now, let's use these, shall we?

---

## Example 1

1. Differentiate $y = 2 \sec 3x$
    * $y = 2 \sec 3x$
    * $u = 2 \sec v$
    * $v = 3x$
    * $\diff{x} y = \diff{v} 2 \sec v (\diff{x} 3x)$
    * $\dd[y]{x} = 2 \tan v \sec v (3)$
* $\dd[y]{x} = 6 \tan 3x \sec 3x$

---

## Example 2

2. Differentiate $f(x) = \sin 2x \tan x$
    * $g(x) = \sin 2x$
    * $h(x) = \tan x$
    * $y = \sin u$
    * $u = 2x$
    * $\diff{x} f(x) = (\sin 2x) [\diff{x} (\tan x)] + (\tan x) [\diff{u} \sin u (\diff{x} 2x)]$
    * $f'(x) = (\sin 2x)(\sec^2 x) + (\tan x) (2 \cos 2x)$
* $f'(x) = \sin 2x \sec^2 x + 2 \tan x \cos 2x$

---

## Example 3

3. Differentiate $f(x) = \frac{\cot 5x}{\csc^2 4x}$
    * $g(x) = \cot 5x$
    * $h(x) = (\csc 4x)^2$
    * $y = u^2$
    * $u = \csc v$
    * $v = 4x$
    * $m = \cot n$
    * $n = 5x$
    * $\diff{x} f(x) = \frac{(\csc^2 4x) [\diff{n} \cot n (\diff{x} 5x)] - \cot 5x [\diff{u} u^2 (\diff{v} \csc v)(\diff{x} 4x)]}{(\csc^2 4x)^2}$

---

## Example 3

3. Differentiate $f(x) = \frac{\cot 5x}{\csc^2 4x}$
    * $u = \csc v$
    * $v = 4x$
    * $n = 5x$
    * $\diff{x} f(x) = \frac{(\csc^2 4x) [\diff{n} \cot n (\diff{x} 5x)] - \cot 5x [\diff{u} u^2 (\diff{v} \csc v)(\diff{x} 4x)]}{(\csc^2 4x)^2}$
    * $f'(x) = \frac{-5(\csc^2 4x)(\csc^2 5x) - \cot 5x [-8(\cot 4x \csc^2 4x)]}{\csc^4 4x}$
    * $f'(x) = \frac{\csc^2 4x[8 \cot 5x \cot 4x - 5\csc^2 5x)}{\csc^4 4x}$
* $f'(x) = \frac{8 \cot 5x \cot 4x - 5\csc^2 5x}{\csc^2 4x}$

---

## Exercise for Readers

* Differentiate the following:
    * $f(x) = 2 \cot 2x$
    * $y = \sin x \sec 2x$
    * $f(x) = \frac{\tan (5x - 4)}{\cos (x^2)}$
    * $y = \csc^3 (3x^2)$

---

# [Practice Quiz](Quiz)

Or

# [Next Lesson](Lesson%204)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercise

* Differentiate $f(x) = 2 \cot 2x$
    * $y = 2u$
    * $u = \cot v$
    * $v = 2x$
    * $\diff{x} f(x) = \diff{u} 2u (\diff{v} \cot v)(\diff{x} 2x)$
    * $f'(x) = -4 (\csc^2 v)$
    * $f'(x) = -4 \csc^2 (2x)$

---

## Answers to Exercise, cont.

* Differentiate $y = \sin x \sec 2x$
    * $g(x) = \sin x$
    * $h(x) = \sec 2x$
    * $u = \sec v$
    * $v = 2x$
    * $\diff{x} y = (\sin x) [\diff{v} \sec v (\diff{x} 2x)] + (\sec 2x) [\diff{x} (\sin x)]$
    * $\dd[y]{x} = (\sin x) [2\tan 2x \sec 2x] + (\sec 2x)(\cos x)$
    * $\dd[y]{x} = \sec 2x[2 \sin x \tan 2x + \cos x]$

---

## Answers to Exercise, cont.

* Differentiate $f(x) = \frac{\tan (5x - 4)}{\cos (x^2)}$
    * $g(x) = \tan (5x - 4)$
    * $h(x) = \sec (x^2)$
    * $y = \tan u$
    * $u = 5x - 4$
    * $\theta = x^2$
    * $r = \sec \theta$
    * $\diff{x} f(x) = \tan(5x - 4) [\diff{\theta} \sec \theta (\diff{x} x^2)] +$ 
    $\sec(x^2) (\diff{u} \tan u [\diff{x} (5x - 4)])$

---

## Answers to Exercise, cont.

* Differentiate $f(x) = \frac{\tan (5x - 4)}{\cos (x^2)}$
    * $u = 5x - 4$
    * $\theta = x^2$
    * $\diff{x} f(x) = \tan(5x - 4) [\diff{\theta} \sec \theta (\diff{x} x^2)] +$ 
    $\sec(x^2) (\diff{u} \tan u [\diff{x} (5x - 4)])$
    * $\diff{x} f(x) = \tan(5x - 4) [\diff{\theta} \sec \theta (\diff{x} x^2)] +$ 
    $\sec(x^2) (\diff{u} \tan u [\diff{x} (5x) - \diff{x} (4)])$
    * $f'(x) = \tan(5x - 4) [2x \tan \theta \sec \theta] + 5\sec(x^2)\sec^2 u$

---

## Answers to Exercise, cont.

* Differentiate $f(x) = \frac{\tan (5x - 4)}{\cos (x^2)}$
    * $u = 5x - 4$
    * $\theta = x^2$
    * $f'(x) = \tan(5x - 4) [2x \tan \theta \sec \theta] + 5\sec(x^2)\sec^2 u$
    * $f'(x) = 2x\tan(5x - 4)\tan(x^2) \sec(x^2) +$ 
    $5\sec(x^2)\sec^2 (5x - 4)$
    * $f'(x) = \sec(x^2) [2x\tan(5x - 4)\tan(x^2) + 5\sec^2 (5x - 4)]$
    * $f'(x) = \frac{2x\tan(5x - 4)\tan(x^2) + 5\sec^2 (5x - 4)}{\cos (x^2)}$

---

## Answers to Exercise, cont.

* Differentiate $y = \csc^3 (3x^2)$
    * $u = v^3$
    * $v = \csc \theta$
    * $\theta = 3x^2$
    * $\diff{x} y = \diff{v} v^3 (\diff{\theta} \csc \theta)(\diff{x} 3x^2)$
    * $\dd[y]{x} = 3v^2 (-\cot \theta \csc \theta)(6x)$
    * $\dd[y]{x} = -18x \csc^3(3x^2) \cot (3x^2)$

---

# [Practice Quiz](Quiz)

Or

# [Next Lesson](Lesson%204)