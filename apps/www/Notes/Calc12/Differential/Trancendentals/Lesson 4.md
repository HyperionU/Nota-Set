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

# Lesson 4: Logarithmic Derivatives I

---

<!--paginate: true-->

## Intro

* For this unit, all six of the previous rules (Constant, Power, Sum / Difference, Product, Quotient and Chain) are used in the same way as elementary functions.
* The only additional rules needed are the derivatives for specific transcendental functions.
* We started by deriving rules 7 and 8: The Sine and Cosine Rules.
* Let's start by looking at a special case of one of our unknown rules: The Logarithm Rule.

---

## Logarithmic Functions

* A logarithmic function is the inverse of an exponential function.
* It is written as follows:
    * $y = \log_b x$ s.t. $x > 0$, $x \in \mathbb{R}$, $b > 1$
* Prior to this lesson, the logarithmic function you're most familiar with had rational bases. 
* The common logarithm you learned has a base of 10. (e.g. $\log x$)
* Now, you'll learn the logarithm with an irrational base: $e$

---

## What is $e$?

* $e$ represents an irrational number defined by one of these two limits:
    * $\limit{n}{0} (1 + n)^\frac{1}{n}$
    * $\limit{n}{0} (1 + \frac{1}{n})^n$
* Both of these limits have the same value: about $2.7182\dots$
* Because of the importance of the base-$e$ logarithm, it's given a special name: The Natural Logarithm ($\ln x$)

---

## Deriving the Derivative of $\ln x$

* Let's start with first principles, given $f(x) = \ln x$.
    * $f'(x) = \limit{h}{0} \frac{\ln (x + h) - \ln x}{h}$
* Using $\ln A - \ln B = \ln \frac{A}{B}$
    * $f'(x) = \limit{h}{0} \frac{\ln (\frac{x + h}{x})}{h}$
    * $f'(x) = \limit{h}{0}\frac{1}{h} \ln (1 + \frac{h}{x})$
    * $f'(x) = \limit{h}{0} \frac{x}{h}\frac{1}{x} \ln (1 + \frac{h}{x})$


---

## Deriving the Derivative of $\ln x$

* We have this:
    * $f'(x) = \limit{h}{0} \frac{x}{h}\frac{1}{x} \ln (1 + \frac{h}{x})$
    * $f'(x) = \frac{1}{x} \limit{h}{0} \frac{x}{h} \ln (1 + \frac{h}{x})$
* Using $n \ln A = \ln A^n$:
    * $f'(x) = \frac{1}{x} \limit{h}{0} \ln (1 + \frac{h}{x})^\frac{x}{h}$
* Let $n = \frac{h}{x}$, $h \to 0$, $n \to 0$
    * $f'(x) = \frac{1}{x} \limit{n}{0} \ln (1 + n)^\frac{1}{n}$

---

## Deriving the Derivative of $\ln x$

* We now have:
    * $f'(x) = \frac{1}{x} \limit{n}{0} \ln (1 + n)^\frac{1}{n}$
* Since $\ln x$ is continuous, $\limit{a}{0} \ln (f(a)) = \ln (\limit{a}{0} f(a))$
    * $f'(x) = \frac{1}{x} \ln [\limit{n}{0} (1 + n)^\frac{1}{n}]$
* $\limit{n}{0} (1 + n)^\frac{1}{n} = e$
    * $f'(x) = \frac{1}{x} \ln e$
* Using $\log_b b = 1$, and $\ln x = \log_e x$
    * $f'(x) = \frac{1}{x}$

---

## The Derivative of $\ln x$

$\diff{x} (\ln x) = \frac{1}{x}$

* By the chain rule: $\diff{x} (\ln u) = \frac{1}{x} \dd[u]{x}$
* With this, we can find the derivative of some logarithmic functions.
* Next lesson, this will be helpful to know for differentiating exponentials as well.
* This works for all prior differentiation rules. (Constant, Power, Sum / Difference, Product, Quotient, Chain)

---

## Example 1

1. Differentiate $y = 2 \ln x$
    * $\diff{x} y = \diff{x} (2 \ln x)$
    * $\dd[y]{x} = 2 (\frac{1}{x})$
    * $\dd[y]{x} = \frac{2}{x}$

---

## Example 2

2. Differentiate $y = 4x \ln x$
    * $g(x) = 4x$
    * $h(x) = \ln x$
    * $\diff{x} y = (4x) [\diff{x} (\ln x)] + (\ln x) [\diff{x} (4x)]$
    * $\dd[y]{x} = (4x) \frac{1}{x} + (\ln x)(4)$
    * $\dd[y]{x} = 4 + 4\ln x$

---

## Example 3

3. Differentiate $f(x) = \ln (x^2 - x)$
    * Method 1: Logarithm Rules
        * $f(x) = \ln [x(x - 1)]$
        * $f(x) = \ln x + \ln (x - 1)$
        * $y = \ln u$
        * $u = x - 1$
        * $\diff{x} f(x) = \diff{x} (\ln x) + [\diff{u} (\ln u) (\diff{x} x - 1)]$
        * $\diff{x} f(x) = \diff{x} (\ln x) + [\diff{u} (\ln u) (\diff{x} x) - \diff{x} (1)]$
        * $f'(x) = \frac{1}{x} + \frac{1}{x - 1}$

---

## Example 3, cont.

3. Differentiate $f(x) = \ln (x^2 - x)$
    * Method 1: Logarithm Rules
        * $f'(x) = \frac{1}{x} + \frac{1}{x - 1}$
        * $f'(x) = \frac{x - 1 + x}{x(x - 1)}$
        * $f'(x) = \frac{2x - 1}{x^2 - x}$
    * Method 2: Chain Rule
        * $y = \ln u$
        * $u = x^2 - x$
        * $\diff{x} f(x) = \diff{u} \ln u [\diff{x} (x^2 - x)]$

---

## Example 3, cont.

3. Differentiate $f(x) = \ln (x^2 - x)$
    * Method 2: Chain Rule
        * $u = x^2 - x$
        * $\diff{x} f(x) = \diff{u} \ln u [\diff{x} (x^2 - x)]$
        * $\diff{x} f(x) = \diff{u} \ln u [\diff{x} (x^2) - \diff{x} (x)]$
        * $f'(x) = \frac{1}{u}(2x - 1)$
        * $f'(x) = \frac{2x - 1}{x^2 - x}$

---

## Example 4

4. Differentiate $3y = \ln xy$
    * $u = \ln v$
    * $v = xy$
    * $\diff{} 3y = \diff{v} \ln v [x (\diff{} y) + y (\diff{} x)]$
    * $3dy = \frac{1}{xy} [x(dy) + y(dx)]$
    * $3dy = \frac{dy}{y} + \frac{dx}{x}$
    * $3dy - \frac{dy}{y} = \frac{dx}{x}$
    * $dy(3 - \frac{1}{y}) = dx(\frac{1}{x})$

---

## Example 4, cont.

4. Differentiate $3y = \ln xy$
    * $dy(3 - \frac{1}{y}) = dx(\frac{1}{x})$
    * $\dd[y]{x} = \frac{1}{x(3 - \frac{1}{y})}$
    * $\dd[y]{x} = \frac{1}{x(\frac{3y - 1}{y})}$
    * $\dd[y]{x} = \frac{1}{\frac{x(3y - 1)}{y}}$

---

## Example 4, cont.

4. Differentiate $3y = \ln xy$
    * $\dd[y]{x} = \frac{1}{\frac{x(3y - 1)}{y}}$
    * $\dd[y]{x} = \frac{y}{x(3y - 1)}$
    * $\dd[y]{x} = \frac{y}{3xy - x}$

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
9. Exponential: Lesson 5
10. Logarithm (General): Lesson 5 
    * Special Case ($\ln x$): $\diff{x} \ln x = \frac{1}{x}$

---

## Exercise for Readers

* Differentiate the following:
    * $y = \ln (x^2)$
    * $f(x) = 3x^2 \ln (x + 1)$
    * $y = \frac{\ln x}{x^3}$
    * $y = \ln (3x^2 - 1)$
    * $xy = \ln y$

---

# [Next Lesson](Lesson%205)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Differentiate $y = \ln (x^2)$
    * Method 1: Logarithm Rules
        * $\diff{x} y = 2 \diff{x} (\ln x)$
        * $\dd[y]{x} = 2 (\frac{1}{x})$
        * $\dd[y]{x} = \frac{2}{x}$

---

## Answers to Exercises, cont.

* Differentiate $y = \ln (x^2)$
    * Method 2: Chain Rule
        * $u = \ln v$
        * $v = x^2$
        * $\diff{x} y = \diff{v} \ln v (\diff{x} x^2)$
        * $\dd[y]{x} = \frac{1}{x^2} (2x)$
        * $\dd[y]{x} = \frac{2}{x}$


---

## Answers to Exercises, cont.

* Differentiate $f(x) = 3x^2 \ln (x + 1)$
    * $g(x) = 3x^2$
    * $h(x) = \ln (x + 1)$
    * $y = \ln u$
    * $u = x + 1$
    * $\diff{x} f(x) = (3x^2) [\diff{u} \ln u [\diff{x} (x + 1)]] + [\ln (x + 1)] [\diff{x} (3x^2)]$
    * $\diff{x} f(x) = (3x^2) [\diff{u} (\ln u) [\diff{x} (x) + \diff{x} (1)]] +$ 
    $[\ln (x + 1)] [\diff{x} (3x^2)]$
    * $f'(x) = (3x^2) \frac{1}{x + 1} + (6x)\ln (x + 1)$

---

## Answers to Exercises, cont.

* Differentiate $f(x) = 3x^2 \ln (x + 1)$
    * $f'(x) = (3x^2) \frac{1}{x + 1} + (6x)\ln (x + 1)$
    * $f'(x) = 3x[\frac{x}{x + 1} + 2\ln (x + 1)]$
    * $f'(x) = 3x[\frac{x}{x + 1} + \ln (x + 1)^2]$

---

## Answers to Exercises, cont.

* Differentiate $y = \frac{\ln x}{x^3}$
    * $g(x) = \ln x$
    * $h(x) = x^3$
    * $\diff{x} y = \frac{x^3 [\diff{x} (\ln x)] - (\ln x) [\diff{x} (x^3)]}{(x^3)^2}$
    * $\dd[y]{x} = \frac{x^3 (\frac{1}{x}) - 3(\ln x)(x^2)}{x^6}$
    * $\dd[y]{x} = \frac{x^2 - 3(\ln x)(x^2)}{x^6}$

---

## Answers to Exercises, cont.

* Differentiate $y = \frac{\ln x}{x^3}$
    * $\dd[y]{x} = \frac{x^2 - 3(\ln x)(x^2)}{x^6}$
    * $\dd[y]{x} = \frac{x^2[1 - 3\ln x]}{x^6}$
    * $\dd[y]{x} = \frac{1 - \ln x^3}{x^4}$

---

## Answers to Exercises, cont.

* Differentiate $y = \ln (3x^2 - 1)$
    * $u = \ln v$
    * $v = 3x^2 - 1$
    * $\diff{x} y = \diff{v} (\ln v) [\diff{x} (3x^2 - 1)]$
    * $\diff{x} y = \diff{v} (\ln v) [\diff{x} (3x^2) - \diff{x} (1)]$
    * $\dd[y]{x} = \frac{1}{3x^2 - 1} (6x)$
    * $\dd[y]{x} = \frac{6x}{3x^2 - 1}$

---

## Answers to Exercises, cont.

* Differentiate $xy = \ln y$
    * $\diff{} (\ln y) = x [\diff{} (y)] + y [\diff{} (x)]$
    * $\frac{1}{y}(dy) = x(dy) + y(dx)$
    * $\frac{1}{y}(dy) - x(dy) = y(dx)$
    * $dy[\frac{1}{y} - x] = y(dx)$
    * $\dd[y]{x} = \frac{y}{\frac{1}{y} - x}$
    * $\dd[y]{x} = \frac{y}{\frac{1 - xy}{y}}$

---

## Answers to Exercises, cont.

* Differentiate $xy = \ln y$
    * $\dd[y]{x} = \frac{y}{\frac{1 - xy}{y}}$
    * $\dd[y]{x} = y \cdot \frac{y}{1 - xy}$
    * $\dd[y]{x} = \frac{y^2}{1 - xy}$

---

# [Next Lesson](Lesson%205)