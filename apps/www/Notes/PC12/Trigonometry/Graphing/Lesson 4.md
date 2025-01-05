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

# Lesson 4: Applications

---

## Congruent Equations

Write an equation that gives the same graph as $y = 2 \sin 3x$.

* There's an infinite amount similar to this one: 
* $y = 2 \sin (3(x \pm \pi n)), n \mod 2 = 0$
* How about cosine?
* $y = 2 \cos 3(x - \frac{\pi}{6})$

---

## Equation from Extrema Points

A cosine curve has a maximum at $(2, 3)$, with the closest minimum at $(6, -7)$. Find a possible equation.

1. Determine $\alpha$.
    * $\frac{|y_1| + |y_2|}{2}$
    * $\alpha = 5$
2. Since it's a cosine graph, we can use the maximum to determine $\rho$
    * $\rho = 2$

$y = 5 \cos\beta(x - 2) + \delta$

---

## Equation from Extrema, cont.

$y = 5 \cos\beta(x - 2) + \delta$, min: $(6, -7)$, max: $(2, 3)$

3. Determine $\delta$
    * $y_{max} - \alpha$
    * After evaluating this, we get $\delta = -2$
4. Determine $\beta$
    * Since we have half of the period, we can take $2 (x_{max} + x_{min})$ to get the whole period.
    * $P = 8$, then just take $\frac{2\pi}{P}$, which gives us $\beta = \frac{\pi}{4}$

$y = 5 \cos\frac{\pi}{4}(x - 2) - 2$

---

## Applications of Trig Functions

The previous examples are cool, but what about actual applications?

* Tidal heights,
* Ferris wheels,
* Springs,
* Sunrise / sunsets,
* Pendula (pendulums),
* Heights of wheels, etc.

---

## Tidal Example

High tide is $14\text{m}$ at 6 hours, and the next low tide is $2\text{m}$ at 12.4 hours.
1. Determine an equation of this sinusoidal function
    * Use the skills from determining equations from extrema.
2. At 10 hours, what is the depth?
3. When is the first time the water is at $9\text{m}$? [desmos]
4. How long is the water above $9\text{m}$? [desmos]

---

## Tidal Answers

1. $h(t) = 6 \cos(\frac{1}{2}(t - 6)) + 8$
2. $h(10) = 5.5\text{m}$
3. There's a way to solve this algebraically, but $t = 3.19 \text{hrs}$
4. $11.44\text{hrs}$

---

# [Next Unit <i class="fa-solid fa-diagram-next"></i>](../Identities/Lesson%201%20(Definitions).html)

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">