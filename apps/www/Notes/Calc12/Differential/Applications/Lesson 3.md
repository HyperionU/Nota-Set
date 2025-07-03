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

# Lesson 3: Rate of Change II: Triangles

---

<!--paginate: true-->

## Intro 

* As with the other types of related rates questions, one of the first steps is determining how the variables relate to each other.
* Since we're working with triangles for all of these questions, we have a variety of ways to define these relations.
* Some examples include:
    * Similar triangle ratios
    * Pythagorean Theorem
    * Trigonometric ratios and laws

---

## Example 1a

1. A $15\text{ft}$ ladder is leaning against a building. The base of the ladder begins sliding away from the wall at a rate of $2.5\text{ft/s}$. What rate is the ladder sliding down the wall when the top is $3\text{ft}$ from the floor?
    * $l^2 = x^2 + y^2$
    * $(15\text{ft})^2 = x^2 + y^2$
    * $225\text{ft}^2 = x^2 + y^2$
    * $\diff{t} (225\text{ft}^2) = \diff{t} (x^2 + y^2)$
    * $\diff{t} (225\text{ft}^2) = \diff{t} (x^2) + \diff{t} (y^2)$

---

## Example 1a, cont.

1. A $15\text{ft}$ ladder is leaning against a building. The base of the ladder begins sliding away from the wall at a rate of $2.5\text{ft/s}$. What rate is the ladder sliding down the wall when the top is $3\text{ft}$ from the floor?
    * $225\text{ft}^2 = x^2 + y^2$
    * $\diff{t} (225\text{ft}^2) = \diff{t} (x^2) + \diff{t} (y^2)$
    * $0 = \dot{x}2x + \dot{y}2y$
    * $225\text{ft}^2 - y^2 = x^2$
    * $x^2 = 225\text{ft}^2 - 9\text{ft}^2$
    * $x = \sqrt{225 - 9}\text{ft}$

---

## Example 1a, cont.

1. A $15\text{ft}$ ladder is leaning against a building. The base of the ladder begins sliding away from the wall at a rate of $2.5\text{ft/s}$. What rate is the ladder sliding down the wall when the top is $3\text{ft}$ from the floor?
    * $0 = \dot{x}2x + \dot{y}2y$
    * $x = \sqrt{225 - 9}\text{ft}$
    * $x = \sqrt{216}\text{ft}$
    * $x = 6\sqrt{6}\text{ft}$
    * $0 = 2(2.5\text{ft/s})(6\sqrt{6}\text{ft}) + 2(3\text{ft})\dot{y}$

---

## Example 1a, cont.

1. A $15\text{ft}$ ladder is leaning against a building. The base of the ladder begins sliding away from the wall at a rate of $2.5\text{ft/s}$. What rate is the ladder sliding down the wall when the top is $3\text{ft}$ from the floor?
    * $0 = 2(2.5\text{ft/s})(6\sqrt{6}\text{ft}) + 2(3\text{ft})\dot{y}$
    * $-30\sqrt{6} \text{ft}^2\text{/s} = (6\text{ft})\dot{y}$
    * $\dot{y} = -\frac{30\sqrt{6}\text{ft}^2\text{/s}}{6\text{ft}}$
    * $\dot{y} = -5\sqrt{6}\text{ft/s}$

---

## Example 1b

1. A $15\text{ft}$ ladder is leaning against a building. The base of the ladder begins sliding away from the wall at a rate of $2.5\text{ft/s}$. At what rate is the angle formed by the ladder and the floor decreasing when the base is $10\text{ft}$ from the wall (to 2 decimal places)?
    * $\cos \theta = \frac{x}{15\text{ft}}$
    * $\diff{t} (\cos \theta) = \diff{t} (\frac{x}{15\text{ft}})$
    * $(-\sin \theta)\dot{\theta} = \frac{1}{15\text{ft}}\dot{x}$
    * $\cos \theta = \frac{10\text{ft}}{15\text{ft}}$

---

## Example 1b, cont.

1. A $15\text{ft}$ ladder is leaning against a building. The base of the ladder begins sliding away from the wall at a rate of $2.5\text{ft/s}$. At what rate is the angle formed by the ladder and the floor decreasing when the base is $10\text{ft}$ from the wall (to 2 decimal places)?
    * $(-\sin \theta)\dot{\theta} = \frac{1}{15\text{ft}}\dot{x}$
    * $\cos \theta = \frac{10\text{ft}}{15\text{ft}}$
    * $\theta = \arccos(\frac{10}{15})$
    * $\theta = \arccos(\frac{2}{3})$

---

## Example 1b, cont.

1. A $15\text{ft}$ ladder is leaning against a building. The base of the ladder begins sliding away from the wall at a rate of $2.5\text{ft/s}$. At what rate is the angle formed by the ladder and the floor decreasing when the base is $10\text{ft}$ from the wall (to 2 decimal places)?
    * $(-\sin \theta)\dot{\theta} = \frac{1}{15\text{ft}}\dot{x}$
    * $\theta = \arccos(\frac{2}{3})$
    * $\theta = 0.841$
    * $(-\sin 0.841)\dot{\theta} = \frac{1}{15\text{ft}}(2.5\text{ft/s})$

---

## Example 1b, cont.

1. A $15\text{ft}$ ladder is leaning against a building. The base of the ladder begins sliding away from the wall at a rate of $2.5\text{ft/s}$. At what rate is the angle formed by the ladder and the floor decreasing when the base is $10\text{ft}$ from the wall (to 2 decimal places)?
    * $(-\sin 0.841)\dot{\theta} = \frac{1}{15\text{ft}}(2.5\text{ft/s})$
    * $\dot{\theta} = -\frac{2.5\text{ft/s}}{15\text{ft}(\sin 0.841)}$
    * $\dot{\theta} = -\frac{2.5}{11.179}\text{rad/s}$
    * $\dot{\theta} = -0.22\text{rad/s}$

---

## Example 1c

1. A $15\text{ft}$ ladder is leaning against a building. The base of the ladder begins sliding away from the wall at a rate of $2.5\text{ft/s}$. At what rate is the angle formed by the ladder and the floor decreasing when the base is $10\text{ft}$ from the wall (to 2 decimal places, no determining $\theta$)?
    * $(-\sin \theta)\dot{\theta} = \frac{1}{15\text{ft}}\dot{x}$
    * $(15\text{ft})^2 = (10\text{ft})^2 + y^2$
    * $(15)^2\text{ft}^2 - (10^2)\text{ft}^2 = y^2$
    * $y = \sqrt{15^2 - 10^2}\text{ft}$

---

## Example 1c, cont.

1. A $15\text{ft}$ ladder is leaning against a building. The base of the ladder begins sliding away from the wall at a rate of $2.5\text{ft/s}$. At what rate is the angle formed by the ladder and the floor decreasing when the base is $10\text{ft}$ from the wall (to 2 decimal places, no determining $\theta$)?
    * $(-\sin \theta)\dot{\theta} = \frac{1}{15\text{ft}}\dot{x}$
    * $\sin \theta = \frac{y}{15\text{ft}}$
    * $y = \sqrt{15^2 - 10^2}\text{ft}$
    * $y = \sqrt{125}\text{ft}$

---

## Example 1c, cont.

1. A $15\text{ft}$ ladder is leaning against a building. The base of the ladder begins sliding away from the wall at a rate of $2.5\text{ft/s}$. At what rate is the angle formed by the ladder and the floor decreasing when the base is $10\text{ft}$ from the wall (to 2 decimal places, no determining $\theta$)?
    * $(-\sin \theta)\dot{\theta} = \frac{1}{15\text{ft}}\dot{x}$
    * $\sin \theta = \frac{y}{15\text{ft}}$
    * $y = \sqrt{125}\text{ft}$
    * $y = 5\sqrt{5}\text{ft}$

---

## Example 1c, cont.

1. A $15\text{ft}$ ladder is leaning against a building. The base of the ladder begins sliding away from the wall at a rate of $2.5\text{ft/s}$. At what rate is the angle formed by the ladder and the floor decreasing when the base is $10\text{ft}$ from the wall (to 2 decimal places, no determining $\theta$)?
    * $(-\sin \theta)\dot{\theta} = \frac{1}{15\text{ft}}\dot{x}$
    * $\sin \theta = \frac{y}{15\text{ft}}$
    * $y = 5\sqrt{5}\text{ft}$
    * $\sin \theta = \frac{5\sqrt{5}\text{ft}}{15\text{ft}}$

---

## Example 1c, cont.

1. A $15\text{ft}$ ladder is leaning against a building. The base of the ladder begins sliding away from the wall at a rate of $2.5\text{ft/s}$. At what rate is the angle formed by the ladder and the floor decreasing when the base is $10\text{ft}$ from the wall (to 2 decimal places, no determining $\theta$)?
    * $(-\sin \theta)\dot{\theta} = \frac{1}{15\text{ft}}\dot{x}$
    * $\sin \theta = \frac{5\sqrt{5}\text{ft}}{15\text{ft}}$
    * $\sin \theta = \frac{\sqrt{5}}{3}$
    * $\dot{\theta} = -\frac{\dot{x}}{15\text{ft}(\sin \theta)}$

---

## Example 1c, cont.

1. A $15\text{ft}$ ladder is leaning against a building. The base of the ladder begins sliding away from the wall at a rate of $2.5\text{ft/s}$. At what rate is the angle formed by the ladder and the floor decreasing when the base is $10\text{ft}$ from the wall (to 2 decimal places, no determining $\theta$)?
    * $\sin \theta = \frac{\sqrt{5}}{3}$
    * $\dot{\theta} = -\frac{\dot{x}}{15\text{ft}(\sin \theta)}$
    * $\dot{\theta} = -\frac{2.5\text{ft/s}}{15\text{ft}(\frac{\sqrt{5}}{3})}$

---

## Example 1c, cont.

1. A $15\text{ft}$ ladder is leaning against a building. The base of the ladder begins sliding away from the wall at a rate of $2.5\text{ft/s}$. At what rate is the angle formed by the ladder and the floor decreasing when the base is $10\text{ft}$ from the wall (to 2 decimal places, no determining $\theta$)?
    * $\dot{\theta} = -\frac{2.5\text{ft/s}}{15\text{ft}(\frac{\sqrt{5}}{3})}$
    * $\dot{\theta} = -\frac{1}{2\sqrt{5}}\text{rad/s}$
    * $\dot{\theta} = -0.22 \text{rad/s}$

---

## Example 2

2. A streetlight is 6m tall. A person who is 2m tall is walking away from it at a rate of 1.5 m/s. How fast is the tip of the shadow cast moving away from the base?
    * $x$ is distance of the person, $y$ is the distance of the shadow.
    * $\frac{x}{4\text{m}} = \frac{y}{6\text{m}}$
    * $\diff{t} (\frac{x}{4\text{m}}) = \diff{t} (\frac{y}{6\text{m}})$
    * $\dot{x} (\frac{1}{4}\text{m}) = \dot{y} (\frac{1}{6}\text{m})$
    * $\dot{x} (\frac{6\text{m}}{4\text{m}}) = \dot{y}$

---

## Example 2, cont.

2. A streetlight is 6m tall. A person who is 2m tall is walking away from it at a rate of 1.5 m/s. How fast is the tip of the shadow cast moving away from the base?
    * $x$ is distance of the person, $y$ is the distance of the shadow.
    * $\dot{x} (\frac{6\text{m}}{4\text{m}}) = \dot{y}$
    * $\dot{y} = \frac{3}{2}\dot{x}$
    * $\dot{y} = \frac{3}{2}(1.5\text{m/s})$
    * $\dot{y} = 2.25\text{m/s}$

---

## Example 3

3. At 1pm, a van is 140km due north of a car. The van is travelling due west at 60km/hr and the car is heading north at 50km/hr. What rate is the distance between them changing at 3pm?
    * $\dot{x} = 60\text{km/hr}, \dot{y} = -50\text{km/hr}$
    * $x = 120\text{km}, y = 40\text{km}$
    * $x^2 + y^2 = z^2$
    * $z = \sqrt{x^2 + y^2}$
    * $z = \sqrt{(120\text{km})^2 + (40\text{km})^2}$

---

## Example 3, cont.

3. At 1pm, a van is 140km due north of a car. The van is travelling due west at 60km/hr and the car is heading north at 50km/hr. What rate is the distance between them changing at 3pm?
    * $\dot{x} = 60\text{km/hr}, \dot{y} = -50\text{km/hr}$
    * $x = 120\text{km}, y = 40\text{km}$
    * $x^2 + y^2 = z^2$
    * $z = \sqrt{(120\text{km})^2 + (40\text{km})^2}$
    * $z = \sqrt{1.6\times 10^4 \text{km}^2}$
    * $z = 40\sqrt{10} \text{km}$

---

## Example 3, cont.

3. At 1pm, a van is 140km due north of a car. The van is travelling due west at 60km/hr and the car is heading north at 50km/hr. What rate is the distance between them changing at 3pm?
    * $\dot{x} = 60\text{km/hr}, \dot{y} = -50\text{km/hr}$
    * $x = 120\text{km}, y = 40\text{km}, z = 40\sqrt{10} \text{km}$
    * $\diff{t} (x^2 + y^2) = \diff{t} (z^2)$
    * $\diff{t} (x^2) + \diff{t} (y^2) = \diff{t} (z^2)$
    * $2x(\dot{x}) + 2y(\dot{y}) = 2z(\dot{z})$

---

## Example 3, cont.

3. At 1pm, a van is 140km due north of a car. The van is travelling due west at 60km/hr and the car is heading north at 50km/hr. What rate is the distance between them changing at 3pm?
    * $\dot{x} = 60\text{km/hr}, \dot{y} = -50\text{km/hr}$
    * $x = 120\text{km}, y = 40\text{km}, z = 40\sqrt{10} \text{km}$
    * $2(120\text{km})(60\text{km/hr}) + 2(40\text{km})(-50\text{km/hr}) =$ 
    $2(40\sqrt{10}\text{km})(\dot{z})$
    * $\dot{z} = \frac{2(120\text{km})(60\text{km/hr}) + 2(40\text{km})(-50\text{km/hr})}{2(40\sqrt{10}\text{km})}$

---

## Example 3, cont.

3. At 1pm, a van is 140km due north of a car. The van is travelling due west at 60km/hr and the car is heading north at 50km/hr. What rate is the distance between them changing at 3pm?
    * $\dot{z} = \frac{2(120\text{km})(60\text{km/hr}) + 2(40\text{km})(-50\text{km/hr})}{2(40\sqrt{10}\text{km})}$
    * $\dot{z} = \frac{7200\text{km}^2\text{/hr} - 2000\text{km}^2\text{/hr}}{40\sqrt{10}\text{km}}$
    * $\dot{z} = \frac{5200\text{km}^2\text{/hr}}{40\sqrt{10}\text{km}}$
    * $\dot{z} = \frac{130}{\sqrt{10}}\text{km/hr}$

---

## Example 4

4. A triangle has 2 sides of length 15cm and 17cm. The angle between these is increasing at a rate of $\frac{\pi}{24}$ rad/s. At what rate is the length of the third side increasing when its opposite angle measures $\frac{\pi}{3}$ rads?
    * $\dot{\theta} = \frac{\pi}{24}\text{rad/s}$
    * $a^2 = b^2 + c^2 - 2bc \cos \theta$
    * $a^2 = (15\text{cm})^2 + (17\text{cm})^2 - 2(15\text{cm})(17\text{cm}) \cos \frac{\pi}{3}$
    * $a^2 = 225\text{cm}^2 + 289\text{cm}^2 - 510\text{cm}^2 (\frac{1}{2})$
    * $a^2 = 225\text{cm}^2 + 289\text{cm}^2 - 255\text{cm}^2$

---

## Example 4, cont.

4. A triangle has 2 sides of length 15cm and 17cm. The angle between these is increasing at a rate of $\frac{\pi}{24}$ rad/s. At what rate is the length of the third side increasing when its opposite angle measures $\frac{\pi}{3}$ rads?
    * $\dot{\theta} = \frac{\pi}{24}\text{rad/s}$
    * $a^2 = b^2 + c^2 - 2bc \cos \theta$
    * $a^2 = 225\text{cm}^2 + 289\text{cm}^2 - 255\text{cm}^2$
    * $\not\sqrt{a^{\not2}} = \sqrt{259\text{cm}^2}$
    * $a = \sqrt{259}\text{cm}$

---

## Example 4, cont.

4. A triangle has 2 sides of length 15cm and 17cm. The angle between these is increasing at a rate of $\frac{\pi}{24}$ rad/s. At what rate is the length of the third side increasing when its opposite angle measures $\frac{\pi}{3}$ rads?
    * $\dot{\theta} = \frac{\pi}{24}\text{rad/s}$
    * $a^2 = b^2 + c^2 - 2bc \cos \theta$
    * $a = \sqrt{259}\text{cm}$
    * $\diff{t} (a^2) = \diff{t} ((15\text{cm})^2 + (17\text{cm})^2 - 2(15\text{cm})(17\text{cm}) \cos \theta)$

---

## Example 4, cont.

4. A triangle has 2 sides of length 15cm and 17cm. The angle between these is increasing at a rate of $\frac{\pi}{24}$ rad/s. At what rate is the length of the third side increasing when its opposite angle measures $\frac{\pi}{3}$ rads?
    * $\dot{\theta} = \frac{\pi}{24}\text{rad/s}$
    * $a = \sqrt{259}\text{cm}$
    * $\diff{t} (a^2) = \diff{t} ((15\text{cm})^2 + (17\text{cm})^2 - 2(15\text{cm})(17\text{cm}) \cos \theta)$
    * $\diff{t} (a^2) = \diff{t} ((15\text{cm})^2) + \diff{t} ((17\text{cm})^2) -$ 
    $\diff{t} (2(15\text{cm})(17\text
    {cm}) \cos \theta)$

---

## Example 4, cont.

4. A triangle has 2 sides of length 15cm and 17cm. The angle between these is increasing at a rate of $\frac{\pi}{24}$ rad/s. At what rate is the length of the third side increasing when its opposite angle measures $\frac{\pi}{3}$ rads?
    * $\dot{\theta} = \frac{\pi}{24}\text{rad/s}$
    * $a = \sqrt{259}\text{cm}$
    * $\diff{t} (a^2) = \diff{t} ((15\text{cm})^2) + \diff{t} ((17\text{cm})^2) -$ 
    $\diff{t} (2(15\text{cm})(17\text
    {cm}) \cos \theta)$
    * $2a(\dot{a}) = \dot{\theta} (510\text{cm}^2 \sin \theta)$

---

## Example 4, cont.

4. A triangle has 2 sides of length 15cm and 17cm. The angle between these is increasing at a rate of $\frac{\pi}{24}$ rad/s. At what rate is the length of the third side increasing when its opposite angle measures $\frac{\pi}{3}$ rads?
    * $\dot{\theta} = \frac{\pi}{24}\text{rad/s}$
    * $a = \sqrt{259}\text{cm}$
    * $2a(\dot{a}) = \dot{\theta} (510\text{cm}^2 \sin \theta)$
    * $(2\sqrt{259}\text{cm})\dot{a} = (\frac{\pi}{24}\text{rad/s}) (510\text{cm}^2 \sin \frac{\pi}{3})$
    * $(2\sqrt{259}\text{cm})\dot{a} = (\frac{510\pi}{24}\text{rad}\text{ cm}^2\text{ s}^{-1} \frac{\sqrt{3}}{2})$

---

## Example 4, cont.

4. A triangle has 2 sides of length 15cm and 17cm. The angle between these is increasing at a rate of $\frac{\pi}{24}$ rad/s. At what rate is the length of the third side increasing when its opposite angle measures $\frac{\pi}{3}$ rads?
    * $(2\sqrt{259}\text{cm})\dot{a} = (\frac{510\pi}{24}\text{rad}\text{ cm}^2\text{ s}^{-1} \frac{\sqrt{3}}{2})$
    * $(2\sqrt{259}\text{cm})\dot{a} = (\frac{510\pi\sqrt{3}}{48}\text{rad}\text{ cm}^2\text{ s}^{-1})$
    * $\dot{a} = (\frac{85\pi\sqrt{3}}{8}\text{rad}\text{ cm}^2\text{ s}^{-1})/(2\sqrt{259}\text{cm})$
    * $\dot{a} = \frac{85\pi\sqrt{3}}{16\sqrt{259}}\text{cm/s}$
    * $\dot{a} \approx 1.8\text{cm/s}$

---

## Exercise for Readers

* A spotlight set on the ground is shining on a wall 20m away. A person 1.7m tall walks away from the light toward the wall at a rate of 1.4m/s. At what rate is the shadow cast on the wall decreasing in height when the person is 14m away from the light?
* The length of the hypotenuse of a right triangle is constant at 64cm. The vertical leg is decreasing at a rate of 5cm/s. At what rate is the angle opposite the vertical leg changing when the horizontal side is 40cm?

---

## Exercise for Readers, cont.

* Two sides of a triangle have a fixed lengths of 20cm and 24cm respectively. The third side is increasing at a rate of 3.5cm/s. When the third side is 15cm in length, what is the rate of change of the angle between the fixed sides?

---

# [Practice Quiz](Quiz)

Or

# [Next Lesson](Lesson%204)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercise

* A spotlight set on the ground is shining on a wall 20m away. A person 1.7m tall walks away from the light toward the wall at a rate of 1.4m/s. At what rate is the shadow cast on the wall decreasing in height when the person is 14m away from the light?
    * $\frac{1.7\text{m}}{x} = \frac{y}{20\text{m}}$
    * $\diff{t} (\frac{1.7\text{m}}{x}) = \diff{t} (\frac{1}{20\text{m}}y)$
    * $-\frac{1.7\text{m}(\dot{x})}{x^2} = \frac{1}{20\text{m}}\dot{y}$
    * $-\frac{1.7\text{m}(1.4\text{m/s})}{(14\text{m})^2} = \frac{1}{20\text{m}}\dot{y}$

---

## Answers to Exercise

* A spotlight set on the ground is shining on a wall 20m away. A person 1.7m tall walks away from the light toward the wall at a rate of 1.4m/s. At what rate is the shadow cast on the wall decreasing in height when the person is 14m away from the light?
    * $-\frac{1.7\text{m}(1.4\text{m/s})}{(14\text{m})^2} = \frac{1}{20\text{m}}\dot{y}$
    * $-\frac{2.38\text{m}^2\text{/s}}{196\text{m}^2} = \frac{1}{20\text{m}}\dot{y}$
    * $-\frac{47.6}{196} \text{m/s} = \dot{y}$
    * $\dot{y} = -0.24 \text{m/s}$

---

## Answers to Exercise, cont.

* The length of the hypotenuse of a right triangle is constant at 64cm. The vertical leg is decreasing at a rate of 5cm/s. At what rate is the angle opposite the vertical leg changing when the horizontal side is 40cm?
    * $\sin \theta = \frac{y}{64\text{cm}}$
    * $\cos \theta = \frac{40}{64}$
    * $\diff{t} (\sin \theta) = \diff{t} (\frac{1}{64\text{cm}}y)$
    * $\dot{\theta} (\cos \theta) = \frac{1}{64\text{cm}}\dot{y}$

---

## Answers to Exercise, cont.

* The length of the hypotenuse of a right triangle is constant at 64cm. The vertical leg is decreasing at a rate of 5cm/s. At what rate is the angle opposite the vertical leg changing when the horizontal side is 40cm?
    * $\cos \theta = \frac{40}{64}$
    * $\dot{\theta} (\cos \theta) = \frac{1}{64\text{cm}}\dot{y}$
    * $\frac{40}{64} \dot{\theta} = \frac{1}{64\text{cm}}(-5\text{cm/s})$
    * $40 \dot{\theta} = -5\text{rad/s}$

---

## Answers to Exercise, cont.

* The length of the hypotenuse of a right triangle is constant at 64cm. The vertical leg is decreasing at a rate of 5cm/s. At what rate is the angle opposite the vertical leg changing when the horizontal side is 40cm?
    * $40 \dot{\theta} = -5\text{rad/s}$
    * $\dot{\theta} = -\frac{5}{40}\text{rad/s}$
    * $\dot{\theta} = -\frac{1}{8}\text{rad/s}$

---

## Answers to Exercise, cont.

* Two sides of a triangle have a fixed lengths of 20cm and 24cm respectively. The third side is increasing at a rate of 3.5cm/s. When the third side is 15cm in length, what is the rate of change of the angle between the fixed sides?
    * $l^2 = a^2 + b^2 - 2ab \cos \theta$
    * $l^2 = (20\text{cm})^2 + (24\text{cm})^2 - 2(20\text{cm})(24\text{cm}) \cos \theta$
    * $\diff{t} (l^2) = \diff{t} [(20\text{cm})^2 + (24\text{cm})^2 - 960\text{cm}^2 \cos \theta]$
    * $\diff{t} (l^2) = \diff{t} ((20\text{cm})^2) + \diff{t} ((24\text{cm})^2) - \diff{t} (960\text{cm}^2 \cos \theta)$

---

## Answers to Exercise, cont.

* Two sides of a triangle have a fixed lengths of 20cm and 24cm respectively. The third side is increasing at a rate of 3.5cm/s. When the third side is 15cm in length, what is the rate of change of the angle between the fixed sides?
    * $\diff{t} (l^2) = \diff{t} ((20\text{cm})^2) + \diff{t} ((24\text{cm})^2) - \diff{t} (960\text{cm}^2 \cos \theta)$
    * $2l(\dot{l}) = 960\text{cm}^2 \sin \theta (\dot{\theta})$
    * $2(15\text{cm})(3.5\text{cm/s}) = 960\text{cm}^2 \sin \theta (\dot{\theta})$
    * $(15\text{cm})^2 = 400\text{cm}^2 + 576\text{cm}^2 - 960\text{cm}^2 \cos \theta$

---

## Answers to Exercise, cont.

* Two sides of a triangle have a fixed lengths of 20cm and 24cm respectively. The third side is increasing at a rate of 3.5cm/s. When the third side is 15cm in length, what is the rate of change of the angle between the fixed sides?
    * $2(15\text{cm})(3.5\text{cm/s}) = 960\text{cm}^2 \sin \theta (\dot{\theta})$
    * $(15\text{cm})^2 = 400\text{cm}^2 + 576\text{cm}^2 - 960\text{cm}^2 \cos \theta$
    * $225\text{cm}^2 = 976\text{cm}^2 - 960\text{cm}^2 \cos \theta$
    * $751\text{cm}^2 = 960\text{cm}^2 \cos \theta$

---

## Answers to Exercise, cont.

* Two sides of a triangle have a fixed lengths of 20cm and 24cm respectively. The third side is increasing at a rate of 3.5cm/s. When the third side is 15cm in length, what is the rate of change of the angle between the fixed sides?
    * $2(15\text{cm})(3.5\text{cm/s}) = 960\text{cm}^2 \sin \theta (\dot{\theta})$
    * $751\text{cm}^2 = 960\text{cm}^2 \cos \theta$
    * $\frac{751\text{cm}^2}{960\text{cm}^2} = \cos \theta$
    * $\theta = \arccos \frac{751}{960}$

---

## Answers to Exercise, cont.

* Two sides of a triangle have a fixed lengths of 20cm and 24cm respectively. The third side is increasing at a rate of 3.5cm/s. When the third side is 15cm in length, what is the rate of change of the angle between the fixed sides?
    * $2(15\text{cm})(3.5\text{cm/s}) = 960\text{cm}^2 \sin \theta (\dot{\theta})$
    * $\theta = \arccos \frac{751}{960}$
    * $\theta = 0.672$
    * $105\text{cm}^2\text{/s} = 960\text{cm}^2 \sin (0.672) (\dot{\theta})$

---

## Answers to Exercise, cont.

* Two sides of a triangle have a fixed lengths of 20cm and 24cm respectively. The third side is increasing at a rate of 3.5cm/s. When the third side is 15cm in length, what is the rate of change of the angle between the fixed sides?
    * $105\text{cm}^2\text{/s} = 960\text{cm}^2 \sin (0.672) (\dot{\theta})$
    * $\dot{\theta} = \frac{105\text{cm}^2\text{/s}}{960\text{cm}^2 \sin (0.672)}$
    * $\dot{\theta} = \frac{105}{960(0.623)}\text{rad/s}$
    * $\dot{\theta} = \frac{105}{598}\text{rad/s}$

---

## Answers to Exercise, cont.

* Two sides of a triangle have a fixed lengths of 20cm and 24cm respectively. The third side is increasing at a rate of 3.5cm/s. When the third side is 15cm in length, what is the rate of change of the angle between the fixed sides?
    * $\dot{\theta} = \frac{105}{598}\text{rad/s}$
    * $\dot{\theta} \approx 0.176\text{rad/s}$

---

# [Practice Quiz](Quiz)

Or

# [Next Lesson](Lesson%204)