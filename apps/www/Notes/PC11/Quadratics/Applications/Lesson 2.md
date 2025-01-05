---
marp: true
theme: uncover
class: invert
paginate: true
math: mathjax
---

# <!--fit--> Pre-Calculus 11 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2023-->

---

## Lesson 2: Applications, Part 2

---

## Example 1: Dimensions

* The area of a rectangular table is $45\text{ ft}^2$. The length is $4\text{ ft}$ more than the width. What are the dimensions of the table?
1) Define Variables:
    * $A=\text{area}$, $\ell=\text{length}$, $w=\text{width}$.
2) Write the formula for the situation
    * $A=\ell w$
3) Fill in the formula
    * What do we know?
        * $A=45,\ell=4+w$

---

## Solving Example 1, Part 1

* Work with new equation to determine factors: $45=(w+4)w$ 
    * $w^2+4w-45=0$
* We have many tools we can use, *which one?*
    * Graph
    * Square-Root Principle
    * Factoring
    * Quadratic Formula
* How about *factoring?*

---

## Solving Example 1, Part 2

* Remember: our equation is: $w^2+4w-45=0$
    * Let's try factoring the equation:
    * $(w+9)(w-5)=0$
* Now, let's solve for $w$.
    * $w+9=0,w-5=0$
    * $w=\{-9\text{ (ext)},5\}$
* $-9$ as an area is not possible. Since we cannot have a negative length, we call this an **extraneous root**.
* $\therefore D:5\text{ ft}\times9\text{ ft}$.

---

## Example 2: Object Heights

* The height, $h$, in feet of an object above the ground is given by $h=-16t^2+64t+190$, where $t$ is the time in seconds. 
* Find the time it takes the object to strike the ground.
* Find the maximum height of the object.
* We have our options. *Which one?*
    * Graph (inefficient)
    * S.R. Principle (works **only** w/ Binomials.)
    * Factor (large numbers)
    * Quadratic Formula (versatile)

---

## Solving Example 2, Part 1

* Given the size of the numbers, it's best to use the **Quad Formula** to solve.
    * It's very likely they're not clean numbers.
* $t=\frac{-(64)\pm\sqrt{64^2-4(-16*90)}}{2(-16)}$
* $t=\frac{-64\pm\sqrt{4096+12160}}{-32}$
* $t=\frac{-64\pm\sqrt{16256}}{-32}$
* $t=\frac{-64\pm127.4990}{-32}$

---

## Solving Example 2, Part 2

* $t=\{\frac{63.499}{-32},\frac{-191.499}{-32}\}$
* $t=\{-1.98\text{ (ext)},5.98\}$
* Since a negative time answer is extraneous, we can exclude it. $\therefore t=5.98s$.
* To find the maximum height, we need the vertex.
    * $h=-16(t^2-4t+c)+190-(-16c)$
    * $h=-16(t^2-4t+4)+190+64$
    * $h=-16(t-2)^2+254$
    * $\therefore \max(h)=254\text{ ft}$.

---

## Example 3: Multi-sectioned Area

* Two rectangular coralls are being made from $100 \text{ yds}$ of fencing. If the rancher wants to maximise the area, what dimensions should be used to make the corrals?
1) Define Variables
    * $\text{let }A=\text{area}, \ell=\text{length}, w=\text{width}, P=\text{perimeter}$
2) Make formulas
    * $A=\ell w, 100=3w+2\ell, 50-1.5w=\ell$
    * $A=w(50-1.5w)$
    * $A=-1.5w^2+50w$

---

## Solving Example 3

* $A=-1.5(w^2-33.\bar3+c)-(-1.5c)$
* $A=-1.5(w^2-33.\bar3+277.223)+415.834$
* $A=-1.5(w-16\frac{2}{3})^2+415.834$
* $w=16\frac{2}{3},\ell=25$
* $\therefore D:16\frac{2}{3}\text{ yds}\times25\text{ yds}$

---

# [Next Unit <i class="fa-solid fa-diagram-next"></i>](../../Rationals/Lesson%201%20(Basics).html)

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">