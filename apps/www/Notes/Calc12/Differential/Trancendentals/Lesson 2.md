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

# Lesson 2: Trigonometric Differentiation I

---

<!--paginate: true-->

## Intro

* In the previous unit, you learned how to calculate the **Derivative** using six differentiation rules:
    * Constant: $\diff{x} c = 0$
    * Power: $\diff{x} x^n = nx^{n - 1}$
    * Sum / Difference: $\diff{x} [f(x) \pm g(x)] = \diff{x} [f(x)] \pm \diff{x} [g(x)]$
    * Product: $\diff{x} [f(x)g(x)] = f(x) [\diff{x} g(x)] + g(x) [\diff{x} f(x)]$
    * Quotient: $\diff{x} f(x) = \frac{h(x) (\diff{x} g(x)) - g(x) (\diff{x} h(x))}{(h(x))^2}$
    * Chain: $\diff{x} f(x) = \diff{x} g(h(x)) [\diff{x} h(x)]$ or $\diff{x} y = \diff{u} y (\diff{x} u)$

---

## Intro, cont.

* For this unit, all six of the previous rules (Constant, Power, Sum / Difference, Product, Quotient and Chain) are used in the same way as elementary functions.
* The only additional rules needed are the derivatives for specific transcendental functions.
* We'll start by deriving rules 7 and 8: The Sine and Cosine Rules.
* For these, we'll need some Trigonometric Identities and The Trigonometric Limits (from Lesson 1)

---

## Deriving the Derivative of Sine

* Consider $f(x) = \sin x$.
* Let's use first principles to find this derivative: $\diff{x} f(x) = \limit{h}{0} \frac{f(x + h) - f(x)}{h}$
    * $f'(x) = \limit{h}{0} \frac{\sin (x + h) - \sin x}{h}$
* Sine Sum / Difference Identity: $\sin (A \pm B) = \sin A \cos B \pm \cos A \sin B$
    * $f'(x) = \limit{h}{0} \frac{\sin x \cos h + \cos x \sin h - \sin x}{h}$

---

## Deriving the Derivative of Sine, cont.

* Here's what we have:
    * $f'(x) = \limit{h}{0} \frac{\sin x \cos h + \cos x \sin h - \sin x}{h}$
    * $f'(x) = \limit{h}{0} \frac{\sin x \cos h - \sin x + \cos x \sin h}{h}$
    * $f'(x) = \limit{h}{0} \frac{\sin x( \cos h - 1) + \cos x \sin h}{h}$

---

## Deriving the Derivative of Sine, cont.

* $f'(x) = \limit{h}{0} \frac{\sin x( \cos h - 1) + \cos x \sin h}{h}$
* $f'(x) = \limit{h}{0} \sin x \frac{\cos h - 1}{h} + \limit{h}{0} \cos x \frac{\sin h}{h}$
* $f'(x) = \sin x \limit{h}{0} \frac{\cos h - 1}{h} + \cos x \limit{h}{0} \frac{\sin h}{h}$

---

## Deriving the Derivative of Sine, cont.

* $f'(x) = \sin x \limit{h}{0} \frac{\cos h - 1}{h} + \cos x \limit{h}{0} \frac{\sin h}{h}$
* $\limit{x}{0} \frac{\sin x}{x} = 1$, $\limit{x}{0} \frac{\cos x - 1}{x} = 0$
* $f'(x) = \sin x (0) + \cos x$
* $f'(x) = \cos x$
* $\therefore \diff{x} (\sin x) = \cos x$
* $\diff{x} \sin u = \cos u (\diff{x} u)$, by chain rule.

---

## Deriving the Derivative of Cosine

* Consider $f(x) = \cos x$, we can use a complimentary angle identity and $\diff{x} \sin x$.
* Complimentary Angle Identities: 
    * $\cos x = \sin(\pfrac{2} - x)$
    * $\sin x = \cos(\pfrac{2} - x)$
    * *This is also why* $\cos \pfrac{4} = \sin \pfrac{4}$
* $y = \cos x = \sin(\pfrac{2} - x)$
* $\diff{x} y = \diff{x} \sin(\pfrac{2} - x)$
* $\dd[y]{x} = \cos(\pfrac{2} - x)(-1)$

---

## Deriving the Derivative of Cosine, cont.

* $\dd[y]{x} = \cos(\pfrac{2} - x)(-1)$
* $\dd[y]{x} = -\cos(\pfrac{2} - x)$
* Using Complimentary Angle Identity:
    * $\dd[y]{x} = -\sin x$
* $\therefore \diff{x} \cos x = -\sin x$
* $\diff{x} \cos u = -\sin u (\diff{x} u)$, by chain rule.

---

## Example 1

1. Find the derivative of $y = 3 \sin x$
    * $\diff{x} y = \diff{x} (3 \sin x)$
    * $\dd[y]{x} = 3 \cos x$

---

## Example 2

2. Differentiate $y = -2 \sin 5x$
    * $u = 5x$
    * $\diff{x} y = \diff{u} (-2 \sin u) (\diff{x} 5x)$
    * $\dd[y]{x} = -2 \cos 5x (5)$
    * $\dd[y]{x} = -10 \cos 5x$

---

## Example 3

3. Differentiate $f(x) = 4 \sin x$ and find the slope of the tangent line at $x = \pfrac{6}$
    * $\diff{x} f(x) = \diff{x} (4 \sin x)$
    * $f'(x) = 4 \cos x$
    * $f'(\pfrac{6}) = 4 \cos \pfrac{6}$
    * $f'(\pfrac{6}) = 4\frac{\sqrt{3}}{2}$
    * $f'(\pfrac{6}) = 2\sqrt{3}$

---

## Example 4

4. Differentiate $f(x) = \sin x \cos x$ and find the slope of the tangent line at $x = \pfrac{3}$
    * $g(x) = \sin x$
    * $h(x) = \cos x$
    * $\diff{x} f(x) = (\sin x) [\diff{x} \cos x] + (\cos x) [\diff{x} \sin x]$
    * $f'(x) = (\sin x)(-\sin x) + (\cos x) (\cos x)$
    * $f'(x) = -\sin^2 x + \cos^2 x$
    * $f'(x) = \cos^2 x - \sin^2 x$
    * $f'(x) = \cos 2x$

---

## Example 4, cont.

4. Differentiate $f(x) = \sin x \cos x$ and find the slope of the tangent line at $x = \pfrac{3}$
    * $f'(x) = \cos 2x$
    * $f'(\pfrac{3}) = \cos (\frac{2\pi}{3})$
    * $f'(\pfrac{3}) = -\frac{1}{2}$

---

## Example 5

5. Differentiate $f(x) = \frac{\sin 3x}{\cos(x^2)}$
    * $g(x) = \sin 3x$
    * $u = 3x$
    * $h(x) = \cos x^2$
    * $v = x^2$
    * $\diff{x} f(x) = \frac{[\cos (x^2)] [\diff{u} \sin u (\diff{x} 3x)] - (\sin 3x) [\diff{x} h(x) = \diff{v} \cos v (\diff{x} x^2)]}{[\cos (x^2)]^2}$
    * $f'(x) = \frac{[\cos (x^2)] [3\cos u] - (\sin 3x) [-2x \sin v]}{\cos^2 (x^2)}$
    * $f'(x) = \frac{3\cos (x^2) \cos 3x + 2x\sin 3x \sin (x^2)}{\cos^2 (x^2)}$

---

## Example 6

6. Differentiate $f(x) = 4 \sin^2 (x^2 + 2)$
    * $f(x) = 4[\sin (x^2 + 2)]^2$
    * $y = 4u^2$
    * $u = \sin v$
    * $v = x^2 + 2$
    * $\diff{x} f(x) = \diff{u} 4u^2 (\diff{v} \sin v)(\diff{x} x^2 + 2)$
    * $\diff{x} f(x) = \diff{u} 4u^2 (\diff{v} \sin v)[\diff{x} (x^2) + \diff{x} (2)]$
    * $f'(x) = 4(2u)(\cos v)2x$
    * $f'(x) = 8x(2\sin v \cos v)$

---

## Example 6, cont.

6. Differentiate $f(x) = 4 \sin^2 (x^2 + 2)$
    * $v = x^2 + 2$
    * $f'(x) = 8x(2\sin v \cos v)$
    * $\sin 2a = 2\sin a \cos a$
    * $f'(x) = 8x\sin 2v$
    * $f'(x) = 8x[\sin 2(x^2 + 2)]$

---

## Example 7

7. Differentiate $f(x) = 3x^2 \cos^2 (2x)$ using Product and Chain Rule
    * $g(x) = 3x^2$
    * $h(x) = (\cos 2x)^2$
    * $y = u^2$
    * $u = \cos v$
    * $v = 2x$
    * $\diff{x} f(x) = (3x^2) [\diff{u} u^2 (\diff{v} \cos v)(\diff{x} 2x)] + (\cos 2x)^2 [\diff{x} (3x^2)]$
    * $f'(x) = (3x^2) [2u (-\sin v)(2)] + 6x(\cos 2x)^2$


---

## Example 7

7. Differentiate $f(x) = 3x^2 \cos^2 (2x)$ using Product and Chain Rule
    * $u = \cos v$
    * $v = 2x$
    * $f'(x) = (3x^2) [2u (-\sin v)(2)] + 6x(\cos 2x)^2$
    * $f'(x) = (3x^2) [-4 \cos v \sin v] + 6x(\cos 2x)^2$
    * $f'(x) = (3x^2) [-2 \sin 2(2x)] + 6x(\cos 2x)^2$
    * $f'(x) = -2(3x^2)\sin 4x + 6x(\cos 2x)^2$
    * $f'(x) = 6x \cos^2 2x - 6x^2 \sin 4x$

---

## Differentiation Laws

1. Constant: $\diff{x} c = 0$
2. Power: $\diff{x} x^n = nx^{n - 1}$
3. Sum / Difference: $\diff{x} [f(x) \pm g(x)] = \diff{x} [f(x)] \pm \diff{x} [g(x)]$
4. Product: $\diff{x} f(x) = g(x) [\diff{x} h(x)] + h(x) [\diff{x} g(x)]$
5. Quotient: $\diff{x} f(x) = \frac{h(x) (\diff{x} g(x)) - g(x) (\diff{x} h(x))}{(h(x))^2}$
6. Chain: $\diff{x} f(x) = \diff{x} g(h(x)) [\diff{x} h(x)]$ or $\diff{x} y = \diff{u} y (\diff{x} u)$
7. Sine: $\diff{x} \sin x = \cos x$
8. Cosine: $\diff{x} \cos x = \sin x$
9-10. Lessons 4 & 5

---

## Exercise for Readers

* Differentiate the Following:
    * $y = 4 \cos x$
    * $f(x) = 3 \sin (5x^2)$
    * $y = \frac{\sin^2 x}{\cos 2x}$
    * $f(x) = -2 \cos^3 7x$
* Find the slope of the tangent:
    * $y = \cos^2 (2x)$, $x = \pfrac{2}$

---

# [Next Lesson](Lesson%203)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Differentiate $y = 4 \cos x$
    * $\diff{x} y = \diff{x} 4 \cos x$
    * $\dd[y]{x} = -4 \sin x$
* Differentiate $f(x) = 3 \sin (5x^2)$
    * $y = 3 \sin u$
    * $u = 5x^2$
    * $\diff{x} f(x) = \diff{u} 3 \sin u (\diff{x} 5x^2)$
    * $f'(x) = 3 \cos u (10x)$
    * $f'(x) = 30x \cos (5x^2)$

---

## Answers to Exercises, cont.

* Differentiate $y = \frac{\sin^2 x}{\cos 2x}$
    * $g(x) = (\sin x)^2$
    * $h(x) = \cos 2x$
    * $u = v^2$
    * $v = \sin x$
    * $w = \cos \theta$
    * $\theta = 2x$
    * $\diff{x} f(x) = \frac{(\cos 2x) [\diff{v} v^2 (\diff{x} \sin x)] - (\sin^2 x)[\diff{\theta} \cos \theta (\diff{x} 2x)]}{(\cos 2x)^2}$

---

## Answers to Exercises, cont.

* Differentiate $y = \frac{\sin^2 x}{\cos 2x}$
    * $v = \sin x$
    * $\theta = 2x$
    * $\diff{x} y = \frac{(\cos 2x) [\diff{v} v^2 (\diff{x} \sin x)] - (\sin^2 x)[\diff{\theta} \cos \theta (\diff{x} 2x)]}{(\cos 2x)^2}$
    * $\dd[y]{x} = \frac{(\cos 2x) [2v (\cos x)] - (\sin^2 x)[-2\sin \theta]}{(\cos 2x)^2}$
    * $\dd[y]{x} = \frac{(\cos 2x) [2\sin x(\cos x)] - (\sin^2 x)[-2\sin 2x]}{(\cos 2x)^2}$
    
---

## Answers to Exercises, cont.

* Differentiate $y = \frac{\sin^2 x}{\cos 2x}$
    * $\dd[y]{x} = \frac{(\cos 2x) [2\sin x(\cos x)] - (\sin^2 x)[-2\sin 2x]}{(\cos 2x)^2}$
    * $\dd[y]{x} = \frac{(\cos 2x)\sin 2x + 2(\sin^2 x)\sin 2x}{(\cos 2x)^2}$
    * $\dd[y]{x} = \frac{\sin 2x[(\cos 2x) + 2\sin^2 x]}{(\cos 2x)^2}$
    
---

## Answers to Exercises, cont.

* Differentiate $y = \frac{\sin^2 x}{\cos 2x}$
    * $\dd[y]{x} = \frac{\sin 2x[(\cos 2x) + 2\sin^2 x]}{(\cos 2x)^2}$
    * $\dd[y]{x} = \frac{\sin 2x}{\cos 2x} \frac{\cos 2x + 2\sin^2 x}{\cos 2x}$
    * $\dd[y]{x} = \tan 2x \frac{\cos^2 x - \sin^2 x + 2\sin^2 x}{\cos 2x}$
    * $\dd[y]{x} = \tan 2x \frac{\cos^2 x + \sin^2 x}{\cos 2x}$
    

---

## Answers to Exercises, cont.

* Differentiate $y = \frac{\sin^2 x}{\cos 2x}$
    * $\dd[y]{x} = \tan 2x \frac{\cos^2 x + \sin^2 x}{\cos 2x}$
    * $\dd[y]{x} = \tan 2x \frac{1}{\cos 2x}$
    * $\dd[y]{x} = \tan 2x \sec 2x$

---

## Answers to Exercises, cont.

* Differentiate $f(x) = -2 \cos^3 7x$
    * $y = -2u^3$
    * $u = \cos v$
    * $v = 7x$
    * $\diff{x} f(x) = \diff{u} (-2u^3) (\diff{v} \cos v)(\diff{x} 7x)$
    * $f'(x) = 6u^2(\sin v)(7)$
    * $f'(x) = 42\sin 7x \cos^2 (7x)$
    * $f'(x) = 42\sin 7x \cos 7x (\cos 7x)$
    * $f'(x) = 21\sin 14x \cos 7x$

---

## Answers to Exercises, cont.

* Find the slope of the tangent line: $y = \cos^2 (2x)$, $x = \pfrac{2}$
    * $u = v^2$
    * $v = \cos w$
    * $w = 2x$
    * $\diff{x} y = \diff{v} v^2 (\diff{w} \cos w)(\diff{x} 2x)$
    * $\diff{x} y = 2v (-\sin w)(2)$
    * $\diff{x} y = -4(\cos w)(\sin w)$
    * $\diff{x} y = -2\sin 4x$

---

## Answers to Exercises, cont.

* Find the slope of the tangent line: $y = \cos^2 (2x)$, $x = \pfrac{2}$
    * $m = -2\sin 4x$
    * $m = -2 \sin 4(\pfrac{2})$
    * $m = -2 \sin (2\pi)$
    * $m = -2 (0)$
    * $m = 0$

---

# [Next Lesson](Lesson%203)