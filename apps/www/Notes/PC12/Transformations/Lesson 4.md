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

# Lesson 4: Composition of Transformations

---

## Prerequisites:

* Simple Transformations of Functions
* Factoring

---

## Composing Transformations

If we apply more than one transformation to a function:

$y = f(x) \mapsto \begin{cases} y = af(b
(x-h))+k \\ \text{or} \\ \frac{y-k}{a} = f(b(x-h)) \end{cases}$

The order is **important!**

* Mapping: $(x,y) \mapsto (\frac{x}{b} + h, ay + k)$

---

## Composing Transformations, cont

The order of transformations is as follows:
1. Stretches ($a$ and $b$)
2. Reflections
3. Translations ($h$ and $k$)

|   | $x$ | $y$ |
|---|-----|-----|
| S |$1/b$| $a$ |
| R |$f(-x)$|$-f(x)$|
| T |$-h$ | $k$ |

---

## Description of Transformations

Describe the Transformations on $y = f(x)$ and give the mapping notation.

* $y = 3f(x) + 2$  
    - $VS(3),\uparrow 2$, $(x,y) \mapsto (x,3y + 2)$ 
* $y - 4 = -f(x + 1)$
    - $VR,\uparrow 3, \leftarrow 1$, $(x,y) \mapsto (x - 1,-y + 4)$
* $y = \frac{1}{2}f(2x - 6)$ 
    - $y = \frac{1}{2}f(2(x - 3))$ 
    - $VS(\frac{1}{2}), HS(\frac{1}{2}), \rightarrow 3$, $(x,y) \mapsto (\frac{x}{2} + 3, \frac{y}{2})$

---

## Mapping Points

If the point $P(-6,12)$ is on the graph $y = f(x)$, what point must be on the graph of $y + 3 = -f(-(x + 2))$?

|   | $x$ | $y$ |
|---|-----|-----|
| S |  ø  |  ø  |
| R | $-$ | $-$ |
| T |$L2$ |$D3$ |

$(x,y) \mapsto (-x - 2, -y - 3)$, $P(-6,12) \mapsto P'(4, -15)$

---

## Going Backwards

Determine the equation for $y = g(x)$
* $g(x) := \{A'(-8,-10), B'(-7,2), C'(-6,-10)\}$
* $f(x) := \{A(2,6), B(4,2), C(6,6)\}$

$(x,y) \mapsto (\frac{x}{2} - 9, 2y - 2)$

$\therefore g(x) = 2f(2(x + 9)) - 2$

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%205%20(Inverses).html) 

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">
