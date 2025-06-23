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

# Lesson 1: Physical Applications

---

<!--paginate: true-->

## Intro 

* It's important to understand what a derivative represents when it comes to how to use them.
* For any function $f(x)$, its derivative $f'(x)$ represents the rate of change of the function for any value in the domain.

---

## Intro, cont.

* For Physics, the most significant usage of calculus is for kinematics.
* If we state that the function is expressing displacement ($s$), over some time $t$, the derivative is the change in displacement over time, or Velocity ($v$).
* Similarly, the derivative for velocity is its rate of change over time, or Acceleration ($a$).

---

## A Note on Notation

* Here's some notation you'll see throughout:
    * Displacement: $s$ or $s(t)$
    * Velocity: $v$, $v(t)$, $\dot{s}$ or $\dot{s}(t)$
    * Acceleration: $a$, $a(t)$, $\dot{v}$, $\dot{v}(t)$, $\ddot{s}$ or $\ddot{s}(t)$

---

## Kinematic Freefall

* The following represents the displacement, with respect to time, of an object thrown off a 250m cliff, in a downward direction at a velocity of 9m/s.
* $s(t) = -4.9t^2 - 9t + 250$
* For objects in freefall, we assume that the ground represents a displacement of zero, and any distance above has a positive displacement.

---

## Kinematic Freefall, cont.

* We can therefore represent the velocity as the first derivative of this function.
* $v(t) = \dot{s}(t) = -9.8t - 9$
* If we take the derivative again, we get the acceleration function.
* $a(t) = \dot{v}(t) = \ddot{s}(t) = -9.8$
* Since gravity is the force which produces a constant acceleration towards the Earth, the acceleration is a constant which doesn't change.

---

## Kinematic Freefall, cont.

* We can therefore represent the velocity as the first derivative of this function.
* $v(t) = \dot{s}(t) = -9.8t - 9$
* If we take the derivative again, we get the acceleration function.
* $a(t) = \dot{v}(t) = \ddot{s}(t) = -9.8$
* Since gravity is the force which produces a constant acceleration towards the Earth, the acceleration is a constant which doesn't change.

---

## Kinematic Freefall, cont.

* The sign of $a(t)$ indicates what $v(t)$ is doing.
* Since $a(t) < 0$ for the duration of the problem, the velocity must be decreasing at all points in time ($v(t)$ is *monotonically decreasing*).
* The velocity function can illustrate this point.
    * $v(0) = -9$
    * $v(1) = -18.8$
* For most cases, the basic kinematic function for objects in freefall is $s(t) = -\frac{a}{2}t^2 + v_0 t + s_0$

---

## Example 1

1. The function $s(t) = -4.9t^2 - 12t + 180$ represents the displacement of an object in freefall.
    * How long does it take for the object to reach the ground ($s(t) = 0$)?
    * What is the object's velocity just before impact and what is its maximum speed?
    * How long does it take to reach a downward speed of 20m/s ($v(t) = -20$)?
    * What is the velocity at 3s ($v(3)$)?
    * What is the maximum acceleration?

---

## Example 1, cont.

1. The function $s(t) = -4.9t^2 - 12t + 180$ represents the displacement of an object in freefall.
    * How long does it take for the object to reach the ground ($s(t) = 0$)?
        * $0 = -4.9t^2 - 12t + 180$
        * $t = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$
        * $t = \frac{12 \pm \sqrt{3672}}{-9.8}$
        * $t = \frac{12 + \sqrt{3672}}{-9.8} = -7.41\text{s}$
        * $t = \frac{12 - \sqrt{3672}}{-9.8} = 4.96\text{s}$

---

## Example 1, cont.

1. The function $s(t) = -4.9t^2 - 12t + 180$ represents the displacement of an object in freefall.
    * What is the object's velocity just before impact and what is its maximum speed?
        * $\diff{t} s(t) = \diff{t} (-4.9t^2 - 12t + 180)$
        * $\diff{t} s(t) = \diff{t} (-4.9t^2) - \diff{t} (12t) + \diff{t} (180)$
        * $v(t) = \dot{s}(t) = -9.8t - 12$
        * $v(4.96) = -9.8(4.96) - 12$
        * $v(4.96) = -60.6\text{m/s}$

---

## Example 1, cont.

1. The function $s(t) = -4.9t^2 - 12t + 180$ represents the displacement of an object in freefall.
    * How long does it take to reach a downward speed of 20m/s ($v(t) = -20$)?
        * $v(t) = -9.8t - 12$
        * $-20 = -9.8t - 12$
        * $-8 = -9.8t$
        * $t = 0.82\text{s}$

---

## Example 1, cont.

1. The function $s(t) = -4.9t^2 - 12t + 180$ represents the displacement of an object in freefall.
    * What is the velocity at 3s ($v(3)$)?
        * $v(t) = -9.8t - 12$
        * $v(3) = -9.8(3) - 12$
        * $v(3) = -41.4\text{m/s}$

---

## Example 1, cont.

1. The function $s(t) = -4.9t^2 - 12t + 180$ represents the displacement of an object in freefall.
    * What is the maximum acceleration?
        * $v(t) = -9.8t - 12$ 
        * $\diff{t} v(t) = \diff{t} (-9.8t - 12)$
        * $\diff{t} v(t) = \diff{t} (-9.8t) - \diff{t} (12)$
        * $a(t) = \dot{v}(t) = -9.8$

---

## Example 2

2. On some distant planet, the function $s(t) = -3.2t^2 + 2.5t + 70$ represents the displacement of an object in freefall.
    * How long does it take for the object to reach the ground ($s(t) = 0$)?
    * What is the object's velocity at 1.5s ($v(1.5)$)?
    * What is the object's maximum speed? 
    * What is the acceleration due to gravity ($a(t)$)?

---

## Example 2, cont.

2. On some distant planet, the function $s(t) = -3.2t^2 + 2.5t + 70$ represents the displacement of an object in freefall.
    * How long does it take for the object to reach the ground ($s(t) = 0$)?
        * $0 = -3.2t^2 + 2.5t + 70$
        * $t = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$
        * $t = \frac{2.5 \pm \sqrt{902.25}}{6.4}$
        * $t = 5.1\text{s}$

---

## Example 2, cont.

2. On some distant planet, the function $s(t) = -3.2t^2 + 2.5t + 70$ represents the displacement of an object in freefall.
    * What is the object's velocity at 1.5s ($v(1.5)$)?
        * $s(t) = -3.2t^2 + 2.5t + 70$
        * $\diff{t} s(t) = \diff{t} (-3.2t^2 + 2.5t + 70)$
        * $\diff{t} s(t) = \diff{t} (-3.2t^2) + \diff{t} (2.5t) + \diff{t} (70)$
        * $v(t) = \dot{s}(t) = -6.4t + 2.5$
        * $v(1.5) = -6.4(1.5) + 2.5$
        * $v(1.5) = -7.1\text{m/s}$

---

## Example 2, cont.

2. On some distant planet, the function $s(t) = -3.2t^2 + 2.5t + 70$ represents the displacement of an object in freefall.
    * What is the object's maximum speed?
        * $v(t) = -6.4t + 2.5$
        * $v(5.1) = -6.4(5.1) + 2.5$
        * $v(5.1) = -30.1\text{m/s}$

---

## Example 2, cont.

2. On some distant planet, the function $s(t) = -3.2t^2 + 2.5t + 70$ represents the displacement of an object in freefall.
    * What is the acceleration due to gravity ($a(t)$)?
        * $v(t) = -6.4t + 2.5$
        * $\diff{t} v(t) = \diff{t} (-6.4t + 2.5)$
        * $\diff{t} v(t) = \diff{t} (-6.4t) + \diff{t} (2.5)$
        * $a(t) = \dot{v}(t) = -6.4$

---

## Exercise for Readers

* A bullet is fired straight up into the air at a speed of 900m/s. The equation relating its height is $h(t) = -4.9t^2 + 900t + 2.4$
    * How long does it take for the bullet to hit the ground?
    * What are the extrema values for the velocity of the bullet?
    * What is the bullet's velocity after 60s (Magnitude & Direction)?

---

## Exercise for Readers, cont.

* On the moon, an object is dropped straight down a crater 150m deep. The height of the object is $h(t) = -0.8t^2 + 150$
    * What is the maximum speed of the object?
    * What is the acceleration due to gravity?

---

## Exercise for Readers, cont.

* On three different planets, the following express the height of an object dropped from 200m:
* Neptune: $h_n(t) = -5.88t^2 - 8t + 200$
* Mars: $h_m(t) = -1.85t^2 - 8t + 200$
* Venus: $h_v(t) = -4.45t^2 - 8t + 200$
    * What is the acceleration due to gravity for each planet?
    * What is the maximum speed of the object on Venus?
    * How much faster is the maximum speed of the object on Neptune compared to Mars?

---

# [Next Lesson](Lesson%202)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* A bullet is fired straight up into the air at a speed of 900m/s. The equation relating its height is $h(t) = -4.9t^2 + 900t + 2.4$
    * How long does it take for the bullet to hit the ground?
        * $0 = -4.9t^2 + 900t + 2.4$
        * $t = \frac{900 \pm 900}{9.8}$
        * $t = 183.7\text{s}$

---

## Answers to Exercises, cont.

* A bullet is fired straight up into the air at a speed of 900m/s. The equation relating its height is $h(t) = -4.9t^2 + 900t + 2.4$
    * What are the extrema values for the velocity of the bullet?
        * $\diff{t} h(t) = \diff{t} (-4.9t^2 + 900t + 2.4)$
        * $\diff{t} h(t) = \diff{t} (-4.9t^2) + \diff{t} (900t) + \diff{t} (2.4)$
        * $v(t) = -9.8t + 900$
        * $v(183.7) = -9.8(183.7) + 900$
        * $v(183.7) = -900.26\text{m/s}$

---

## Answers to Exercises, cont.

* A bullet is fired straight up into the air at a speed of 900m/s. The equation relating its height is $h(t) = -4.9t^2 + 900t + 2.4$
    * What is the bullet's velocity after 60s (Magnitude & Direction)?
        * $\vec{v}(t) = -9.8t + 900$ 
        * $\vec{v}(60) = -9.8(60) + 900$ 
        * $\vec{v}(60) = 312\text{m/s [Up]}$ 

---

## Answers to Exercises, cont.

* On the moon, an object is dropped straight down a crater 150m deep. The height of the object is $h(t) = -0.8t^2 + 150$
    * What is the maximum speed of the object?
        * $0 = -0.8t^2 + 150$
        * $150 = 0.8t^2$
        * $t^2 = 187.5$
        * $t = 13.69$

---

## Answers to Exercises, cont.

* On the moon, an object is dropped straight down a crater 150m deep. The height of the object is $h(t) = -0.8t^2 + 150$
    * What is the maximum speed of the object?
        * $t = 13.69$
        * $\diff{t} h(t) = \diff{t} (-0.8t^2 + 150)$
        * $\diff{t} h(t) = \diff{t} (-0.8t^2) + \diff{t} (150)$
        * $v(t) = -1.6t$
        * $v(13.69) = -1.6(13.69)$
        * $v(13.69) = 21.9\text{m/s [Down]}$

---

## Answers to Exercises, cont.

* On the moon, an object is dropped straight down a crater 150m deep. The height of the object is $h(t) = -0.8t^2 + 150$
    * What is the acceleration due to gravity?
        * $v(t) = -1.6t$
        * $\diff{t} v(t) = \diff{t} (-1.6t)$
        * $a(t) = -1.6\text{m/s}^2$

---

## Answers to Exercises, cont.

* On three different planets, the following express the height of an object dropped from 200m:
* Neptune: $h_n(t) = -5.88t^2 - 8t + 200$
* Mars: $h_m(t) = -1.85t^2 - 8t + 200$
* Venus: $h_v(t) = -4.45t^2 - 8t + 200$
    * What is the acceleration due to gravity for Neptune?
        * $\diff{t}^2 h_n(t) = \diff{t}^2 (-5.88t^2 - 8t + 200)$
        * $\diff{t} (\diff{t} h_n(t)) = \diff{t} (\diff{t} (-5.88t^2) - \diff{t} (8t) + \diff{t} (200))$
        * $\diff{t} \dot{h_n}(t) = \diff{t} (-11.76t - 8)$
        * $\diff{t} \dot{h_n}(t) = \diff{t} (-11.76t) - \diff{t} (8)$

---

## Answers to Exercises, cont.

* On three different planets, the following express the height of an object dropped from 200m:
* Neptune: $h_n(t) = -5.88t^2 - 8t + 200$
* Mars: $h_m(t) = -1.85t^2 - 8t + 200$
* Venus: $h_v(t) = -4.45t^2 - 8t + 200$
    * What is the acceleration due to gravity for Neptune?
        * $\diff{t} \dot{h_n}(t) = \diff{t} (-11.76t) - \diff{t} (8)$
        * $\ddot{h_n}(t) = -11.76$
        * $a_n(t) = -11.76$

---

## Answers to Exercises, cont.

* On three different planets, the following express the height of an object dropped from 200m:
* Neptune: $h_n(t) = -5.88t^2 - 8t + 200$
* Mars: $h_m(t) = -1.85t^2 - 8t + 200$
* Venus: $h_v(t) = -4.45t^2 - 8t + 200$
    * What is the acceleration due to gravity for Mars?
        * $\diff{t}^2 h_m(t) = \diff{t}^2 (-5.88t^2 - 8t + 200)$
        * $\diff{t} (\diff{t} h_m(t)) = \diff{t} (\diff{t} (-1.85t^2) - \diff{t} (8t) + \diff{t} (200))$
        * $\diff{t} \dot{h_m}(t) = \diff{t} (-3.70t - 8)$
        * $\diff{t} \dot{h_m}(t) = \diff{t} (-3.70t) - \diff{t} (8)$

---

## Answers to Exercises, cont.

* On three different planets, the following express the height of an object dropped from 200m:
* Neptune: $h_n(t) = -5.88t^2 - 8t + 200$
* Mars: $h_m(t) = -1.85t^2 - 8t + 200$
* Venus: $h_v(t) = -4.45t^2 - 8t + 200$
    * What is the acceleration due to gravity for Mars?
        * $\diff{t} \dot{h_m}(t) = \diff{t} (-3.70t) - \diff{t} (8)$
        * $\ddot{h_m}(t) = -3.70$
        * $a_m(t) = -3.70$

---

## Answers to Exercises, cont.

* On three different planets, the following express the height of an object dropped from 200m:
* Neptune: $h_n(t) = -5.88t^2 - 8t + 200$
* Mars: $h_m(t) = -1.85t^2 - 8t + 200$
* Venus: $h_v(t) = -4.45t^2 - 8t + 200$
    * What is the acceleration due to gravity for Venus?
        * $\diff{t}^2 h_v(t) = \diff{t}^2 (-4.45t^2 - 8t + 200)$
        * $\diff{t} (\diff{t} h_v(t)) = \diff{t} (\diff{t} (-4.45t^2) - \diff{t} (8t) + \diff{t} (200))$
        * $\diff{t} \dot{h_v}(t) = \diff{t} (-8.90t - 8)$
        * $\diff{t} \dot{h_v}(t) = \diff{t} (-8.90t) - \diff{t} (8)$

---

## Answers to Exercises, cont.

* On three different planets, the following express the height of an object dropped from 200m:
* Neptune: $h_n(t) = -5.88t^2 - 8t + 200$
* Mars: $h_m(t) = -1.85t^2 - 8t + 200$
* Venus: $h_v(t) = -4.45t^2 - 8t + 200$
    * What is the acceleration due to gravity for Venus?
        * $\diff{t} \dot{h_v}(t) = \diff{t} (-8.90t) - \diff{t} (8)$
        * $\ddot{h_v}(t) = -8.90$
        * $a_v(t) = -8.90$

---

## Answers to Exercises, cont.

* On three different planets, the following express the height of an object dropped from 200m:
* Neptune: $h_n(t) = -5.88t^2 - 8t + 200$
* Mars: $h_m(t) = -1.85t^2 - 8t + 200$
* Venus: $h_v(t) = -4.45t^2 - 8t + 200$
    * What is the maximum speed of the object on Venus?
        * $0 = -4.45t^2 - 8t + 200$
        * $t = 5.87$
        * $\dot{h_v}(5.87) = -8.90(5.87) - 8$
        * $\dot{h_v}(5.87) = -60.24\text{m/s}$

---

## Answers to Exercises, cont.

* On three different planets, the following express the height of an object dropped from 200m:
* Neptune: $h_n(t) = -5.88t^2 - 8t + 200$
* Mars: $h_m(t) = -1.85t^2 - 8t + 200$
* Venus: $h_v(t) = -4.45t^2 - 8t + 200$
    * How much faster is the maximum speed of the object on Neptune compared to Mars?
        * $0 = -5.88t^2 - 8t + 200$
        * $t = 5.18$

---

## Answers to Exercises, cont.

* On three different planets, the following express the height of an object dropped from 200m:
* Neptune: $h_n(t) = -5.88t^2 - 8t + 200$
* Mars: $h_m(t) = -1.85t^2 - 8t + 200$
* Venus: $h_v(t) = -4.45t^2 - 8t + 200$
    * How much faster is the maximum speed of the object on Neptune compared to Mars?
        * $0 = -1.85t^2 - 8t + 200$
        * $t = 8.46$

---

## Answers to Exercises, cont.

* On three different planets, the following express the height of an object dropped from 200m:
* Neptune: $h_n(t) = -5.88t^2 - 8t + 200$
* Mars: $h_m(t) = -1.85t^2 - 8t + 200$
* Venus: $h_v(t) = -4.45t^2 - 8t + 200$
    * How much faster is the maximum speed of the object on Neptune compared to Mars?
        * $v_n(5.18) = -11.76(5.18) - 8$
        * $v_n(5.18) = -68.9$

---

## Answers to Exercises, cont.

* On three different planets, the following express the height of an object dropped from 200m:
* Neptune: $h_n(t) = -5.88t^2 - 8t + 200$
* Mars: $h_m(t) = -1.85t^2 - 8t + 200$
* Venus: $h_v(t) = -4.45t^2 - 8t + 200$
    * How much faster is the maximum speed of the object on Neptune compared to Mars?
        * $v_m(8.46) = -3.70(8.46) - 8$
        * $v_m(8.46) = -39.3$

---

## Answers to Exercises, cont.

* On three different planets, the following express the height of an object dropped from 200m:
* Neptune: $h_n(t) = -5.88t^2 - 8t + 200$
* Mars: $h_m(t) = -1.85t^2 - 8t + 200$
* Venus: $h_v(t) = -4.45t^2 - 8t + 200$
    * How much faster is the maximum speed of the object on Neptune compared to Mars?
        * $v_n = -68.9$
        * $v_m = -39.3$
        * It is $\times 1.75$ faster on Neptune than Mars.

---

# [Next Lesson](Lesson%202)