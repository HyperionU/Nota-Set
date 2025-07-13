---
marp: true
theme: uncover
class: invert
math: mathjax
---

$\newcommand\diff[1]{\mathcal{d}_{#1}}$

# <!--fit--> Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

$\newcommand\dd[2][]{\displaystyle\frac{d#1}{d#2}}$

<!--_footer: In partnership with Hyperion University, 2025-->

---

# Lesson 6: Newton's Method

---

<!--paginate: true-->

## Intro 

* Often in many cases, we need to find the roots of equations in the form $f(x) = 0$.
* One common method is Newton's method (or the Newton-Raphson method).
* This method is very useful for approximating roots of complicated equations, or for programming computers and calculators to approximate as required.

---

## Defining Newton's Method

* If $x_1$ is the first approximation of the zero of the function $y = f(x)$, then the slope of the tangent line through $P(x_1, f(x_1))$ and $Q(x_2, 0)$ must equal the derivative at $x = x_1$.
* $\frac{f(x_1) - 0}{x_1 - x_2} = f'(x_1)$
* $\frac{f(x_1)}{f'(x_1)} = x_1 - x_2$
* $x_2 = x_1 - \frac{f(x_1)}{f'(x_1)}$
* We can use this new value to determine the next approximation.

---

## Newton's Method

* In general, each approximation will tend to be closer than the previous one.
* By this method, the approximate root is $x^* = x - \frac{f(x)}{f'(x)}, f'(x) \ne 0$ where our first approximation is provided by the user whom chooses a reasonable approximation for the root.
* Now, let's take it for a spin, shall we?

---

## Example 1

1. Using Newton's method, approximate a root of $f(x) = x^3 - 2x - 6$.
    * $\diff{x} f(x) = \diff{x} (x^3 - 2x - 6)$
    * $\diff{x} f(x) = \diff{x} (x^3) - \diff{x} (2x) - \diff{x} (6)$
    * $f'(x) = 3x^2 - 2$
    * Let $x_1 = 2$
    * $x^* = x - \frac{x^3 - 2x - 6}{3x^2 - 2}$
    * $x^* = 2 - \frac{(2)^3 - 2(2) - 6}{3(2)^2 - 2}$
    * $x^* = 2 - \frac{-2}{10}$

---

## Example 1, cont.

1. Using Newton's method, approximate a root of $f(x) = x^3 - 2x - 6$.
    * $x^* = x - \frac{x^3 - 2x - 6}{3x^2 - 2}$
    * $x^* = 2 - \frac{-2}{10}$
    * $x^* = \frac{10}{5} + \frac{1}{5}$
    * $x^* = \frac{11}{5} = x$
    * $x^* = \frac{11}{5} - \frac{(\frac{11}{5})^3 - 2(\frac{11}{5}) - 6}{3(\frac{11}{5})^2 - 2}$
    * $x^* = \frac{11}{5} - \frac{\frac{11^3}{5^3} - \frac{22}{5} - 6}{\frac{3(11^2)}{5^2} - 2}$

---

## Example 1, cont.

1. Using Newton's method, approximate a root of $f(x) = x^3 - 2x - 6$.
    * $x^* = x - \frac{x^3 - 2x - 6}{3x^2 - 2}$
    * $x^* = \frac{11}{5} - \frac{\frac{11^3}{5^3} - \frac{22}{5} - 6}{\frac{3(11^2)}{5^2} - 2}$
    * $x^* = \frac{11}{5} - (\frac{31}{125} / \frac{313}{25})$
    * $x^* = \frac{11}{5} - \frac{31}{1565}$
    * $x^* \approx 2.18$

---

## Example 2

2. Using the third value from Newton's method, approximate a root of $f(x) = x^2 - 5x - 7$. Use $x_1 = 6$.
    * $\diff{x} f(x) = \diff{x} (x^2 - 5x - 7)$
    * $f'(x) = 2x - 5$
    * $x^* = x - \frac{x^2 - 5x - 7}{2x - 5}$
    * $x^* = 6 - \frac{(6)^2 - 5(6) - 7}{2(6) - 5}$
    * $x^* = 6 + \frac{1}{7}$
    * $x^* = \frac{43}{7} = x$

---

## Example 2, cont.

2. Using the third value from Newton's method, approximate a root of $f(x) = x^2 - 5x - 7$. Use $x_1 = 6$.
    * $x^* = x - \frac{x^2 - 5x - 7}{2x - 5}$
    * $x_2 = \frac{43}{7} = x$
    * $x^* = \frac{43}{7} - \frac{(\frac{43}{7})^2 - 5(\frac{43}{7}) - 7}{2(\frac{43}{7}) - 5}$
    * $x^* = \frac{43}{7} - (\frac{43^2 - 35(43) - 7^3}{7^2} / \frac{2(43) - 5(7)}{7})$
    * $x^* = \frac{43}{7} - \frac{1}{7(51)}$
    * $x^* = \frac{2192}{357} = x_3$

---

## Example 3

3. Using $x_1 = \frac{5}{2}$, find the third approximation a root of $f(x) = x^2 - 3 - \frac{1}{x - 2}$.
    * $\diff{x} f(x) = \diff{x} (x^2 - 3 - (x - 2)^{-1})$
    * $f'(x) = 2x + \frac{1}{(x - 2)^2}$
    * $x^* = x - \frac{x^2 - 3 - \frac{1}{x - 2}}{2x + \frac{1}{(x - 2)^2}}$
    * $x^* = \frac{5}{2} - \frac{(\frac{5}{2})^2 - 3 - \frac{1}{(\frac{5}{2}) - 2}}{2(\frac{5}{2}) + \frac{1}{((\frac{5}{2}) - 2)^2}}$

---

## Example 3, cont.

3. Using $x_1 = \frac{5}{2}$, find the third approximation a root of $f(x) = x^2 - 3 - \frac{1}{x - 2}$.
    * $x^* = x - \frac{x^2 - 3 - \frac{1}{x - 2}}{2x + \frac{1}{(x - 2)^2}}$
    * $x^* = \frac{5}{2} - \frac{(\frac{5}{2})^2 - 3 - \frac{1}{(\frac{5}{2}) - 2}}{2(\frac{5}{2}) + \frac{1}{((\frac{5}{2}) - 2)^2}}$
    * $x^* = \frac{5}{2} - \frac{5}{4(9)}$
    * $x^* = \frac{5(17)}{4(9)}$
    * $x^* = \frac{85}{36}$

---

## Example 3, cont.

3. Using $x_1 = \frac{5}{2}$, find the third approximation a root of $f(x) = x^2 - 3 - \frac{1}{x - 2}$.
    * $x^* = x - \frac{x^2 - 3 - \frac{1}{x - 2}}{2x + \frac{1}{(x - 2)^2}}$
    * $x = \frac{85}{36}$
    * $x^* = \frac{85}{36} - \frac{(\frac{85}{36})^2 - 3 - \frac{1}{(\frac{85}{36}) - 2}}{2(\frac{85}{36}) + \frac{1}{((\frac{85}{36}) - 2)^2}}$
    * $x^* = \frac{85}{36} + \frac{3275}{16848} / \frac{37693}{3042}$
    * $x^* = \frac{85}{36} + \frac{42575}{2713896}$
    * $x^* = \frac{6450385}{2713896}$

---

## Example 3, cont.

3. Using $x_1 = \frac{5}{2}$, find the third approximation a root of $f(x) = x^2 - 3 - \frac{1}{x - 2}$.
    * $x^* = x - \frac{x^2 - 3 - \frac{1}{x - 2}}{2x + \frac{1}{(x - 2)^2}}$
    * $x = \frac{85}{36}$
    * $x^* = \frac{85}{36} + \frac{42575}{2713896}$
    * $x^* = \frac{6450385}{2713896}$

---

## Exercise for Readers

* Use Newton's method for the desired approximation:
    * $x^2 - 12 = 0, x_1 = 2, x_4?$
    * $x^2 - 5x - 5 = 0, x_1 = 2, x_3?$
    * $\sin x = 0, x_1 = 3, x_3?$ (rad.)
    * $x^2 - 2 = \frac{x + 4}{x}, x_1 = 2, x_3?$

---

# [Next Unit](../../Integral/Antiderivatives/Lesson%201)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercise

* Use Newton's method for the desired approximation: $x^2 - 12 = 0, x_1 = 2, x_4?$
    * $\diff{x} f(x) = \diff{x} x^2 - 12$
    * $f'(x) = 2x$
    * $x_2 = x_1 - \frac{f(x_1)}{f'(x_1)}$
    * $x_2 = x_1 - \frac{x_1^2 - 12}{2x_1}$
    * $x_2 = 2 - \frac{(2)^2 - 12}{2(2)}$
    * $x_2 = 2 + \frac{8}{4}$
    * $x_2 = 4$

---

## Answers to Exercise, cont.

* Use Newton's method for the desired approximation: $x^2 - 12 = 0, x_1 = 2, x_4?$
    * $x_3 = x_2 - \frac{x_2^2 - 12}{2x_2}$
    * $x_2 = 4$
    * $x_3 = 4 - \frac{(4)^2 - 12}{2(4)}$
    * $x_3 = 4 - \frac{1}{2}$
    * $x_3 = \frac{7}{2}$

---

## Answers to Exercise, cont.

* Use Newton's method for the desired approximation: $x^2 - 12 = 0, x_1 = 2, x_4?$
    * $x_4 = x_3 - \frac{x_3^2 - 12}{2x_3}$
    * $x_3 = \frac{7}{2}$
    * $x_4 = \frac{7}{2} - \frac{(\frac{7}{2})^2 - 12}{2(\frac{7}{2})}$
    * $x_4 = \frac{7}{2} - \frac{(\frac{49}{4} - 12}{7}$
    * $x_4 = \frac{7}{2} - \frac{1}{28}$
    * $x_4 = \frac{97}{28}$

---

## Answers to Exercise, cont.

* Use Newton's method for the desired approximation: $x^2 - 5x - 5 = 0, x_1 = 2, x_3?$
    * $\diff{x} f(x) = \diff{x} x^2 - 5x - 5$
    * $f'(x) = 2x - 5$
    * $x_2 = x_1 - \frac{f(x_1)}{f'(x_1)}$
    * $x_2 = x_1 - \frac{x_1^2 - 5x_1 - 5}{2x_1 - 5}$
    * $x_2 = 2 - \frac{(2)^2 - 5(2) - 5}{2(2) - 5}$
    * $x_2 = 2 - 11$
    * $x_2 = -9$

---

## Answers to Exercise, cont.

* Use Newton's method for the desired approximation: $x^2 - 5x - 5 = 0, x_1 = 2, x_3?$
    * $x_3 = x_2 - \frac{x_2^2 - 5x_2 - 5}{2x_2 - 5}$
    * $x_2 = -9$
    * $x_3 = (-9) - \frac{(-9)^2 - 5(-9) - 5}{2(-9) - 5}$
    * $x_3 = -\frac{86}{23}$

---

## Answers to Exercise, cont.

* Use Newton's method for the desired approximation: $\sin x = 0, x_1 = 3, x_3?$ (rad.)
    * $x_2 = x_1 - \frac{f(x_1)}{f'(x_1)}$
    * $x_2 = x_1 - \frac{\sin x_1}{\cos x_1}$
    * $x_2 = x_1 - \tan x_1$
    * $x_2 = 3 - \tan 3$
    * $x_2 = 3.1425465431$
    * $x_2 = \pi - \mu_1$ $(\mu_1 = 9.54\times 10^{-4})$

---

## Answers to Exercise, cont.

* Use Newton's method for the desired approximation: $\sin x = 0, x_1 = 3, x_3?$ (rad.)
    * $x_3 = x_2 - \tan x_2$
    * $x_2 = 3.1425465431$
    * $x_2 = \pi - \mu_1$ $(\mu_1 = 9.54\times 10^{-4})$
    * $x_3 = \pi - \mu_1 - \tan (\pi - \mu_1)$
    * $x_3 \approx \pi$

---

## Answers to Exercise, cont.

* Use Newton's method for the desired approximation: $x^2 - 2 = \frac{x + 4}{x}, x_1 = 2, x_3?$
    * $x^3 - 3x - 4 = 0$
    * $\diff{x} f(x) = \diff{x} x^3 - 3x - 4$
    * $f'(x) = 3x^2 - 3$
    * $f'(x) = 3(x^2 - 1)$
    * $x_2 = x_1 - \frac{f(x_1)}{f'(x_1)}$
    * $x_2 = x_1 - \frac{x^3 - 3x - 4}{3(x^2 - 1)}$

---

## Answers to Exercise, cont.

* Use Newton's method for the desired approximation: $x^2 - 2 = \frac{x + 4}{x}, x_1 = 2, x_3?$
    * $x_2 = x_1 - \frac{x_1^3 - 3x_1 - 4}{3(x_1^2 - 1)}$
    * $x_2 = 2 - \frac{(2)^3 - 3(2) - 4}{3(2^2 - 1)}$
    * $x_2 = 2 + \frac{2}{9}$
    * $x_2 = \frac{20}{9}$

---

## Answers to Exercise, cont.

* Use Newton's method for the desired approximation: $x^2 - 2 = \frac{x + 4}{x}, x_1 = 2, x_3?$
    * $x_2 = \frac{20}{9}$
    * $x_3 = x_2 - \frac{x_2^3 - 3x_2 - 4}{3(x_2^2 - 1)}$
    * $x_3 = \frac{20}{9} - \frac{(\frac{20}{9})^3 - 3(\frac{20}{9}) - 4}{3((\frac{20}{9})^2 - 1)}$
    * $x_3 = \frac{20}{9} - \frac{\frac{224}{729}}{\frac{319}{27}}$
    * $x_3 = \frac{44612}{21141}$

---

## Answers to Exercise, cont.

* Use Newton's method for the desired approximation: $4\sin^2 x - 3 = 0, x_1 = 1, x_3?$ (rad.)
    * $\diff{x} f(x) = \diff{x} (4\sin^2 x - 3)$
    * $u = \sin x$
    * $\diff{x} f(x) = \diff{u} 4u^2 (\diff{x} \sin x) - \diff{x} (3)$
    * $f'(x) = 8\sin x(\cos x)$
    * $f'(x) = 4\sin 2x$
    * $x_2 = x_1 - \frac{f(x_1)}{f'(x_1)}$
    * $x_2 = x_1 - \frac{4\sin^2 x_1 - 3}{4\sin 2x_1}$

---

# [Next Unit](../../Integral/Antiderivatives/Lesson%201)