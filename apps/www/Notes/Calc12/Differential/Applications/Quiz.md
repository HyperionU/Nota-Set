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

# Unit 6 Practice Quiz

---

<!--paginate: true-->

## Questions

1. The height in metres from the ground of a falling object after $t$ seconds is $h(t) = -4.9t^2 + 5t + 85$
    * How long will it take to reach the ground?
    * What is the maximum speed of the object?
    * What is the velocity of the object after 2.5s?
    * What is the acceleration of the falling object?

---

## Questions, cont.

2. Find the unknown rate:
    * $V = \frac{4}{3}\pi\rho^3$
    * $\dot{V} = -6\text{m}^3\text{/s}$
    * when $\rho = 5\text{m}$, $\dot{\rho}$?
3. A drop of water creates a circular ripple that moves outwards at a rate of $20\text{cm/s}$. At what rate is the circumference increasing when the area is $1.0 \times 10^4 \text{cm}^2$?

---

## Questions, cont.

4. As the sun rises, the shadow cast by a 15m tree is decreasing at a rate of 55cm/hr. At what rate is the angle of elevation from the shadow to the sun increasing when the shadow is 15m in length?

---

## Question 1 Answers

1. The height in metres from the ground of a falling object after $t$ seconds is $h(t) = -4.9t^2 + 5t + 85$. How long will it take to reach the ground?
    * $h(t) = 0$
    * $-4.9t^2 + 5t + 85 = 0$
    * $t = \frac{-(5) \pm \sqrt{(5)^2 - 4(-4.9)(85)}}{2(-4.9)}, t \ge 0$
    * $t = \frac{-5 \pm \sqrt{25 + 1666}}{-9.8}, t \ge 0$
    * $t = \frac{5 \pm \sqrt{1691}}{9.8}, t \ge 0$
    * $t = 4.7\text{s}$

---

## Question 1 Answers, cont.

1. The height in metres from the ground of a falling object after $t$ seconds is $h(t) = -4.9t^2 + 5t + 85$. What is the maximum speed of the object?
    * $\diff{t} h(t) = \diff{t} (-4.9t^2 + 5t + 85)$
    * $\diff{t} h(t) = \diff{t} (-4.9t^2) + \diff{t} (5t) + \diff{t} (85)$
    * $\dot{h}(t) = v(t) = -9.8t + 5$
    * $v(4.7) = -9.8(4.7) + 5$
    * $v(4.7) = -41.1\text{m/s}$

---

## Question 1 Answers, cont.

1. The height in metres from the ground of a falling object after $t$ seconds is $h(t) = -4.9t^2 + 5t + 85$. What is the velocity of the object after 2.5s?
    * $v(t) = -9.8t + 5$
    * $v(2.5) = -9.8(2.5) + 5$
    * $v(2.5) = -19.5\text{m/s}$

---

## Question 1 Answers, cont.

1. The height in metres from the ground of a falling object after $t$ seconds is $h(t) = -4.9t^2 + 5t + 85$. What is the acceleration of the falling object?
    * $\diff{t} v(t) = \diff{t} (-9.8t + 5)$
    * $\diff{t} v(t) = \diff{t} (-9.8t) + \diff{t} (5)$
    * $\dot{v}(t) = a(t) = -9.8\text{m/s}^2$
    * $a(t) = -9.8\text{m/s}^2$

---

## Question 2 Answer

2. Find the unknown rate:
    * $V = \frac{4}{3}\pi\rho^3$
    * $\dot{V} = -6\text{m}^3\text{/s}$
    * when $\rho = 5\text{m}$, $\dot{\rho}$?
    * $\diff{t} V = \diff{t} (\frac{4}{3}\pi\rho^3)$
    * $\dot{V} = 3(\frac{4}{3}\pi\rho^2)\dot{\rho}$
    * $-6\text{m}^3\text{/s} = 4\pi(5\text{m})^2\dot{\rho}$
    * $-6\text{m}^3\text{/s} = 4\pi(25\text{m}^2)\dot{\rho}$
    * $-6\text{m}^3\text{/s} = (100\pi\text{m}^2)\dot{\rho}$

---

## Question 2 Answer

2. Find the unknown rate: $\dot{\rho}$
    * $-6\text{m}^3\text{/s} = (100\pi\text{m}^2)\dot{\rho}$
    * $\dot{\rho} = -\frac{6\text{m}^3\text{/s}}{100\pi\text{m}^2}$
    * $\dot{\rho} \approx -0.02\text{m/s}$

---

## Question 3 Answer

3. A drop of water creates a circular ripple that moves outwards at a rate of $20\text{cm/s}$. At what rate is the circumference increasing when the area is $1.0 \times 10^4 \text{cm}^2$?
    * $C = 2\pi r$
    * $\diff{t} C = \diff{t} (2\pi r)$
    * $\dot{C} = 2\pi\dot{r}$
    * $\dot{C} = 2\pi(20\text{cm/s})$
    * $\dot{C} = 40\pi\text{cm/s}$

---

## Question 4 Answer

4. As the sun rises, the shadow cast by a 15m tree is decreasing at a rate of 55cm/hr. At what rate is the angle of elevation from the shadow to the sun increasing when the shadow is 15m in length?
    * $h = 15\text{m}$
    * $\dot{l_s} = -55\text{cm/hr} = -0.55\text{m/hr}$
    * $\tan \theta = \frac{15\text{m}}{l_s}$
    * $\diff{t} (\tan \theta) = \diff{t} (\frac{15\text{m}}{l_s})$
    * $\frac{\dot{\theta}}{\cos^2 \theta} = -\frac{15\text{m}(\dot{l_s})}{l_s^2}$

---

## Question 4 Answer, cont

4. As the sun rises, the shadow cast by a 15m tree is decreasing at a rate of 55cm/hr. At what rate is the angle of elevation from the shadow to the sun increasing when the shadow is 15m in length?
    * $\dot{l_s} = -55\text{cm/hr} = -0.55\text{m/hr}$
    * $l_s = 15\text{m}$
    * $\frac{\dot{\theta}}{\cos^2 \theta} = -\frac{15\text{m}(\dot{l_s})}{l_s^2}$
    * $\dot{\theta} = -\frac{15\text{m}(-0.55\text{m/hr})}{(15\text{m})^2}\cos^2 \theta$

---

## Question 4 Answer, cont

4. As the sun rises, the shadow cast by a 15m tree is decreasing at a rate of 55cm/hr. At what rate is the angle of elevation from the shadow to the sun increasing when the shadow is 15m in length?
    * $h = 15\text{m}, l_s = h$
    * $\dot{\theta} = -\frac{15\text{m}(-0.55\text{m/hr})}{(15\text{m})^2}\cos^2 \theta$
    * $l_s^2 + h^2 = c^2$
    * $2(15\text{m})^2 = c^2$
    * $2(225\text{m}^2) = c^2$
    * $450\text{m}^2 = c^2$

---

## Question 4 Answer, cont

4. As the sun rises, the shadow cast by a 15m tree is decreasing at a rate of 55cm/hr. At what rate is the angle of elevation from the shadow to the sun increasing when the shadow is 15m in length?
    * $h = 15\text{m}, l_s = h$
    * $\dot{\theta} = -\frac{15\text{m}(-0.55\text{m/hr})}{(15\text{m})^2}\cos^2 \theta$
    * $450\text{m}^2 = c^2$
    * $15\sqrt{2}\text{m} = c$
    * $\dot{\theta} = -\frac{15\text{m}(-0.55\text{m/hr})}{(15\text{m})^2}(1 - \sin^2 \theta)$

---

## Question 4 Answer, cont

4. As the sun rises, the shadow cast by a 15m tree is decreasing at a rate of 55cm/hr. At what rate is the angle of elevation from the shadow to the sun increasing when the shadow is 15m in length?
    * $h = 15\text{m}$
    * $c = 15\sqrt{2}\text{m}$
    * $\dot{\theta} = -\frac{15\text{m}(-0.55\text{m/hr})}{(15\text{m})^2}(1 - \sin^2 \theta)$
    * $\sin \theta = \frac{15\text{m}}{15\sqrt{2}\text{m}}$
    * $\sin \theta = \frac{1}{\sqrt{2}}$

---

## Question 4 Answer, cont

4. As the sun rises, the shadow cast by a 15m tree is decreasing at a rate of 55cm/hr. At what rate is the angle of elevation from the shadow to the sun increasing when the shadow is 15m in length?
    * $\sin \theta = \frac{1}{\sqrt{2}}$
    * $\dot{\theta} = -\frac{15\text{m}(-0.55\text{m/hr})}{(15\text{m})^2}(1 - \sin^2 \theta)$
    * $\dot{\theta} = -\frac{15\text{m}(-0.55\text{m/hr})}{(15\text{m})^2}(1 - (\frac{1}{\sqrt{2}})^2)$
    * $\dot{\theta} = \frac{8.25\text{m}^2\text{/hr}}{225\text{m}^2}(1 - (\frac{1}{\sqrt{2}})^2)$

---

## Question 4 Answer, cont

4. As the sun rises, the shadow cast by a 15m tree is decreasing at a rate of 55cm/hr. At what rate is the angle of elevation from the shadow to the sun increasing when the shadow is 15m in length?
    * $\dot{\theta} = \frac{8.25\text{m}^2\text{/hr}}{225\text{m}^2}(1 - (\frac{1}{\sqrt{2}})^2)$
    * $\dot{\theta} = \frac{8.25}{225}(1 - \frac{1}{2}) \text{rad/hr}$
    * $\dot{\theta} = \frac{8.25}{225}(\frac{1}{2}) \text{rad/hr}$
    * $\dot{\theta} = \frac{8.25}{450}\text{rad/hr}$
    * $\dot{\theta} = \frac{825}{45000}\text{rad/hr}$

---

## Question 4 Answer, cont

4. As the sun rises, the shadow cast by a 15m tree is decreasing at a rate of 55cm/hr. At what rate is the angle of elevation from the shadow to the sun increasing when the shadow is 15m in length?
    * $\dot{\theta} = \frac{825}{45000}\text{rad/hr}$
    * $\dot{\theta} = \frac{11}{600}\text{rad/hr}$

---

# [Next Lesson](Lesson%204)