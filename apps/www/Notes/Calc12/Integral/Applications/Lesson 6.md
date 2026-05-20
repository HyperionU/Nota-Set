---
marp: true
theme: uncover
class: invert
math: mathjax
---

$\newcommand\diff[1]{\mathcal{d}_{#1}}$

# <!--fit--> Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2025-->

$\newcommand\dd[2][]{\displaystyle\frac{d#1}{d#2}}$

---

# Lesson 6: Differential Equations and Initial Values

---

<!--paginate: true-->

## Intro

* When the concept of the antiderivative was first introduced, it was made clear that a general constant must be included.
* When we include this constant, this is the most general antiderivative.
* However, we can solve for $C$ if we have additional information. 
* This is known as the initial condition.

---

## Initial Value Problems

* Earlier uses of differentiation was to find the rate of change of displacement ($s$) of an object with respect to time. This is our velocity $v$.
* If we know the velocity (and it is constant), we can multiply by time to get the displacement.
* However, there may be an initial condition that we'd need to consider.
* The problem of finding the particular antiderivative from a point is called an Initial Value Problem.

---

## Example 1

1. Solve for $y$ if $\dd[y]{x} = 4x$ and $x = 1 \mapsto y = 7$.
    * $dy = 4x dx$
    * $\int dy = \int 4x dx$
    * $y = 2x^2 + C$
    * $7 = 2(1)^2 + C$
    * $C = 5$
    * $y = 2x^2 + 5$.

---

## Example 2

2. Mr. Jones stand a short distance behind a sedan driving away from him at a velocity of 50 km/hr. If we assume the velocity is constant, how far is the sedan away after six minutes?
    * $v = \dot{s} = 50 \left.\mathrm{km}\!\middle/\!\mathrm{hr}\right.$
    * $s = (50 \left.\mathrm{km}\!\middle/\!\mathrm{hr}\right.)t + C$
    * $s = (5\mathrm{km}) + C$

---

## Example 3: Graphs

3. The slope of a given graph is $\frac{x}{2}$. If the function has a y-intercept of $3$, what is the original function?
    * $\dd[y]{x} = \frac{x}{2}$
    * $y = \frac{x^2}{4} + C$
    * $C = 3$
    * $\therefore y = \frac{x^2}{4} + 3$.

---

## Example 4: Gravity

4. A person standing on top of a 50m building throws a ball upward with a velocity of 10m/s. If gravity is constant ($g = 9.8 \left.\mathrm{m}\!\middle/\!\mathrm{s}^2\right.$), what is the displacement function of the ball?
    * $a = \dot{v} = -g$
    * $v = -gt + 10$
    * $s = -\frac{1}{2}gt + 10t + s_0$
* $s_0$ is dependent on where we define our reference point to determine distance.

---

## Springs and Pendulums

* An important type of differential equation is $\ddot{y} + ky = 0, k > 0$.
* These are often use to represent osciliatory systems like springs and pendulums.
* We can't simply take the antiderivative of this function, but we can use some interesting properties to determine results.

---

## Springs and Pendulums: Solving

* First, our equation $\ddot{y} + ky = 0, k > 0$ is linear. So, if we know some solutions, other solutions are linear combinations of them.
* So, $y = \sum C_i y_i$.
* What if we use sine and cosine?
* $y = \sin kx, y' = k\cos kx, y'' = -k^2 \sin kx = -k^2 y$.
* $y = \cos kx, y' = -k\sin kx, y'' = -k^2 \cos kx = -k^2 y$.
* So, $y = A\sin(\sqrt{k}x) + B\cos(\sqrt{k}x), k > 0$!

---

## Example 5: Pendulum

5. The displacement of a pendulum is given by $\ddot{s} + 9s = 0$ with initial conditions $s(0) = 0, s'(0) = \frac{1}{2}$. Find the original displacement function.
    * We'll use the sample equation $y = A\sin \sqrt{k} x + B \cos \sqrt{k} x$
    * So $s = A \sin 3t + B\cos 3t$.
    * We can use our first condition: $0 = A \sin 0 + B \cos 0$.
    * And we get $B = 0$.

---

## Example 5, cont.

5. The displacement of a pendulum is given by $\ddot{s} + 9s = 0$ with initial conditions $s(0) = 0, s'(0) = \frac{1}{2}$. Find the original displacement function.
    * So $s = A \sin 3t$.
    * We can use our second condition: $\frac{1}{2} = 3A \cos 0$
    * And we obtain $A = \frac{1}{6}$
    * So $s = \frac{1}{6} \sin 3t$

---

## Hooke's Law

* Using this equation is very common when using Hooke's Law.
* It states that the force needed to stretch a spring is proportional to the distance stretched: $F(s) = ks$
* Adding this to Newton's Second Law: $ks = -m\ddot{s}$ (it's negative because the force opposes the motion).
* Therefore: $\ddot{s} + \frac{k}{m}s = 0$, and its solution will be $s = A\sin \sqrt{\frac{k}{m}}t + B \cos \sqrt{\frac{k}{m}}t$ based on initial conditions.

---

## Exponential Growth / Decau

* In a continuous exponential growth or decay problem, the rate of change is proportional to its value at that instant.
* Put simply, $\dot{y} = ky$.

---

## Example 6: Compound Interest

6. An account pays continuous compound interest at a rate of 5.2%. If the account balance at the end of eight years is $1k, what is the equation relating the amortised value and time?
    * $\dot{y} = ry$
    * Using separation of variables: $\frac{dy}{y} = r dt$
    * Integrating: $\ln y = rt + C$
    * $y = e^{rt + C}$
    * $y = Ae^{rt}, A = e^C$.

---

## Example 6, cont.

6. An account pays continuous compound interest at a rate of 5.2%. If the account balance at the end of eight years is $1k, what is the equation relating the amortised value and time?
    * $y = Ae^{kt}, A = e^C$.
    * $1000 = Ae^{(0.052)8}$.
    * $1000 = Ae^{0.416}$.
    * $A = \frac{1000}{e^{0.416}} \approx 659.68$.
    * $y = 659.68e^{0.052t}$

---

## Exercise for Readers

* Solve the following Initial Value Problems:
    * Given $a(t) = t + 1$, determine the velocity and displacement, given $v(0) = 0, s(0) = 0, t \ge 0$.
    * Given $a(t) = 3\sin t$, find $s$ if $v(0) = 1, s(0) = 1$.
    * $\diff{x}^2 y = x - 1, \dd[y]{x}(0) = 1, P(1, 2)$
    * $v = 2t - 1$, find the distance traveled in $t \in [3, 5]$
    * Solve $y'' + 16y = 0, x = \frac{\pi}{2}, y = 1, y' = 1$.

---

## Exercise for Readers, cont
* Solve the following Initial Value Problems:
    * A spring with a mass of 0.5kg has a natural length of 0.1m. A force of 10N is required to stretch to 0.2m. If the spring is stretched to 3 times its normal length, what is the displacement of the mass at time $t$ after it is released from rest?

---

# [Finish](../../../../)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Given $a(t) = t + 1$, determine the velocity and displacement, given $v(0) = 0, s(0) = 0, t \ge 0$.
    * $a = \dot{v} = t + 1$
    * $v = \dot{s} = \frac{t^2 + 2t}{2}$
    * $s = \frac{t^3}{6} + \frac{t^2}{2}$
    * $s = \frac{t^3 + 3t^2}{6}$

---

## Answers to Exercises, cont.

* Given $a(t) = 3\sin t$, find $s$ if $v(0) = 1, s(0) = 1$.
    * $a = \dot{v} = 3\sin t$
    * $v = \dot{s} = -3\cos t + v_0$
    * $s = -3\sin t + 4t + 1$

---

## Answers to Exercises, cont.

* $\diff{x}^2 y = x - 1, \dd[y]{x}(0) = 1, P(1, 2)$
    * $y' = \frac{x^2}{2} - x + 1$
    * $y = \frac{x^3}{6} - \frac{x^2}{2} + x + \frac{4}{3}$
    * $y = \frac{x^3 - 3x^2 + 6x + 8}{6}$

---

## Answers to Exercises, cont.

* $v = 2t - 1$, find the distance traveled in $t \in [3, 5]$
    * $\int_3^5 v dt = \int_3^5 (2t - 1) dt$
    * $s = (5^2 - 5) - (3^2 - 3)$
    * $s = 5(2^2) - 3(2)$
    * $s = 20 - 6$
    * $s = 14\mathrm{m}$

---

## Answers to Exercises, cont.

* Solve $y'' + 16y = 0, x = \frac{\pi}{2}, y = 1, y' = 1$.
    * $y = A\sin 4x + B\cos 4x$
    * $1 = A\sin 2\pi + B\cos 2\pi$
    * $1 = B$
    * $1 = 4A\cos 2\pi - 4\sin 2\pi$
    * $A = \frac{1}{4}$
    * $y = \frac{1}{4}\sin 4x + \cos 4x$

---

## Answers to Exercises, cont.

* A spring with a mass of 0.5kg has a natural length of 0.1m. A force of 10N is required to stretch to 0.2m. If the spring is stretched to 3 times its normal length, what is the displacement of the mass at time $t$ after it is released from rest?
    * $F = kx$
    * $k = 100$
    * $(\frac{1}{2} \mathrm{kg})\ddot{x} = -(100 \left.\mathrm{N}\!\middle/\!\mathrm{m}\right.)x$
    * $(\frac{1}{2} \mathrm{kg})\ddot{x} + (100 \left.\mathrm{N}\!\middle/\!\mathrm{m}\right.)x = 0$

---

## Answers to Exercises, cont.

* A spring with a mass of 0.5kg has a natural length of 0.1m. A force of 10N is required to stretch to 0.2m. If the spring is stretched to 3 times its normal length, what is the displacement of the mass at time $t$ after it is released from rest?
    * $(\frac{1}{2} \mathrm{kg})\ddot{x} + (100 \left.\mathrm{N}\!\middle/\!\mathrm{m}\right.)x = 0$
    * $\ddot{x} + (200\mathrm{s}^{-2})x = 0$
    * $x = A \sin 10\sqrt{2} t + B \cos 10\sqrt{2} t$
    * $x = \frac{1}{5} \cos 10\sqrt{2} t$

---

# [Finish](../../../../)