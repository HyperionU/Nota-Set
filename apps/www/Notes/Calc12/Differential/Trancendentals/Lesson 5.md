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

# Lesson 5: Exponential and Logarithmic Derivatives II

---

<!--paginate: true-->

## Intro

* For this unit, all six of the previous rules (Constant, Power, Sum / Difference, Product, Quotient and Chain) are used in the same way as elementary functions.
* The only additional rules needed are the derivatives for specific transcendental functions.
* Previously, we looked at a special case for logarithms with a base of $e$ (The Natural Logarithm).
* Now, we'll derive the actual Logarithm Rule, as well as its inverse: The Exponential Rule, and look at another special case.

---

## Why Start with $\ln x$?

* There's a reason why we learned the derivative of the natural log first.
* We actually need it, alongside our other rules to derive the Exponential Rule and the general Logarithm Rule.
* Now, let's start by deriving the Exponential Rule.

---

## Deriving the Exponential Rule

* Recall that an exponential can be written as follows:
    * $y = b^x$, $b > 1$, $b \in \mathbb{R}$
* Consider some general exponential $y = b^x$
* Take the natural log of both sides.
    * $\ln y = \ln b^x$
* Using $n \ln A = \ln A^n$:
    * $\ln y = x \ln b$
* Differentiate both sides.
    * $\diff{} (\ln y) = \diff{} (x \ln b)$
    * $\frac{1}{y}(dy) = \diff{} (x \ln b)$

---

## Deriving the Exponential Rule

* We have this:
    * $\ln y = x \ln b$
* Differentiate both sides.
    * $\diff{} (\ln y) = \diff{} (x \ln b)$
    * $\frac{1}{y}(dy) = dx(\ln b)$
* Isolate $\dd[y]{x}$
    * $\dd[y]{x} = \frac{(\ln b)}{\frac{1}{y}}$

---

## Deriving the Exponential Rule

* We have this:
    * $\dd[y]{x} = \frac{(\ln b)}{\frac{1}{y}}$
    * $\dd[y]{x} = y(\ln b)$
* Recall $y = b^x$
    * $\dd[y]{x} = b^x \ln b$

---

## The Exponental Rule

$\diff{x} (b^x) = b^x \ln b$

* By the chain rule: $\diff{x} (b^u) = b^u \ln b \dd[u]{x}$
* With this, we can find the derivative of all exponential functions.
* This works for all prior differentiation rules. (Constant, Power, Sum / Difference, Product, Quotient, Chain)
* Now, let's test it, shall we?

---

## Example 1

1. Differentiate $y = 6^x$
    * $\diff{x} y = \diff{x} 6^x$
    * $\dd[y]{x} = 6^x \ln 6$
* It's important to note, $\ln b$ is a constant, and should be treated as such.

---

## Example 2

2. Differentiate $y = (5x)2^x$
    * $g(x) = 5x$
    * $h(x) = 2^x$
    * $\diff{x} y = (5x) [\diff{x} (2^x)] + (2^x) [\diff{x} (5x)]$
    * $\dd[y]{x} = (5x)2^x \ln 2 + (2^x) (5)$
    * $\dd[y]{x} = 5(2^x)[x \ln 2 + 1]$

---

## Example 3

3. Differentiate $f(x) = \frac{3x^2}{4^x}$
    * $g(x) = 3x^2$
    * $h(x) = 4^x$
    * $\diff{x} f(x) = \frac{(4^x) [\diff{x} (3x^2)] - (3x^2) [\diff{x} (4^x)]}{(4^x)^2}$
    * $f'(x) = \frac{(4^x)(6x) - (3x^2) (4^x)\ln 4}{4^2x}$
    * $f'(x) = \frac{3x(4^x)[2 - x \ln 4]}{4^2x}$
    * $f'(x) = \frac{3x(2 - x \ln 4)}{4^x}$

---

## Example 4

4. Differentiate $y = 2(3^{6x^2 - x})$
    * $y = 2(3^u)$
    * $u = 6x^2 - x$
    * $\diff{x} y = \diff{u} 2(3^u) [\diff{x} (6x^2 - x)]$
    * $\diff{x} y = 2\diff{u} (3^u) [\diff{x} (6x^2) - \diff{x} (x)]$
    * $\dd[y]{x} = 2(3^u)\ln 3(12x - 1)$

---

## Exponential's Special Case: $e^x$

* There's two ways to determine the derivative of $e^x$. Here's both.
* Consider $y = e^x$
* Method 1: Logarithms
    * $\ln y = \ln e^x$
    * Using $n \ln A = \ln A^n$:
        * $\ln y = x \ln e$
    * $\ln e = 1$
        * $\ln y = x$

---

## Exponential's Special Case, cont.

* Method 1: Logarithms
    * We have this:
        * $\ln y = x$
    * Differentiate both sides.
        * $\diff{} (\ln y) = \diff{} (x)$
        * $\frac{1}{y}(dy) = dx$
        * $dy = \frac{dx}{\frac{1}{y}}$
        * $dy = y(dx)$

---

## Exponential's Special Case, cont.

* Method 1: Logarithms
    * We have this:
        * $dy = y(dx)$
        * $\dd[y]{x} = y$
    * Recall $y = e^x$
        * $\dd[y]{x} = e^x$

---

## Exponential's Special Case, cont.

* Method 2: Exponental Rule
    * Consider $y = e^x$
    * Differentiate both sides.
        * $\diff{x} y = \diff{x} (e^x)$
        * $\dd[y]{x} = (e^x)\ln e$  
    * $\ln e = 1$
        * $\dd[y]{x} = e^x$     

---

## Derivative of $e^x$

$\diff{x} (e^x) = e^x$

* By the chain rule: $\diff{x} (e^u) = e^u \dd[u]{x}$
* This means that $e^x$ is its own derivative!
* This is an important property which is exclusive only to $e^x$.
* This is also why we use $\ln x$.
* Let's try this out, shall we?

---

## Example 5

5. Differentiate $y = e^{2x}$
    * $y = e^u$
    * $u = 2x$
    * $\diff{x} y = \diff{u} (e^u) \diff{x} (2x)$
    * $\dd[y]{x} = (e^u)(2)$
    * $\dd[y]{x} = 2(e^{2x})$

---

## Example 6

6. Differentiate $y = e^{6x^3 - 7x}$
    * $y = e^u$
    * $u = 6x^3 - 7x$
    * $\diff{x} y = \diff{u} (e^u) [\diff{x} (6x^3 - 7x)]$
    * $\diff{x} y = \diff{u} (e^u) [\diff{x} (6x^3) - \diff{x} (7x)]$
    * $\dd[y]{x} = (e^{6x^3 - 7x})(18x^2 - 7)$

---

## Example 7

7. Differentiate $y = 5(2^{4x^3 - x^2})$
* Method 1: Logarithms
    * $\ln y = \ln [5(2^{4x^3 - x^2})]$
    * $\ln y = \ln 5 + \ln (2^{4x^3 - x^2})$
    * $\ln y = \ln 5 + (4x^3 - x^2) \ln 2$
    * $\ln y = \ln 5 + 4x^3 \ln 2 - x^2 \ln 2$
    * $\diff{} (\ln y) = \diff{} (\ln 5 + 4x^3 \ln 2 - x^2 \ln 2)$
    * $\diff{} (\ln y) = \diff{} (\ln 5) + \diff{} (4x^3 \ln 2) - \diff{} (x^2 \ln 2)$
    * $\frac{1}{y} dy = (12x^2 \ln 2)dx - (2x \ln 2)dx$


---

## Example 7, cont.

7. Differentiate $y = 5(2^{4x^3 - x^2})$
* Method 1: Logarithms
    * $\frac{1}{y} dy = (12x^2 \ln 2)dx - (2x \ln 2)dx$
    * $\frac{1}{y} dy = \ln 2(dx)(12x^2 - 2x)$
    * $dy = \frac{\ln 2(dx)(12x^2 - 2x)}{\frac{1}{y}}$
    * $\dd[y]{x} = y\ln 2(12x^2 - 2x)$
    * $\dd[y]{x} = 5(2^{4x^3 - x^2})\ln 2(12x^2 - 2x)$

---

## Example 7, cont.

7. Differentiate $y = 5(2^{4x^3 - x^2})$
* Method 1: Logarithms
    * $\dd[y]{x} = 5(2^{4x^3 - x^2})\ln 2(12x^2 - 2x)$
    * $\dd[y]{x} = 5(2^{4x^3 - x^2})(2x\ln 2)(6x - 1)$

---

## Example 7, cont.

7. Differentiate $y = 5(2^{4x^3 - x^2})$
* Method 2: Exponential Rule
    * $y = 5(2^u)$
    * $u = 4x^3 - x^2$
    * $\diff{x} y = \diff{u} 5(2^u) [\diff{x} (4x^3 - x^2)]$
    * $\diff{x} y = 5 \diff{u} (2^u) [\diff{x} (4x^3) - \diff{x} (x^2)]$
    * $\dd[y]{x} = 5(2^{4x^3 - x^2})(\ln 2)(12x^2 - 2x)$
    * $\dd[y]{x} = 5(2^{4x^3 - x^2})(2x \ln 2)(6x - 1)$

---

## The General Logarithm Rule

* A logarithm written in the form $y = \log_b x$ can be rewritten in its exponential form.
    * $b^y = b^{\log_b x}$
    * $x = b^y$
* Take the Natural Logarithm.
    * $\ln x = \ln b^y$
* Using $n \ln A = \ln A^n$:
    * $\ln x = y \ln b$
* Differentiate both sides.
    * $\diff{} (\ln x) = \diff{} (y \ln b)$

---

## The General Logarithm Rule, cont.

* We have this:
    * $\ln x = y \ln b$
* Differentiate both sides.
    * $\diff{} (\ln x) = \diff{} (y \ln b)$
    * $\frac{1}{x} dx = (dy) \ln b$
    * $\frac{1}{x \ln b} = \dd[y]{x}$
    * $\dd[y]{x} = \frac{1}{x \ln b}$
    
---

## The Logarithm Rule

$\diff{x} (\log_b x) = \frac{1}{x \ln b}$

* By the chain rule: $\diff{x} (\log_b u) = \frac{1}{u \ln b} \dd[u]{x}$
* Now, we can find the derivative of all Logarithmic functions.
* This works for all prior differentiation rules.
* And with this, we have all of our main differentiation rules!
* Now, let's test it, shall we?

---

## Example 8

8. Differentiate $y = \log_2 (2x - 7)$
* Method 1: Exponentials
    * $2^y = 2^{\log_2 (2x - 7)}$
    * $2^y = 2x - 7$
    * $\ln 2^y = \ln (2x - 7)$
    * $y \ln 2 = \ln (2x - 7)$
    * $\diff{} (y \ln 2) = \diff{} (\ln u) [\diff{} (2x - 7)]$
    * $\diff{} (y \ln 2) = \diff{} (\ln u) [\diff{} (2x) - \diff{} (7)]$
    * $dy \ln 2 = (\frac{1}{2x - 7}dx)(2)dx$

---

## Example 8, cont.

8. Differentiate $y = \log_2 (2x - 7)$
* Method 1: Exponentials
    * $dy \ln 2 = (\frac{1}{2x - 7}dx)(2)dx$
    * $dy \ln 2 = dx(\frac{2}{2x - 7})$
    * $\dd[y]{x} = \frac{\frac{2}{2x - 7}}{\ln 2}$
    * $\dd[y]{x} = \frac{2}{(2x - 7)\ln 2}$

---

## Example 8, cont.

8. Differentiate $y = \log_2 (2x - 7)$
* Method 2: Logarithm Rule
    * $y = \log_2 (2x - 7)$
    * $\diff{x} y = \diff{u} (\log_2 u) [\diff{x} (2x - 7)]$
    * $\diff{x} y = \diff{u} (\log_2 u) [\diff{x} (2x) - \diff{x} (7)]$
    * $\dd[y]{x} = \frac{1}{(2x - 7) \ln 2}(2)$
    * $\dd[y]{x} = \frac{2}{(2x - 7) \ln 2}$

---

## Complex Functions

* Now that we have all ten of our main rules, we can differentiate these functions:
    * Polynomials
    * Rationals 
    * Radicals 
    * Logarithmic 
    * Trigonometric 
    * Exponential
    * Any combination of these functions using arithmetic operations and composition.

---

## The (actual) Elementary Functions

* I have a confession to make.
* I (sorta) lied to you.
* In Lesson 1 of this unit, I said that only Polynomials, Rationals and Radicals were elementary functions.
* In reality, all of the functions we've discussed so far are elementary.
* Math is weird, and we have weird names for things.

---

## Example 9

9. Differentiate $f(x) = 2x \ln (\sin x)$
    * $g(x) = 2x$
    * $h(x) = \ln (\sin x)$
    * $y = \ln u$
    * $u = \sin x$
    * $\diff{x} f(x) = (2x) [\diff{u} \ln u (\diff{x} \sin x)] + [\ln (\sin x)] \diff{x} (2x)$
    * $f'(x) = 2x [\frac{1}{\sin x} (\cos x)] + 2[\ln (\sin x)]$
    * $f'(x) = 2x \cot x + 2\ln (\sin x)$
    * $f'(x) = 2(x \cot x + \ln (\sin x))$

---

## Differentiation Laws

1. Constant: $\diff{x} c = 0$
2. Power: $\diff{x} x^n = nx^{n - 1}$
3. Sum / Difference: $\diff{x} [f(x) \pm g(x)] = \diff{x} [f(x)] \pm \diff{x} [g(x)]$
4. Product: $\diff{x} f(x) = g(x) [\diff{x} h(x)] + h(x) [\diff{x} g(x)]$
5. Quotient: $\diff{x} f(x) = \frac{h(x) (\diff{x} g(x)) - g(x) (\diff{x} h(x))}{(h(x))^2}$

---

## Differentiation Laws

6. Chain: $\diff{x} f(x) = \diff{x} g(h(x)) [\diff{x} h(x)]$ or $\diff{x} y = \diff{u} y (\diff{x} u)$
7. Sine: $\diff{x} \sin x = \cos x$
8. Cosine: $\diff{x} \cos x = \sin x$
9. Exponential (General): $\diff{x} b^x = b^x \ln b$
    * Special Case ($e^x$): $\diff{x} e^x = e^x$
10. Logarithm (General): $\diff{x} \log_b x = \frac{1}{x \ln b}$
    * Special Case ($\ln x$): $\diff{x} \ln x = \frac{1}{x}$

---

## Exercise for Readers

* Differentiate the Following Exponentials:
    * $y = 2^x$
    * $y = 4(5^{x^2})$
    * $y = 7^{x^3 - x}$
* Differentiate the Following Logarithmics:
    * $y = \log_7 x$
    * $y = 2 \log_3 (x - 6)$

---

## Exercise for Readers, cont.

* Differentiate the following:
    * $f(x) = 2^{\sin x}$
    * $y = 4x^2 \ln x$
    * $f(x) = 2^x x^2$
    * $y = x \ln [\cos^2 (2x)]$

---

# [Next Unit](../Extrema/Lesson%201)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Differentiate $y = 2^x$
    * $\diff{x} y = \diff{x} 2^x$
    * $\dd[y]{x} = 2^x \ln 2$
* Differentiate $y = 4(5^{x^2})$
    * $y = 4(5^u)$
    * $u = x^2$
    * $\diff{x} y = 4 \diff{u} 5^u (\diff{x} x^2)$
    * $\dd[y]{x} = 4(5^{x^2} \ln 5) (2x)$

---

## Answers to Exercises, cont.

* Differentiate $y = 4(5^{x^2})$
    * $\dd[y]{x} = 4(5^{x^2} \ln 5) (2x)$
    * $\dd[y]{x} = 8x\ln 5(5^{x^2})$

---

## Answers to Exercises, cont.

* Differentiate $y = 7^{x^3 - x}$
    * $y = 7^u$
    * $u = x^3 - x$
    * $\diff{x} y = \diff{u} 7^u [\diff{x} (x^3 - x)]$
    * $\diff{x} y = \diff{u} 7^u [\diff{x} (x^3) - \diff{x} (x)]$
    * $\dd[y]{x} = 7^{x^3 - x} \ln 7 (3x^2 - 1)$

---

## Answers to Exercises, cont.

* Differentiate $y = \log_7 x$
    * $\diff{x} y = \diff{x} (\log_7 x)$
    * $\dd[y]{x} = \frac{1}{x \ln 7}$

---

## Answers to Exercises, cont.

* Differentiate $y = 2 \log_3 (x - 6)$
    * $y = \log_3 (x - 6)^2$
    * $y = \log_3 u$
    * $u = v^2$
    * $v = (x - 6)$
    * $\diff{x} y = \diff{u} \log_3 u (\diff{v} v^2)[\diff{x} (x - 6)]$
    * $\diff{x} y = \diff{u} \log_3 u (\diff{v} v^2)[\diff{x} (x) - \diff{x} (6)]$
    * $\dd[y]{x} = \frac{1}{(x - 6)^2 \ln 3} 2(x - 6)$

---

## Answers to Exercises, cont.

* Differentiate $y = 2 \log_3 (x - 6)$
    * $\dd[y]{x} = \frac{1}{(x - 6)^2 \ln 3} 2(x - 6)$
    * $\dd[y]{x} = \frac{2}{(x - 6) \ln 3}$

---

## Answers to Exercises, cont.

* Differentiate $f(x) = 2^{\sin x}$
    * $y = 2^u$
    * $u = \sin x$
    * $\diff{x} f(x) = \diff{u} 2^u (\diff{x} \sin x)$
    * $f'(x) = 2^u \ln 2 (\cos x)$
    * $f'(x) = 2^{\sin x} \ln 2 (\cos x)$

---

## Answers to Exercises, cont.

* Differentiate $y = 4x^2 \ln x$
    * $g(x) = 4x^2$
    * $h(x) = \ln x$
    * $\diff{x} y = (4x^2) [\diff{x} (\ln x)] + (\ln x) [\diff{x} (4x^2)]$
    * $\dd[y]{x} = (4x^2) (\frac{1}{x}) + (\ln x)(8x)$
    * $\dd[y]{x} = 4x(1 + 2 \ln x)$

---

## Answers to Exercises, cont.

* Differentiate $f(x) = 2^x x^2$
    * $g(x) = 2^x$
    * $h(x) = x^2$
    * $\diff{x} f(x) = (2^x) [\diff{x} (x^2)] + (x^2) [\diff{x} (2^x)]$
    * $f'(x) = (2^x) (2x) + (x^2) (2^x \ln 2)$
    * $f'(x) = x(2^x)[2 + x\ln 2]$

---

## Answers to Exercises, cont.

* Differentiate $y = x \ln [\cos^2 (2x)]$
    * $g(x) = x$
    * $h(x) = \ln [\cos^2 (2x)]$
    * $h(u) = \ln u$
    * $u = v^2$
    * $v = \cos w$
    * $w = 2x$
    * $\diff{x} y = (x) [\diff{u} \ln u (\diff{v} v^2)(\diff{w} \cos w)(\diff{x} 2x)]$ 
    $+ (\ln [\cos^2 (2x)]) [\diff{x} (x)]$

---

## Answers to Exercises, cont.

* Differentiate $y = x \ln [\cos^2 (2x)]$
    * $u = v^2$
    * $v = \cos w$
    * $w = 2x$
    * $\diff{x} y = (x) [\diff{u} \ln u (\diff{v} v^2)(\diff{w} \cos w)(\diff{x} 2x)]$ 
    $+ (\ln [\cos^2 (2x)]) [\diff{x} (x)]$
    * $\dd[y]{x} = (x) [\frac{1}{u} (2v)(-\sin w)(2)] + (\ln [\cos^2 (2x)])$
    * $\dd[y]{x} = (x) (-4\frac{\sin 2x}{\cos 2x}) + (\ln [\cos^2 (2x)])$

---

## Answers to Exercises, cont.

* Differentiate $y = x \ln [\cos^2 (2x)]$
    * $\dd[y]{x} = (x) (-4\frac{\sin 2x}{\cos 2x}) + (\ln [\cos^2 (2x)])$
    * $\dd[y]{x} = \ln [\cos^2 (2x)] - 4x\tan 2x$

---

# [Next Unit](../Extrema/Lesson%201)