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

<!--paginate: true-->

# Lesson 7: Change of Domain

---

## Change of Domain

Sometimes, you'll be asked to find solutions in different domains.
Previously you only needed to find solutions in $[0, 2\pi)$, but in reality, the domain could be any amount of revolutions or part of $\mathbb{c}$ you'd want.

---

## Symmetric Domains

Solve $\sin x = - \frac{1}{2}, -\pi \leq x < \pi$

1. Split the domain
$-\pi \leq x \leq 0, 0 \leq x < \pi$
2. Consider each domain
$0 \leq x < \pi$ has no solutions, but $-\pi \leq x \leq 0$ does.
3. Find $x_r$
$\sin^{-1}(\frac{1}{2}) = \frac{\pi}{6} = x_r$
4. Solve for x.
$x = -\frac{6\pi}{6} + x_r, -\frac{\pi}{6}$, $x = -\frac{5\pi}{6}, -\frac{\pi}{6}$

---

## Asymmetric Domains

Solve $\tan x = 0, -\frac{\pi}{2} \leq x \leq \pi$

1. Find $x$.
$x = 0, \pi$.
2. Verify if $x \in \mathfrak{D}$

$x = 0, \pi$.

---

## Quadratic Trig Domains

Solve $3 \cos^2 x - \cos x - 2 = 0$ for these domains:

* $0 \leq x < 2\pi$
* $-\pi \leq x < \pi$

1. Factor to make this easier

$(3\cos x + 2)(\cos x - 1)$
$\cos x = 1, -\frac{2}{3}$

---

## Quadratic Domains, cont.

* $0 \leq x < 2\pi$
    * $\cos x = 1$: $x = 0$
    * $\cos x = -\frac{2}{3}$: $x_r = 0.8411, x_2 = 2.30, x_3 = 3.98$   
    * $x = 0, 2.30, 3.98$
* $-\pi \leq x < \pi$
    * $\cos x = 1$: $x = 0$
    * $\cos x = -\frac{2}{3}$: $x_r = 0.8411, x_2 = 2.30, x_3 = -2.30$   
    * $x = 0, \pm 2.30$

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%208%20(General%20Solutions).html)

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">
