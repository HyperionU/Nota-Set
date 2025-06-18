---
marp: true
theme: uncover
class: invert
math: mathjax
---

$\newcommand\odd{\mathbb{O}[f(x)]}$
$\newcommand\diff[1]{\mathcal{d}_{#1}}$

# <!--fit--> Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

$\newcommand\dd[2][]{\displaystyle\frac{d#1}{d#2}}$
$\newcommand\even{\mathbb{E}[f(x)]}$

<!--_footer: In partnership with Hyperion University, 2025-->

---

# Unit 5 Practice Quiz

---

<!--paginate: true-->

## Questions

1. Determine what symmetry, if any, $f(x) = \frac{4x^4 - 1}{x^2}$ has.
2. Determine intervals of Increase and Decrease, as well as any extrema values for the following:
    - $f(x) = x^2 - 4x + 1$
    - $y = \frac{x^2 + 1}{x}$
3. Determine concavity intervals and inflection points for the following:
    - $y = x^3 + 2x^2 - x + 4$
    - $f(x) = 2 \sin x$, $x \in (0, 2\pi)$

---

## Questions

4. Determine the dimensions of a can that can hold 355ml of soup, such that the cost required is minimised.

---

## Question 1 Answer

1. Determine what symmetry, if any, $f(x) = \frac{4x^4 - 1}{x^2}$ has.
    * $f(x) = \frac{4x^4}{x^2} - \frac{1}{x^2}$
    * $f(x) = 4x^2 - x^{-2}$
    * $f(-x) = 4(-x)^2 - (-x)^{-2}$
    * $f(-x) = 4x^2 - x^{-2}$
    * $-f(x) = -(4x^2 - x^{-2})$
    * $-f(x) = -4x^2 + x^{-2}$
    * $f(x) = f(-x) \therefore f(x) \in \even$
    * $f(-x) = -f(x) \therefore f(x) \notin \odd$

---

## Question 2a Answer

2. Determine intervals of Increase and Decrease, as well as any extrema values for $f(x) = x^2 - 4x + 1$
    * $\diff{x} f(x) = \diff{x} (x^2 - 4x + 1)$
    * $\diff{x} f(x) = \diff{x} (x^2) - \diff{x} (4x) + \diff{x} (1)$
    * $f'(x) = 2x - 4$
    * $2x - 4 = 0$
    * $x = 2$
    * $f'(0) = -$ (Dec.)
    * $f'(4) = +$ (Inc.)

---

## Question 2a Answer, cont.

2. Determine intervals of Increase and Decrease, as well as any extrema values for $f(x) = x^2 - 4x + 1$
    * Intervals:
        * Inc: $(2, \infty)$
        * Dec: $(-\infty, 2)$
    * Minimum: $(2, f(2))$
        * $f(2) = 2^2 - 4(2) + 1$
        * $f(2) = 4 - 8 + 1$
        * $f(2) = -3$
    * Minimum: $(2, -3)$

---

## Question 2b Answer

2. Determine intervals of Increase and Decrease, as well as any extrema values for $y = \frac{x^2 + 1}{x}$
    * $y = \frac{x^2}{x} + \frac{1}{x}$
    * $y = x + \frac{1}{x}$
    * $\diff{x} y = \diff{x} (x + \frac{1}{x})$
    * $\diff{x} y = \diff{x} (x) + \diff{x} (\frac{1}{x})$
    * $y' = 1 - \frac{1}{x^2}$
    

---

## Question 2b Answer, cont.

2. Determine intervals of Increase and Decrease, as well as any extrema values for $y = \frac{x^2 + 1}{x}$
    * $y' = 1 - \frac{1}{x^2}$
    * $1 - \frac{1}{x^2} = 0$
    * $\frac{1}{x^2} = 1$
    * $x^2 = 1$
    * $x = \pm 1$

---

## Question 2b Answer, cont.

2. Determine intervals of Increase and Decrease, as well as any extrema values for $y = \frac{x^2 + 1}{x}$
    * $y' = 1 - \frac{1}{x^2}$
    * $x = \pm 1$
    * $y'(-2) = +$
    * $y'(-\frac{1}{2}) = -$
    * $y'(\frac{1}{2}) = -$
    * $y'(2) = +$

---

## Question 2b Answer, cont.

2. Determine intervals of Increase and Decrease, as well as any extrema values for $y = \frac{x^2 + 1}{x}$
    * Intervals:
        * Inc: $(-\infty, -1) \cup (1, \infty)$
        * Dec: $(-1, 0) \cup (0, 1)$
    * Maximum: $(-1, -2)$
    * Minimum: $(1, 2)$

---

## Question 3a Answer

3. Determine concavity intervals and inflection points for $y = x^3 + 2x^2 - x + 4$
    * $\diff{x}^2 y = \diff{x}^2 (x^3 + 2x^2 - x + 4)$
    * $\diff{x} (\diff{x} y) = \diff{x} (\diff{x} (x^3) + \diff{x} (2x^2) - \diff{x} (x) + \diff{x} (4))$
    * $\diff{x} y' = \diff{x} (3x^2) + \diff{x} (4x) - \diff{x} 1$
    * $y'' = 6x + 4$
    * $6x + 4 = 0$
    * $x = -\frac{2}{3}$

---

## Question 3a Answer, cont.

3. Determine concavity intervals and inflection points for $y = x^3 + 2x^2 - x + 4$
    * $y'' = 6x + 4$
    * $x = -\frac{2}{3}$
    * $y''(-1) = -$ (Concave Down)
    * $y''(0) = +$ (Concave Up)
    * $y = (-\frac{2}{3})^3 + 2(-\frac{2}{3})^2 - (-\frac{2}{3}) + 4$
    * $y = -\frac{2^3}{3^3} + \frac{2^3}{3^2} + \frac{2}{3} + 4$
    * $y = -\frac{2^3 + 2^3(3) + 2(3^2) + 4(3^3)}{3^3}$

---

## Question 3a Answer, cont.

3. Determine concavity intervals and inflection points for $y = x^3 + 2x^2 - x + 4$
    * Concavity:
        * Up: $(-\frac{2}{3}, \infty)$
        * Down: $(-\infty, -\frac{2}{3})$
    * Inflection Point: $(-\frac{2}{3}, y)$
    * $y = -\frac{2^3 + 2^3(3) + 2(3^2) + 4(3^3)}{3^3}$
    * $y = -\frac{158}{27}$

---

## Question 3a Answer, cont.

3. Determine concavity intervals and inflection points for $y = x^3 + 2x^2 - x + 4$
    * Concavity:
        * Up: $(-\frac{2}{3}, \infty)$
        * Down: $(-\infty, -\frac{2}{3})$
    * Inflection Point: $(-\frac{2}{3}, -\frac{158}{27})$

---

## Question 3b Answer

3. Determine concavity intervals and inflection points for $f(x) = 2 \sin x$, $x \in (0, 2\pi)$
    * $\diff{x}^2 f(x) = \diff{x}^2 (2 \sin x)$
    * $\diff{x} (\diff{x} f(x)) = \diff{x} (\diff{x} (2 \sin x))$
    * $\diff{x} f'(x) = \diff{x} (2 \cos x)$
    * $f''(x) = -2 \sin x$
    * $-2 \sin x = 0$
    * $x = \pi$

---

## Question 3b Answer, cont.

3. Determine concavity intervals and inflection points for $f(x) = 2 \sin x$, $x \in (0, 2\pi)$
    * $f''(x) = -2 \sin x$
    * $x = \pi$
    * $f''(\frac{\pi}{2}) = -2 \sin \frac{\pi}{2}$
    * $f''(\frac{\pi}{2}) = -$ (Concave Down)
    * $f''(\frac{3\pi}{2}) = +$ (Concave Up)
    * $f(\pi) = 2 \sin \pi$
    * $f(\pi) = 0$

---

## Question 3b Answer, cont.

3. Determine concavity intervals and inflection points for $f(x) = 2 \sin x$, $x \in (0, 2\pi)$
    * Concavity
        * Up: $(\pi, 2\pi)$
        * Down: $(0, \pi)$
    * Inflection Point: $(\pi, 0)$

---

## Question 4 Answer

4. Determine the dimensions of a can that can hold 355ml of soup, such that the cost required is minimised.
    * $A(\rho, h) = 2\pi h\rho + 2\pi\rho^2$
    * $V = \pi\rho^2 h = 355\text{cm}^3$
    * $\pi\rho^2 h = 355$
    * $h = \frac{355}{\pi\rho^2}$
    * $A(\rho) = \frac{710}{\rho} + 2\pi\rho^2$
    * $\diff{\rho}A(\rho) = \diff{\rho}(\frac{710}{\rho} + 2\pi\rho^2)$
    * $\diff{\rho}A(\rho) = \diff{\rho}(\frac{710}{\rho}) + \diff{\rho} (2\pi\rho^2)$

---

## Question 4 Answer, cont.

4. Determine the dimensions of a can that can hold 355ml of soup, such that the cost required is minimised.
    * $A(\rho) = \frac{710}{\rho} + 2\pi\rho^2$
    * $\diff{\rho} A(\rho) = \diff{\rho} (\frac{710}{\rho}) + \diff{\rho} (2\pi\rho^2)$
    * $A'(\rho) = 4\pi\rho - \frac{710}{\rho^2}$
    * $4\pi\rho - \frac{710}{\rho^2} = 0$
    * $4\pi\rho = \frac{710}{\rho^2}$
    * $\rho^3 = \frac{355}{2\pi}$

---

## Question 4 Answer, cont.

4. Determine the dimensions of a can that can hold 355ml of soup, such that the cost required is minimised.
    * $A(\rho) = \frac{710}{\rho} + 2\pi\rho^2$
    * $A'(\rho) = 4\pi\rho - \frac{710}{\rho^2}$
    * $\rho^3 = \frac{355}{2\pi}$
    * $\rho = \sqrt[3]{\frac{355}{2\pi}} \approx 8.24$
    * $A'(1) = -$ (Dec.)
    * $A'(10) = +$ (Inc.)

---

## Question 4 Answer, cont.

4. Determine the dimensions of a can that can hold 355ml of soup, such that the cost required is minimised.
    * $\rho = \sqrt[3]{\frac{355}{2\pi}} \approx 8.24$
    * $h = \frac{355}{\pi(\frac{355}{2\pi})^{\frac{2}{3}}}$
    * $h = \frac{355}{\frac{\sqrt[3]{\pi}\sqrt[3]{355}^2}{\sqrt[3]{2^2}}}$
    * $h = \frac{355\sqrt[3]{2^2}}{\sqrt[3]{\pi}\sqrt[3]{355}^2}$
    * $h = \frac{\sqrt[3]{355}\sqrt[3]{2^2}}{\sqrt[3]{\pi}}$

---

## Question 4 Answer, cont.

4. Determine the dimensions of a can that can hold 355ml of soup, such that the cost required is minimised.
    * $\rho = \sqrt[3]{\frac{355}{2\pi}} \approx 8.24$
    * $h = \frac{\sqrt[3]{1420}}{\sqrt[3]{\pi}}$
    * $h = \sqrt[3]{\frac{1420}{\pi}} \approx 7.67$
    * dim: $\approx 8.24\text{cm}$ radius, $\approx 7.67\text{cm}$ height.
    * dim: $\sqrt[3]{\frac{355}{2\pi}}$ radius, $\sqrt[3]{\frac{1420}{\pi}}$ height.

---

# [Next Lesson](Lesson%206)