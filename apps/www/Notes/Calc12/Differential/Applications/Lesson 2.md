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

# Lesson 2: Rate of Change I: Area and Volume

---

<!--paginate: true-->

## Intro 

* While Calculus can be defined as "Math with infinity", this isn't the full picture.
* In fact, Calculus could be defined as "Math of Dynamic Systems".
* The topic of *Related Rates* is an excellent illustration of how we can use differentiation to discover information of dynamic relationships in geometry.

---

## Dynamic Quantities

* Consider a spherical balloon inflating with air. There are a number of dynamic quantites involved, including:
    * Volume
    * Radius
    * Surface Area
* Take for example the radius and volume. We know that the quantities are related via the formula for the volume: $V = \frac{4}{3}\pi\rho^3$

---

## Dynamic Quantities, cont.

* However, since the balloon is being inflated, these quantites are changing over time.
* Therefore, we have rates of change, which is where derivatives are involved.
* In order to change the volume formula to describe a dynamic system, we must use Implicit Differentiation.
* Time necessitates the introduction of a new variable into the process of differentiation.

---

## Staticism to Dynamicism

* Each variable or dynamic quantity must be differentiated with respect to time ($t$).
    * $\diff{t} V = \diff{t} \frac{4}{3}\pi(\rho^3)$
    * $\dot{V} = 4\pi\rho^2 \dot{\rho}$
* Note: $\pi$ is a constant.
* When inflating the balloon by mechanical means, it's easy to measure the rate the volume is increasing.
* However, it's not as easy to measure the rate the radius is increasing.

---

## Staticism to Dynamicism, cont.

* The method we used allows us to use rates we can easily measure, or obtain information about, to calculate rates that we struggle to measure directly.
* In general, we can use the following procedure:
    * Sketch and label a diagram
    * Define variables and rates
    * Relate known and desired quantities using formulae
    * Differentiate with respect to time
    * Substitute known quantities and solve for the desired rate.

---

## Example 1: Volume of a Sphere

1. Consider an inflating balloon. If the volume is increasing at a rate of $125\text{cm}^3\text{/s}$, calculate the rate which the radius increases when the radius is 10cm.
    * Let $V$ be volume, $r = 10\text{cm}$, $\dot{V} = 125\text{cm}^3\text{/s}$, $\dot{\rho} = ?$
    * Assume the balloon is a sphere.
    * $\diff{t} V = \diff{t} (\frac{4}{3}\pi\rho^3)$
    * $\dot{V} = \dot{\rho}(t) 4\pi\rho^2$ (Since the radius is dynamic, we can't substitute until *after* we differentiate.)
    * $125\text{cm}^3\text{/s} = \dot{\rho} 4\pi(10\text{cm})^2$  

---

## Example 1, cont.

1. Consider an inflating balloon. If the volume is increasing at a rate of $125\text{cm}^3\text{/s}$, calculate the rate which the radius increases when the radius is 10cm.
    * Let $V$ be volume, $r = 10\text{cm}$, $\dot{V} = 125\text{cm}^3\text{/s}$, $\dot{\rho} = ?$
    * $125\text{cm}^3\text{/s} = \dot{\rho}(t) 4\pi(10\text{cm})^2$ 
    * $125\text{cm}^3\text{/s} = \dot{\rho}(t) (400\pi\text{cm}^2)$ 
    * $\dot{\rho} = \frac{125\text{cm/s}}{400\pi}$
    * $\dot{\rho}(10\text{s}) = \frac{5}{16\pi}\text{cm/s}$

---

## Example 2: Cube's Surface Area

2. A cube is shrinking and maintaining its shape. If the side length is decreasing at a rate of $2\text{cm/s}$, what rate is the surface area decreasing when the side length is $25\text{cm}$
    * Let $A_c$ be the surface area, $s = 25\text{cm}$, $\dot{A_c} = ?, \dot{s} = -2\text{cm/s}$
    * $A_c = 6s^2$
    * $\diff{t} A_c = \diff{t} (6s^2)$
    * $\dot{A_c} = \dot{s}12s$

---

## Example 2, cont.

2. A cube is shrinking and maintaining its shape. If the side length is decreasing at a rate of $2\text{cm/s}$, what rate is the surface area decreasing when the side length is $25\text{cm}$
    * Let $A_c$ be the surface area, $s = 25\text{cm}$, $\dot{A_c} = ?, \dot{s} = -2\text{cm/s}$
    * $\dot{A_c} = \dot{s}12s$
    * $\dot{A_c} = 12(-2\text{cm/s})(25\text{cm})$
    * $\dot{A_c} = -600\text{cm}^2\text{/s}$

---

## Example 3: Sphere's Surface Area

3. The radius is decreasing at a rate of $3.5\text{cm/s}$. What is the rate of the surface area's change when the radius is $14\text{cm}$?
    * Let $A_s$ be the surface area, $\rho = 14\text{cm}$, $\dot{\rho} = -3.5 \text{cm/s}, \dot{A_s}$
    * $A_s = 4\pi\rho^2$
    * $\diff{t} A_s = \diff{t} (4\pi\rho^2)$
    * $\dot{A_s} = (8\pi\rho)\dot{\rho}$

---

## Example 3, cont.

3. The radius is decreasing at a rate of $3.5\text{cm/s}$. What is the rate of the surface area's change when the radius is $14\text{cm}$?
    * Let $A_s$ be the surface area, $\rho = 14\text{cm}$, $\dot{\rho} = -3.5 \text{cm/s}, \dot{A_s}$
    * $\dot{A_s} = (8\pi\rho)\dot{\rho}$
    * $\dot{A_s} = 8\pi(14\text{cm})(-3.5\text{cm/s})$
    * $\dot{A_s} = -392\pi\text{cm}^2\text{/s}$

---

## Example 4

4. A circle's area is changing at a rate of $-22\text{cm}^2\text{/s}$. What is the rate of change for the radius when the circumferance is $120\text{cm}$?
    * Let $A = \pi\rho^2$, $C = 2\pi\rho = 120\text{cm}$, $\dot{A} = -22\text{cm}^2\text{/s}, \dot{\rho} = ?$
    * $120\text{cm} = 2\pi\rho$
    * $\rho = \frac{60}{\pi}\text{cm}$
    * $A = \pi\rho^2$
    * $\diff{t} A = \diff{t} (\pi\rho^2)$
    * $\dot{A} = \dot{\rho}2\pi\rho$

---

## Example 4, cont.

4. A circle's area is changing at a rate of $-22\text{cm}^2\text{/s}$. What is the rate of change for the radius when the circumferance is $120\text{cm}$?
    * Let $A = \pi\rho^2$, $C = 2\pi\rho = 120\text{cm}$, $\dot{A} = -22\text{cm}^2\text{/s}, \dot{\rho} = ?, \rho = \frac{60}{\pi}\text{cm}$
    * $\dot{A} = \dot{\rho}2\pi\rho$
    * $-22\text{cm}^2/\text{s} = 2\pi(\frac{60}{\pi}\text{cm})\dot{\rho}$
    * $-22\text{cm}^2/\text{s} = 120\text{cm}(\dot{\rho})$
    * $\dot{\rho} = \frac{-22\text{cm}^2\text{/s}}{120\text{cm}}$

---

## Example 4, cont.

4. A circle's area is changing at a rate of $-22\text{cm}^2\text{/s}$. What is the rate of change for the radius when the circumferance is $120\text{cm}$?
    * $\dot{\rho} = \frac{-22\text{cm}^2\text{/s}}{120\text{cm}}$
    * $\dot{\rho} = -\frac{11}{60}\text{cm/s}$

---

## Example 5

5. A cylindrical water tank is filling at a rate of $1.5\text{m}^3\text{/min}$. If the tank has a radius of $2\text{m}$, what rate is the water level increasing when the water is $3.2\text{m}$ deep?
    * $V = \pi\rho^2 h, \rho = 2\text{m}, h = 3.2\text{m}, \dot{V} = 1.5\text{m}^3\text{/min}, \dot{h} = ?$
    * $V = \pi(2\text{m})^2 h$
    * $V = h\pi(4\text{m}^2)$
    * $\diff{t} V = \diff{t} (h\pi(4\text{m}^2))$
    * $\dot{V} = \dot{h}\pi(4\text{m}^2)$

---

## Example 5, cont.

5. A cylindrical water tank is filling at a rate of $1.5\text{m}^3\text{/min}$. If the tank has a radius of $2\text{m}$, what rate is the water level increasing when the water is $3.2\text{m}$ deep?
    * $h = 3.2\text{m}, \dot{V} = 1.5\text{m}^3\text{/min}, \dot{h} = ?$
    * $\dot{V} = \dot{h}\pi(4\text{m}^2)$
    * $1.5\text{m}^3\text{/min} = \dot{h}\pi(4\text{m}^2)$
    * $\dot{h} = \frac{1.5\text{m}^3\text{/min}}{\pi(4\text{m}^2)}$
    * $\dot{h} = \frac{15\text{m/min}}{40\pi}$
    * $\dot{h} = \frac{3}{8\pi}\text{m/min}$

---

## Example 6

6. Water is draining out of a cone-shaped tank at a rate of $2.5\text{m}^3\text{/min}$. The tank is $8\text{m}$ tall and has a top diameter of $5\text{m}$. What is the rate of change to the water level at $2.8\text{m}$?
    * $V = \frac{1}{3}\pi r^2h, d = 2r = 5\text{m}, h = 2.8\text{m}, h_t = 8\text{m}$ 
    * $\dot{V} = -2.5\text{m}^3\text{/min}, \dot{h} = ?$
    * $r = 2.5\text{m}$
    * Since the change to the radius isn't given, we can eliminate this variable.

---

## Example 6, cont.

6. Water is draining out of a cone-shaped tank at a rate of $2.5\text{m}^3\text{/min}$. What is the rate of change to the water level at $2.8\text{m}$?
    * $V = \frac{1}{3}\pi r^2h, r = 2.5\text{m}, h = 2.8\text{m}, h_t = 8\text{m}$ 
    * $\dot{V} = -2.5\text{m}^3\text{/min}, \dot{h} = ?$
    * We know that the ratio between the radius and height is constant.
    * $\frac{r}{h_t} = \frac{2.5\text{m}}{8\text{m}}$
    * $\frac{r}{h_t} = \frac{5}{16}$

---

## Example 6, cont.

6. Water is draining out of a cone-shaped tank at a rate of $2.5\text{m}^3\text{/min}$. What is the rate of change to the water level at $2.8\text{m}$?
    * $V = \frac{1}{3}\pi r^2h, r = 2.5\text{m}, h = 2.8\text{m}, h = 8\text{m}$ 
    * $\dot{V} = -2.5\text{m}^3\text{/min}, \dot{h} = ?$
    * $\frac{r}{h_t} = \frac{5}{16}$
    * $r = \frac{5}{16}h$
    * $V = \frac{1}{3}\pi (\frac{5}{16}h)^2 h$
    * $V = \frac{25\pi}{768}h^3$

---

## Example 6, cont.

6. Water is draining out of a cone-shaped tank at a rate of $2.5\text{m}^3\text{/min}$. What is the rate of change to the water level at $2.8\text{m}$?
    * $h = 2.8\text{m}, \dot{V} = -2.5\text{m}^3\text{/min}, \dot{h} = ?$
    * $V = \frac{25\pi}{768}h^3$
    * $\diff{t} V = \diff{t} (\frac{25\pi}{768}h^3)$
    * $\dot{V} = (\frac{25\pi}{256}h^2)\dot{h}$
    * $-2.5\text{m}^3\text{/min} = \frac{25\pi}{256}(2.8\text{m})^2\dot{h}$
    * $\dot{h} = \frac{-2.5\text{m}^3\text{/min}}{\frac{25\pi}{256}(2.8\text{m})^2}$

---

## Example 6, cont.

6. Water is draining out of a cone-shaped tank at a rate of $2.5\text{m}^3\text{/min}$. What is the rate of change to the water level at $2.8\text{m}$?
    * $\dot{h} = \frac{-2.5\text{m}^3\text{/min}(256)}{25\pi(2.8\text{m})^2}$
    * $\dot{h} = \frac{-2.5\text{m}^3\text{/min}(256)}{25\pi(7.84\text{m}^2)}$
    * $\dot{h} = -\frac{640\text{m}^3\text{/min}}{196\pi\text{m}^2}$
    * $\dot{h} = -\frac{640}{196\pi} \text{m/min}$
    * $\dot{h} = -\frac{160}{49\pi} \text{m/min}$

---

## Exercise for Readers

* For each of the following, find the desired rate:
    * $V = s^3, \dot{s} = 3\text{m/s}, \dot{V}(10\text{m})?$
    * $A = \pi\rho^2, \dot{A} = -1.2\text{m}^2\text{/s}, A = 15\text{m}^2, \dot{\rho}?$
* Area of a square is increasing at a rate of $20\text{cm}^2\text{/s}$. What is the rate of the side length when it is $200\text{cm}$?
* Volume of a spherical ball of snow is decreasing at a rate of $40\text{cm}^3\text{/s}$. What rate is the radius decreasing when it is $3.5\text{cm}$? Assume it melts uniformly.

---

## Exercise for Readers, cont.

* A landscaping company is pouring woodchips into a conical pile with a constant ratio of $2:5$ between the radius and height. The volume is increasing at a rate of $1.8\text{m}^3\text{/min}$. When the radius is $3\text{m}$, what rate is the height increasing?
* The volume of a cube is increasing at a rate of $6\text{m}^3\text{/s}$. At what rate is the side length increasing when the surface area is $40\text{m}^2$?

---

# [Next Lesson](Lesson%203)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Find the desired rate: $V = s^3, \dot{s} = 3\text{m/s}, \dot{V}(10\text{m})?$
    * $\diff{t} V = \diff{t} (s^3)$
    * $\dot{V} = 3s^2\dot{s}$
    * $\dot{V} = 3(10\text{m})^2(3\text{m/s})$
    * $\dot{V} = (100\text{m}^2)(9\text{m/s})$
    * $\dot{V} = 900\text{m}^3\text{s}$

---

## Answers to Exercises, cont.

* Find the desired rate: $A = \pi\rho^2, \dot{A} = -1.2\text{m}^2\text{/s}, A = 15\text{m}^2, \dot{\rho}?$
    * $15\text{m}^2 = \pi\rho^2$
    * $\rho = \sqrt{\frac{15}{\pi}}\text{m}$
    * $\diff{t} A = \diff{t}(\pi\rho^2)$
    * $\dot{A} = 2\pi\rho\dot{\rho}$
    * $-1.2\text{m}^2\text{/s} = 2\pi(\sqrt{\frac{15}{\pi}}\text{m})\dot{\rho}$
    * $-1.2\text{m}^2\text{/s} = \dot{\rho}\sqrt{60\pi}\text{m}$

---

## Answers to Exercises, cont.

* Find the desired rate: $A = \pi\rho^2, \dot{A} = -1.2\text{m}^2\text{/s}, A = 15\text{m}^2, \dot{\rho}?$
    * $-1.2\text{m}^2\text{/s} = \dot{\rho}\sqrt{60\pi}\text{m}$
    * $\dot{\rho} = \frac{-1.2\text{m}^2\text{/s}}{\sqrt{60\pi}\text{m}}$
    * $\dot{\rho} = \frac{-1.2}{\sqrt{60\pi}}\text{m/s}$
    * $\dot{\rho} = \frac{-0.6}{\sqrt{15\pi}}\text{m/s}$
    * $\dot{\rho} = \frac{-6}{10\sqrt{15\pi}}\text{m/s}$

---

## Answers to Exercises, cont.

* Area of a square is increasing at a rate of $20\text{cm}^2\text{/s}$. What is the rate of the side length when it is $200\text{cm}$?
    * $A = s^2$
    * $\diff{t} A = \diff{t} (s^2)$
    * $\dot{A} = 2\dot{s}(s)$
    * $-20\text{cm}^2\text{/s} = 2\dot{s}(200\text{cm})$
    * $-20\text{cm}^2\text{/s} = \dot{s}(400\text{cm})$
    * $\dot{s} = \frac{-20\text{cm}^2\text{/s}}{400\text{cm}}$
    * $\dot{s} = -\frac{1}{20}\text{cm/s}$

---

## Answers to Exercises, cont.

* Volume of a spherical ball of snow is decreasing at a rate of $40\text{cm}^3\text{/s}$. What rate is the radius decreasing when it is $3.5\text{cm}$? Assume it melts uniformly.
    * $V = \frac{4}{3}\pi\rho^3$
    * $\diff{t} V = \diff{t} (\frac{4}{3}\pi\rho^3)$
    * $\dot{V} = \dot{\rho} 4\pi\rho^2$
    * $-40\text{cm}^3\text{/s} = \dot{\rho} 4\pi(3.5\text{cm})^2$
    * $-40\text{cm}^3\text{/s} = \dot{\rho} 4\pi(12.25\text{cm}^2)$
    * $-40\text{cm}^3\text{/s} = \dot{\rho} \pi(49\text{cm}^2)$

---

## Answers to Exercises, cont.

* Volume of a spherical ball of snow is decreasing at a rate of $40\text{cm}^3\text{/s}$. What rate is the radius decreasing when it is $3.5\text{cm}$? Assume it melts uniformly.
    * $-40\text{cm}^3\text{/s} = \dot{\rho} \pi(49\text{cm}^2)$
    * $\dot{\rho} = \frac{-40\text{cm}^3\text{/s}}{49\pi\text{cm}^2}$
    * $\dot{\rho} = -\frac{40}{49\pi}\text{cm/s}$

---

## Answers to Exercises, cont.

* A landscaping company is pouring woodchips into a conical pile with a constant ratio of $2:5$ between the radius and height. The volume is increasing at a rate of $1.8\text{m}^3\text{/min}$. When the radius is $3\text{m}$, what rate is the height increasing?
    * $\frac{r}{h} = \frac{2}{5}$
    * $r = \frac{2}{5}h$
    * $V = \frac{1}{3}\pi r^2 h$
    * $V = \frac{1}{3}\pi (\frac{2}{5}h)^2 h$

---

## Answers to Exercises, cont.

* A landscaping company is pouring woodchips into a conical pile with a constant ratio of $2:5$ between the radius and height. The volume is increasing at a rate of $1.8\text{m}^3\text{/min}$. When the radius is $3\text{m}$, what rate is the height increasing?
    * $r = \frac{2}{5}h$
    * $V = \frac{1}{3}\pi (\frac{2}{5}h)^2 h$
    * $\diff{t} V = \diff{t} (\frac{1}{3}\pi (\frac{2}{5})^2 h^3)$
    * $\dot{V} = \dot{h} \pi (\frac{2}{5}h)^2$

---

## Answers to Exercises, cont.

* A landscaping company is pouring woodchips into a conical pile with a constant ratio of $2:5$ between the radius and height. The volume is increasing at a rate of $1.8\text{m}^3\text{/min}$. When the radius is $3\text{m}$, what rate is the height increasing?
    * $r = \frac{2}{5}h$
    * $\dot{V} = \dot{h} \pi (\frac{2}{5}h)^2$
    * $\dot{V} = \dot{h} \pi r^2$
    * $1.8\text{m}^3\text{/min} = \dot{h} \pi (3\text{m})^2$

---

## Answers to Exercises, cont.

* A landscaping company is pouring woodchips into a conical pile with a constant ratio of $2:5$ between the radius and height. The volume is increasing at a rate of $1.8\text{m}^3\text{/min}$. When the radius is $3\text{m}$, what rate is the height increasing?
    * $1.8\text{m}^3\text{/min} = \dot{h} \pi (3\text{m})^2$
    * $1.8\text{m}^3\text{/min} = \dot{h} 9\pi\text{m}^2$
    * $\dot{h} = \frac{1.8\text{m}^3\text{/min}}{9\pi\text{m}^2}$
    * $\dot{h} = \frac{1.8}{9\pi}\text{m/min}$

---

## Answers to Exercises, cont.

* A landscaping company is pouring woodchips into a conical pile with a constant ratio of $2:5$ between the radius and height. The volume is increasing at a rate of $1.8\text{m}^3\text{/min}$. When the radius is $3\text{m}$, what rate is the height increasing?
    * $\dot{h} = \frac{1.8}{9\pi}\text{m/min}$
    * $\dot{h} = \frac{18}{90\pi}\text{m/min}$
    * $\dot{h} = \frac{1}{5\pi}\text{m/min}$

---

## Answers to Exercises, cont.

* The volume of a cube is increasing at a rate of $6\text{m}^3\text{/s}$. At what rate is the side length increasing when the surface area is $40\text{m}^2$?
    * $V = s^3$
    * $A_s = 6s^2$
    * $\diff{t} V = \diff{t} (s^3)$
    * $\dot{V} = (3s^2)\dot{s}$
    * $2\dot{V} = 2(3s^2)\dot{s}$
    * $2\dot{V} = (6s^2)\dot{s}$

---

## Answers to Exercises, cont.

* The volume of a cube is increasing at a rate of $6\text{m}^3\text{/s}$. At what rate is the side length increasing when the surface area is $40\text{m}^2$?
    * $A_s = 6s^2$
    * $2\dot{V} = (6s^2)\dot{s}$
    * $2\dot{V} = A_s \dot{s}$
    * $2(6\text{m}^3\text{/s}) = 40\text{m}^2 \dot{s}$
    * $12\text{m}^3\text{/s} = 40\text{m}^2 \dot{s}$
    * $\dot{s} = \frac{12\text{m}^3\text{/s}}{40\text{m}^2}$

---

## Answers to Exercises, cont.

* The volume of a cube is increasing at a rate of $6\text{m}^3\text{/s}$. At what rate is the side length increasing when the surface area is $40\text{m}^2$?
    * $\dot{s} = \frac{12\text{m}^3\text{/s}}{40\text{m}^2}$
    * $\dot{s} = \frac{12}{40}\text{m/s}$
    * $\dot{s} = \frac{3}{10}\text{m/s}$

---

# [Next Lesson](Lesson%203)