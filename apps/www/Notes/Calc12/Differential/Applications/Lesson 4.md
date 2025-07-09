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

# Lesson 4: Applications in Economics

---

<!--paginate: true-->

## Intro 

* For any function $f(x)$, its derivative $f'(x)$ represents the rate of change of the function for any value in the domain.
* For Economics, we use multiple key functions to model costs, profit and revenue for a business.

---

## Introducing: The Cost Function

* Consider the function $C(x)$, where $C$ is the total cost for a business or company to produce $x$ items.
* Increasing the number of items produced has a corresponding increase in cost ($\Delta C$).
* We can then state that the average rate that the cost changes by defining $\frac{\Delta C}{\Delta x} = \frac{C(x + \Delta x) - C(x)}{\Delta x}$.
* *Hmm... This looks familiar.*
* From Elementary Derivatives Lesson 1: 
$\displaystyle \lim_{\Delta x \to 0}\frac{C(x + \Delta x) - f(x)}{\Delta x} = \dd[C]{x}$

---

## The Marginal Cost Function

* So, what happens when $\Delta x \to 0$? 
$\displaystyle \lim_{\Delta x \to 0}\frac{C(x + \Delta x) - f(x)}{\Delta x} = \dd[C]{x}$
* This case is known as *Marginal Cost*, or the rate at which cost is changing with respect to production.
* Hence, Marginal Cost is $\dd[C]{x}$.
* In other words, the Marginal Cost Function is the derivative of the cost function.
* Now, let's try this out, shall we?

---

## Example 1

1. The following is the cost function for the production of $x$ items: $C(x) = 5000 + 3x + 0.02x^2$.
    * Find the marginal cost function.
        * $\diff{x} C(x) = \diff{x} (5000 + 3x + 0.02x^2)$
        * $\diff{x} C(x) = \diff{x} (5000) + \diff{x} (3x) + \diff{x} (0.02x^2)$
        * $C'(x) = 3 + 0.04x$
    * Determine the marginal cost when there are 600 units produced.
        * $C'(600) = 3 + 0.04(600)$
        * $C'(600) = \$27 / \text{unit}$

---

## Example 2

2. The following is the cost function for the production of $x$ items: $C(x) = 8000 + 6x + 0.015x^2$. How many items are produced if the marginal cost is $21.78/unit?
    * $\diff{x} C(x) = \diff{x} (8000 + 6x + 0.015x^2)$
    * $\diff{x} C(x) = \diff{x} (8000) + \diff{x} (6x) + \diff{x} (0.015x^2)$
    * $C'(x) = 6 + 0.03x$
    * $21.78 = 6 + 0.03x$
    * $15.78 = 0.03x$
    * $x = 526\text{ units}$

---

## Introducing: The Price / Revenue Functions

* Some of the other important functions in economics include the *demand / price function*, $p(x)$ and the *revenue function*, $R(x) = xp(x)$.
* The derivative of the revenue function $R'(x)$ represent the rate of change of revenue with respect to the number of items sold ($x$).
* This function is known as the *Marginal Revenue* function.

---

## The Profit Function

* By definition: Profit = Revenue - Costs.
* Therefore, we can state that if $P(x) = R(x) - C(x)$, then $P'(x) = R'(x) - C'(x)$
* Using what we learned last unit, we know that $P(x)$ can have a maximum value when $P'(x) = 0$.
* It follows then that when $P'(x) = 0$, $0 = R'(x) - C'(x) \implies R'(x) = C'(x)$.
* Then, we can conclude that if we maximise profits, the marginal cost and marginal revenue are equal.

---

## Example 3

3. A company determines that its demand function for selling $x$ widgets is $p(x) = 10 - 0.02x$.
    * Determine the Revenue Function.
        * $R(x) = xp(x)$
        * $R(x) = x(10 - 0.02x)$
        * $R(x) = 10x - 0.02x^2$
    * Determine the Marginal Revenue Function.
        * $\diff{x} R(x) = \diff{x} (10x - 0.02x^2)$
        * $\diff{x} R(x) = \diff{x} (10x) - \diff{x} (0.02x^2)$
        * $R'(x) = 10 - 0.04x$

---

## Example 3, cont.

3. A company determines that its demand function for selling $x$ widgets is $p(x) = 10 - 0.02x$.
    * Determine marginal revenue when 1800 units are sold.
        * $R'(x) = 10 - 0.04x$
        * $R'(1800) = 10 - 0.04(1800)$
        * $R'(1800) = -\$62$

---

## Example 3, cont.

3. A company determines that its demand function for selling $x$ widgets is $p(x) = 10 - 0.02x$.
    * How many items must be sold to have a marginal revenue of -46?
        * $R'(x) = 10 - 0.04x$
        * $-46 = 10 - 0.04x$
        * $56 = 0.04x$
        * $x = \frac{5600}{4}$
        * $x = 1400$

---

## Example 4

4. A company produces $x$ batches of its products and has determined that its demand function is $p(x) = 5.5 - 0.012x$ and its cost function is $C(x) = 90 + 1.5x - 0.02x^2 + (3\times10^{-4})x^3$. Determine the number of batches required in order to maximize profit.
    * $R(x) = xp(x)$
    * $\diff{x} R(x) = \diff{x} [xp(x)]$
    * $\diff{x} R(x) = (x) [\diff{x} p(x)] + p(x) [\diff{x} x]$
    * $R'(x) = (x) [p'(x)] + p(x)$

---

## Example 4, cont.

4. A company produces $x$ batches of its products and has determined that its demand function is $p(x) = 5.5 - 0.012x$ and its cost function is $C(x) = 90 + 1.5x - 0.02x^2 + (3\times10^{-4})x^3$. Determine the number of batches required in order to maximize profit.
    * $R'(x) = (x) [p'(x)] + p(x)$
    * $R'(x) = -0.012x + 5.5 - 0.012x$
    * $R'(x) = 5.5 - 0.024x$

---

## Example 4, cont.

4. A company produces $x$ batches of its products and has determined that its demand function is $p(x) = 5.5 - 0.012x$ and its cost function is $C(x) = 90 + 1.5x - 0.02x^2 + (3\times10^{-4})x^3$. Determine the number of batches required in order to maximize profit.
    * $\diff{x} C(x) = \diff{x} (90 + 1.5x - 0.02x^2 + (3\times10^{-4})x^3)$
    * $\diff{x} C(x) = \diff{x} (90) + \diff{x} (1.5x) - \diff{x} (0.02x^2) +$
    $\diff{x} ((3\times10^{-4})x^3)$
    * $C'(x) = 1.5 - 0.04x + 9\times10^{-4}x^2$

---

## Example 4, cont.

4. A company produces $x$ batches of its products and has determined that its demand function is $p(x) = 5.5 - 0.012x$ and its cost function is $C(x) = 90 + 1.5x - 0.02x^2 + (3\times10^{-4})x^3$. Determine the number of batches required in order to maximize profit.
    * $R'(x) = 5.5 - 0.024x$
    * $C'(x) = 1.5 - 0.04x + 9\times10^{-4}x^2$
    * $5.5 - 0.024x = 1.5 - 0.04x + 9\times10^{-4}x^2$
    * $9\times10^{-4}x^2 - 0.016x - 4 = 0$

---

## Example 4, cont.

4. A company produces $x$ batches of its products and has determined that its demand function is $p(x) = 5.5 - 0.012x$ and its cost function is $C(x) = 90 + 1.5x - 0.02x^2 + (3\times10^{-4})x^3$. Determine the number of batches required in order to maximize profit.
    * $9\times10^{-4}x^2 - 0.016x - 4 = 0$
    * $x = \frac{-(-0.016) \pm \sqrt{(-0.016)^2 - 4(0.0009)(-4)}}{2(0.0009)}$
    * $x = \frac{0.016 \pm \sqrt{0.000256 + 0.014400}}{0.0018}$

---

## Example 4, cont.

4. A company produces $x$ batches of its products and has determined that its demand function is $p(x) = 5.5 - 0.012x$ and its cost function is $C(x) = 90 + 1.5x - 0.02x^2 + (3\times10^{-4})x^3$. Determine the number of batches required in order to maximize profit.
    * $x = \frac{0.016 \pm \sqrt{0.000256 + 0.014400}}{0.0018}$
    * $x = \frac{0.016 \pm \sqrt{0.014656}}{0.0018}$
    * $x = \frac{0.016 \pm 0.121}{0.0018}$

---

## Example 4, cont.

4. A company produces $x$ batches of its products and has determined that its demand function is $p(x) = 5.5 - 0.012x$ and its cost function is $C(x) = 90 + 1.5x - 0.02x^2 + (3\times10^{-4})x^3$. Determine the number of batches required in order to maximize profit.
    * $x = \frac{0.016 \pm 0.121}{0.0018}$
    * $x = \frac{0.016 + 0.121}{0.0018} = \frac{+}{+} = +$
    * $x = \frac{0.016 - 0.121}{0.0018} = \frac{-}{+} = -$ (E.R.)

---

## Example 4, cont.

4. A company produces $x$ batches of its products and has determined that its demand function is $p(x) = 5.5 - 0.012x$ and its cost function is $C(x) = 90 + 1.5x - 0.02x^2 + (3\times10^{-4})x^3$. Determine the number of batches required in order to maximize profit.
    * $x = \frac{0.016 + 0.121}{0.0018}$
    * $x = \frac{0.137}{0.0018}$
    * $x \approx 76 \text{ batches}$

---

## Exercise for Reader

* A cost function is represented as $C(x) = 3000 + 4.2x + 0.01x^2$
    * What is the marginal cost function?
    * Determine marginal cost at 1000 units.
    * How many units to give a marginal cost of $40?
* A demand function is $p(x) = 6 - 0.008x$.
    * What is the revenue function?
    * What is the marginal revenue function?
    * Determine marginal revenue when 650 items produced.

---

## Exercise for Reader, cont.

* A demand function is $p(x) = 6 - 0.008x$. The cost function is $C(x) = 55 + 1.9x - 0.009x^2 + 0.00008x^3$.
    * What is the profit function?
    * How many items needed to maximize profit?

---

# [Next Lesson](Lesson%205)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* A cost function is represented as $C(x) = 3000 + 4.2x + 0.01x^2$
    * What is the marginal cost function?
        * $\diff{x} C(x) = \diff{x} (3000 + 4.2x + 0.01x^2)$
        * $\diff{x} C(x) = \diff{x} (3000) + \diff{x} (4.2x) + \diff{x} (0.01x^2)$
        * $C'(x) = 4.2 + 0.02x$
    * Determine marginal cost at 1000 units.
        * $C'(1000) = 4.2 + 0.02(1000)$
        * $C'(1000) = 24.2$

---

## Answers to Exercises, cont.

* A cost function is represented as $C(x) = 3000 + 4.2x + 0.01x^2$
    * $C'(x) = 4.2 + 0.02x$
    * How many units to give a marginal cost of $40?
        * $40 = 4.2 + 0.02x$
        * $x = \frac{40 - 4.2}{0.02}$
        * $x = \frac{35.8}{0.02}$
        * $x = 1790\text{ units}$

---

## Answers to Exercises, cont.

* A demand function is $p(x) = 6 - 0.008x$.
    * What is the revenue function?
        * $R(x) = xp(x)$
        * $R(x) = x(6 - 0.008x)$
        * $R(x) = 6x - 0.008x^2$
    * What is the marginal revenue function?
        * $\diff{x} R(x) = \diff{x} (6x - 0.008x^2)$
        * $\diff{x} R(x) = \diff{x} (6x) - \diff{x} (0.008x^2)$
        * $R'(x) = 6 - 0.016x$

---

## Answers to Exercises, cont.

* A demand function is $p(x) = 6 - 0.008x$.
    * $R'(x) = 6 - 0.016x$
    * Determine marginal revenue when 650 items produced.
        * $R'(650) = 6 - 0.016(650)$
        * $R'(650) = 6 - 10.4$
        * $R'(650) = -4.4$

---

## Answers to Exercises, cont.

* A demand function is $p(x) = 6 - 0.008x$. The cost function is $C(x) = 55 + 1.9x - 0.009x^2 + 0.00008x^3$.
    * $R(x) = 6x - 0.008x^2$
    * What is the profit function?
        * $P(x) = R(x) - C(x)$
        * $P(x) = (6x - 0.008x^2) -$ 
        $(55 + 1.9x - 0.009x^2 + 0.00008x^3)$
        * $P(x) = -0.00008x^3 + 0.001x^2 + 4.1x - 55$
    * How many items needed to maximize profit?

---

## Answers to Exercises, cont.

* A demand function is $p(x) = 6 - 0.008x$. The cost function is $C(x) = 55 + 1.9x - 0.009x^2 + 0.00008x^3$.
    * $R'(x) = 6 - 0.016x$
    * How many items needed to maximize profit?
        * $\diff{x} C(x) = \diff{x} (55 + 1.9x - 0.009x^2 + 0.00008x^3)$
        * $\diff{x} C(x) = \diff{x} (55) + \diff{x} (1.9x) - \diff{x} (0.009x^2) +$ $\diff{x} (0.00008x^3)$
        * $C'(x) = 1.9 - 0.018x + 0.00024x^2$
        * $1.9 - 0.018x + 0.00024x^2 = 6 - 0.016x$
        * $0.00024x^2 - 0.002x - 4.1 = 0$

---

## Answers to Exercises, cont.

* A demand function is $p(x) = 6 - 0.008x$. The cost function is $C(x) = 55 + 1.9x - 0.009x^2 + 0.00008x^3$.
    * How many items needed to maximize profit?
        * $0.00024x^2 - 0.002x - 4.1 = 0$
        * $x = \frac{-(-0.002) \pm \sqrt{(-0.002)^2 - 4(0.00024)(-4.1)}}{2(0.00024)}$
        * $x = \frac{0.002 \pm \sqrt{0.000004 + 0.003936}}{0.00048}$
        * $x = \frac{0.002 \pm \sqrt{0.00394}}{0.00048}$
        * $x = \frac{0.002 \pm 0.0628}{0.00048}$
        * $x = \frac{0.002 + 0.0628}{0.00048}$

---

## Answers to Exercises, cont.

* A demand function is $p(x) = 6 - 0.008x$. The cost function is $C(x) = 55 + 1.9x - 0.009x^2 + 0.00008x^3$.
    * How many items needed to maximize profit?
        * $x = \frac{0.002 + 0.0628}{0.00048}$
        * $x = \frac{0.0648}{0.00048}$
        * $x = 135\text{ items}$

 ---

# [Next Lesson](Lesson%205)