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

$\newcommand\dd[3][]{\displaystyle\frac{d^{#1}#2}{d#3^{#1}}}$

---

# Lesson 5: Optimization Problems

---

<!--paginate: true-->

## Intro 

* Often, we need to find conditions that allow us to maximise or minimise a particular quantity.
* For example, we may want to maximise the area or volume, given a particular quantity of material.
* Another example would be to minimise the required materials and hence, the cost, given a set area.
* Since we can use derivatives to calculate extrema values, we can use calculus to find the optimum values for the types of problems outlined above.

---

## Example 1: Numerical

1. Two numbers have a difference of 3. What is the minimum product these two numbers can have?
    * Let $x, y$ be two numbers, such that $x - y = 3$.
    * Let $P = xy$.
    * We can state that $y = x - 3$.
    * Meaning $P = x(x - 3)$
    * $P = x^2 - 3x$

---

## Example 1, cont.

1. Two numbers have a difference of 3. What is the minimum product these two numbers can have?
    * $P = x^2 - 3x$
    * $\diff{x} P = \diff{x} (x^2 - 3x)$
    * $\diff{x} P = \diff{x} (x^2) - \diff{x} (3x)$
    * $\dd{P}{x} = 2x - 3$
    * CV: $x = \frac{3}{2}$
    * $\dd{P}{x} = 2x - 3$
    * $\dd{P}{x} = 2x - 3$

---

## Example 1, cont.

1. Two numbers have a difference of 3. What is the minimum product these two numbers can have?
    * $P = x^2 - 3x$
    * $\dd{P}{x} = 2x - 3$
    * CV: $x = \frac{3}{2}$
    * $\dd{P}{x}(0) = -$ (Dec.)
    * $\dd{P}{x}(2) = +$ (Inc.)

---

## Example 1, cont.

1. Two numbers have a difference of 3. What is the minimum product these two numbers can have?
    * $P = x^2 - 3x$
    * $x = \frac{3}{2}$
    * $P = (\frac{3}{2})^2 - 3(\frac{3}{2})$
    * $P = -\frac{9}{4}$
* Minimum product of two numbers with a difference of 3 is $-\frac{9}{4}$

---

## Example 2: Area

2. A family wants to build a fenced pen for their pet rabbits. The pen is to be built against their house, with 3 sides of fence and the house forming a rectangular pen. If they have 24m of fencing, what is the maximum area that they can make the pen?
    * Let $l$ be the length, and $w$ be the width.
    * Let $A = lw$.
    * The total length is $24 = l + 2w$
    * $l = 24 - 2w$

---

## Example 2, cont.

2. If they have 24m of fencing, what is the maximum area that they can make the pen?
    * $A = lw$    
    * $l = 24 - 2w$
    * $A = (24 - 2w)w$ 
    * $A = 24w - 2w^2$
    * $\diff{x} A = \diff{x} (24w - 2w^2)$
    * $\diff{w} A = \diff{w} (24w) - \diff{w} (2w^2)$
    * $\dd{A}{w} = 24 - 4w$

---

## Example 2, cont.

2. If they have 24m of fencing, what is the maximum area that they can make the pen? 
    * $A = 24w - 2w^2$
    * $\dd{A}{w} = 24 - 4w$
    * CV: $w = 6$
    * $\dd{A}{w}(0) = +$ (Inc.)
    * $\dd{A}{w}(7) = -$ (Dec.)

---

## Example 2, cont.

2. If they have 24m of fencing, what is the maximum area that they can make the pen? 
    * $A = 24w - 2w^2$
    * $w = 6$
    * $A = 24(6) - 2(6)^2$
    * $A = 144 - 72$
    * $A = 72\text{m}^2$

---

## Example 3: Dimensions

3. A box with a square base and an open top must have a volume of $108 000\text{cm}^3$. What dimensions minimise the material required to make the box?
    * Let $s$ be the length and width, and $h$ be the height.
    * Let $A_S = A_b + 4A_s$.
    * $A_S = s^2 + 4hs$.
    * Let $V = s^2h$.
    * $108000 = s^2h$.
    * $\frac{108000}{s^2} = h$.

---

## Example 3, cont.

3. A box with a square base and an open top must have a volume of $108 000\text{cm}^3$. What dimensions minimise the material required to make the box?
    * $A_S = s^2 + 4hs$
    * $\frac{108000}{s^2} = h$
    * $A_S = s^2 + 4(\frac{108000}{s^2})s$
    * $A_S = s^2 + \frac{432000}{s}$
    * $A_S = s^2 + 432000s^{-1}$

---

## Example 3, cont.

3. A box with a square base and an open top must have a volume of $108 000\text{cm}^3$. What dimensions minimise the material required to make the box?
    * $\frac{108000}{s^2} = h$
    * $A_S = s^2 + 432000s^{-1}$
    * $\diff{s} A_S = \diff{s} (s^2 + 432000s^{-1})$
    * $\diff{s} A_S = \diff{s} (s^2) + \diff{s} (432000s^{-1})$
    * $\dd{A_S}{s} = 2s - (432000s^{-2})$
   
---

## Example 3, cont.

3. A box with a square base and an open top must have a volume of $108 000\text{cm}^3$. What dimensions minimise the material required to make the box?
    * $\frac{108000}{s^2} = h$
    * $\dd{A_S}{s} = 2s - (432000s^{-2})$
    * $\dd{A_S}{s} = 2s - \frac{432000}{s^2}$
    * $2s = \frac{432000}{s^2}$
    * $2s^3 = 432000$

---

## Example 3, cont.

3. A box with a square base and an open top must have a volume of $108 000\text{cm}^3$. What dimensions minimise the material required to make the box?
    * $\frac{108000}{s^2} = h$
    * CV: $s = 60$

---

## Example 3, cont.

3. A box with a square base and an open top must have a volume of $108 000\text{cm}^3$. What dimensions minimise the material required to make the box?
    * $\frac{108000}{s^2} = h$
    * CV: $s = 60$
    * $\dd{A_S}{s}(1) = -$ (Dec.)
    * $\dd{A_S}{s}(100) = +$ (Inc.)

---

## Example 3, cont.

3. A box with a square base and an open top must have a volume of $108 000\text{cm}^3$. What dimensions minimise the material required to make the box?
    * $s = 60$
    * $\frac{108000}{s^2} = h$
    * $\frac{108000}{60^2} = h$
    * $h = 30$
    * Dimensions: Side length of 60cm and height of 30cm.

---

## Exercise for Readers

* Find 2 positive numbers whose product is 100. Minimise their sum.
* Find the dimensions of a rectangle whose area is $8000\text{cm}^2$, and whose perimeter is as small as possible.
* Find the maximum area of a triangle inscribed in a semicircle of diameter 40 cm.

---

# [Practice Quiz](Quiz)

Or

# [Next Lesson](Lesson%206)

<!--_footer: Next page for exercise answers! -->

---

## Exercise for Readers

* Find 2 positive numbers whose product is 100. Minimise their sum.
    * $P = xy = 100$
    * $S = x + y$
    * $y = \frac{100}{x}$
    * $S = x + \frac{100}{x}$
    * $\diff{x} S = \diff{x} (x + \frac{100}{x})$
    * $\diff{x} S = \diff{x} (x) + \diff{x} (\frac{100}{x})$
    * $\dd{S}{x} = 1 - \frac{100}{x^2}$

---

## Exercise for Readers, cont.

* Find 2 positive numbers whose product is 100. Minimise their sum.
    * $\dd{S}{x} = 1 - \frac{100}{x^2}$
    * $1 - \frac{100}{x^2} = 0$
    * $\frac{100}{x^2} = 1$
    * $\sqrt{100} = \not\sqrt{x^{\not2}}$
    * $x = 10$
    * $S = 10 + \frac{100}{10}$
    * $S = 20$

---

## Exercise for Readers, cont.

* Find the dimensions of a rectangle whose area is $8000\text{cm}^2$, and whose perimeter is as small as possible.
    * $A = \ell w = 8000\text{cm}^2$
    * $P = 2(\ell + w)$
    * $\ell = \frac{8000}{w}$
    * $P = 2(\frac{8000}{w} + w)$
    * $P = \frac{16000}{w} + 2w$
    * $\diff{w} P = \diff{w} (\frac{16000}{w} + 2w)$
    * $\dd{P}{w} = 2 - \frac{16000}{w^2}$

---

## Exercise for Readers, cont.

* Find the dimensions of a rectangle whose area is $8000\text{cm}^2$, and whose perimeter is as small as possible.
    * $\ell = \frac{8000}{w}$
    * $\dd{P}{w} = 2 - \frac{16000}{w^2}$
    * $2 - \frac{16000}{w^2} = 0$
    * $\frac{16000}{w^2} = 2$
    * $8000 = w^2$
    * $\sqrt{8000} = \not\sqrt{w^{\not2}}$
    * $w = 40\sqrt{5}$

---

## Exercise for Readers, cont.

* Find the dimensions of a rectangle whose area is $8000\text{cm}^2$, and whose perimeter is as small as possible.
    * $w = 40\sqrt{5}$
    * $\ell = \frac{8000}{40\sqrt{5}}$
    * $\ell = 40\sqrt{5}$
    * dim: $40\sqrt{5} \times 40\sqrt{5}$

---

## Exercise for Readers, cont.

* Find the maximum area of a triangle inscribed in a semicircle of diameter 40 cm.
* *This may seem hard, but I promise this will make sense.*
    * $\sin \vartheta = \frac{\beta}{40}$
    * $\cos \vartheta = \frac{\eta}{40}$
    * $A = \frac{1}{2}\beta\eta$
    * $A = \frac{1}{2}(40\sin \vartheta)(40 \cos \vartheta)$

---

## Exercise for Readers, cont.

* Find the maximum area of a triangle inscribed in a semicircle of diameter 40 cm.
    * $\beta = 40 \sin \vartheta$
    * $\eta = 40 \cos \vartheta$
    * $0 \le \vartheta \le \frac{\pi}{2}$
    * $A = \frac{(40\sin \vartheta)(40 \cos \vartheta)}{2}$
    * $A = \frac{1600\sin \vartheta \cos \vartheta}{2}$
    * $A = 800\sin \vartheta \cos \vartheta$
    * $A = 400\sin 2\vartheta$
    * $\diff{\vartheta} A = \diff{\vartheta} 400\sin 2\vartheta$

---

## Exercise for Readers, cont.

* Find the maximum area of a triangle inscribed in a semicircle of diameter 40 cm.
    * $A = 400\sin 2\vartheta$
    * $\diff{\vartheta} A = \diff{\vartheta} 400\sin 2\vartheta$
    * $\diff{\vartheta} A = \diff{\varphi} 400\sin \varphi (\diff{\vartheta} 2\vartheta)$
    * $\dd{A}{\vartheta} = 800\cos 2\vartheta$
    * $0 \le \vartheta \le \frac{\pi}{2}$
    * $\cos 2\vartheta = 0$
    * $\vartheta = \frac{\pi}{4}$

---

## Exercise for Readers, cont.

* Find the maximum area of a triangle inscribed in a semicircle of diameter 40 cm.
    * $A = 400\sin 2\vartheta$
    * $\vartheta = \frac{\pi}{4}$
    * $A = 400\sin 2\frac{\pi}{4}$
    * $A = 400\text{cm}^2$
* *See, that wasn't so hard.*
    
---

# [Practice Quiz](Quiz)

Or

# [Next Lesson](Lesson%206)