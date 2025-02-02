---
marp: true
theme: uncover
class: invert
math: mathjax
style: |
  .columns {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1rem;
  }
---

# <!--fit--> Pre-Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2024-->

---

<!--paginate: true-->

# Lesson 6: Applications

---

## Types of Applications

* An exponential function is in the form $f(x) = A \cdot c^x$, where $A$ is a constant and $c > 0$.
* There are two types we will consider.
* Type I: $c$ is a % (Compound Interest)
* Type II: Growth and Decay (Double, Triple and Half-life)

---

## Type I: Compound Interest

* $A = P(1 + r)^t$ compounded annually or % increase.
* $A = P(1 + \frac{r}{n})^{nt}$ compounded n times / year.
* $A = P(1 - r)^t$ % decrease.
* *Note: We're only focusing on the discrete case.*

---

## Type I Example (Interest)

<div class = "columns">
<span>
An investment of $500 is earning interest at 6% / annum (year) compounded semi-annually. How long until they double their investment ($1000)?
</span>

<span>

* $A = (1 + \frac{r}{n})^{nt}$
* $1000 = 500(1 + \frac{0.06}{2})^{2t}$
* $2 = (1 + 0.03)^{2t}$
* $\log 2 = 2t \log 1.03$
* $t = \frac{\log 2}{2 \log 1.03}$
* $t = 11.72$ yrs.

</span>
</div>

---

## Type I Example (Increase)

<div class = "columns">
<span>
The population increases at a rate of 7% / year. Currently, there are 1250 people. How long until there is 5000 people?
</span>

<span>

* $A = P(1 \pm r)^t$
* $5000 = 1250(1 + 0.07)^t$
* $4 = 1.07^t$
* $\log 4 = t \log 1.07$
* $t = \frac{\log 4}{\log 1.07}$
* $t = 20.49$ yrs.

</span>
</div>

---

## Type I Example (Decrease)

<div class = "columns">
<span>
An awful investment decreases at a rate of 4% / year. If the original investment was worth $450, how long until it is worth $320?
</span>

<span>

* $A = P(1 \pm r)^t$
* $320 = 450(1 - 0.04)^t$
* $\frac{32}{45} = 0.96^t$
* $\log(\frac{32}{45}) = t \log 0.96$
* $\log 32 - \log 45 = t \log 0.96$
* $t = \frac{\log 32 - \log 45}{\log 0.96}$
* $t = 8.35$ yrs.

</span>
</div>

---

## Type II: Growth / Decay

* Doubling: $A = P(2)^\frac{t}{R_D}$
* Tripling: $A = P(3)^\frac{t}{R_T}$
* Half-Life: $A = P(\frac{1}{2})^\frac{t}{H}$

---

## Type II Example (Doubling)

<div class = "columns">
<span>
The population of rabbits doubles every 3 months. If there are 12 rabbits now, how many months until there are 600 rabbits?
</span>

<span>

* $A = P(2)^\frac{t}{R_D}$
* $600 = 12(2)^\frac{m}{3}$
* $50 = 2^\frac{m}{3}$
* $\log 50 = \frac{m}{3} \log 2$
* $m = 3(\frac{\log 50}{\log 2})$
* $m = 3 \log_2(50)$
* $m = 3 (5.644)$
* $m = 16.93$ months

</span>
</div>

---

## Type II Example (Tripling)

<div class = "columns">
<span>
An insect colong triples every 20 weeks. If there are currently 1300 insects, how long until there are 6000 insects?
</span>

<span>

* $A = P(3)^\frac{t}{R_T}$
* $6000 = 1300(3)^\frac{w}{20}$
* $\frac{60}{13} = 3^\frac{w}{20}$
* $\log 60 - \log 13 = \frac{w}{20} \log 3$
* $w = 20(\frac{\log 60 - \log 13}{\log 3})$
* $w = 27.84$ weeks.

</span>
</div>

---

## Type II Example (Half-life)

<div class = "columns">
<span>
Lead-210 is a radioactive nuclide. If its half-life is 20 years, how long will it take 300g to decay to 200g?
</span>

<span>

* $A = P(\frac{1}{2})^\frac{t}{H}$
* $200 = 300(\frac{1}{2})^\frac{t}{20}$
* $\frac{2}{3} = (\frac{1}{2})^\frac{t}{20}$
* $\log 2 - \log 3 = \frac{t}{20} \log \frac{1}{2}$
* $w = 20(\frac{\log 2 - \log 3}{-\log 2})$
* $w = 11.70$ years.

</span>
</div>

---

## Type II Example (Rates)

A radioactive substance decays from 10g to 5.6g in 5 years. What is its half-life?

* $A = P(\frac{1}{2})^\frac{t}{H}$
* $5.6 = 10(\frac{1}{2})^\frac{5}{H}$
* $\frac{14}{25} = (\frac{1}{2})^\frac{5}{H}$
* $\log 14 - \log 25 = \frac{5}{H} \log \frac{1}{2}$
* $H = 5(\frac{- \log 2}{\log 14 - \log 25})$
* $H = 5.6$ years.

---

## Type I Example (Optics)

<div class = "columns">
<span>
The amount of visible light decreases by 5% / metre a diver descends below the surface. How many metres below is the diver when she sees 20% of the surface light? 
</span>

<span>

* $A = P(1 - r)^d$
* $20 = 100(1 - 0.05)^d$
* $\frac{1}{5} = (\frac{19}{20})^d$
* $- \log 5 = d(\log 19 - \log 20)$
* $d = \frac{-\log 5}{\log 19 - \log 20}$
* $d = 31.38\text{m}$

</span>
</div>

---

# [Next Unit <i class="fa-solid fa-diagram-next"></i>](../Operations/Lesson%201%20(Function%20Operations).html)

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">