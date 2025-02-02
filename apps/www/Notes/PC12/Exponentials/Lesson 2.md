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

# Lesson 2: Graphing Exponential Functions

---

## Graphing

![bg left invert](https://upload.wikimedia.org/wikipedia/commons/a/a0/2%5Ex_function_graph.PNG)

Sketch out the following:

$y = 2^x$
$y = 3^x$
$y = 1^x$
$y = (\frac{1}{2})^2$

---

## Generalizations

For $y = c^x$, where $c$ is a constant:

* if $c > 1$, $c^x$ grows. ($x \to \infty, y \to \infty$)
* if $0 < c < 1$, $c^x$ decays. ($x \to \infty, y \to 0$)
* if $c = 1$, $y = c$.
* As $c \to \infty$, the slope increases.
* There's technically one restriction: $c > 0$.
  * *You get a lot of 'artifacts' if you don't stay above 0. Try it, you'll see why.*

---

## Properties of $c^x$

* $y$-int is **always** 1.
* There (technically) is no $x$-intercept.
* Domain: $\{ x | x \in \mathbb{R} \}$
* Range: $\{ y | y > 0, y \in \mathbb{R} \}$
* Asymptote: $y = 0$.

---

## General Form of Exponentials

$$
  y = ac^{b(x - h)} + k
$$

* $a$: Vertical Stretch (reflects in $x$-axis)
* $b$: Horizontal Stretch (reflects in $y$-axis)
* $h$: Horizontal Shift $(x,y) \mapsto (x + h,y)$
* $k$: Vertical Shift $(x,y) \mapsto (x,y + k)$

Mapping Notation

$(x,y) \mapsto (bx + h, ay + k)$

---

## Graphing Tips

Sketch a graph of $y = 2(3)^{x - 4}$

* Note the transformations ($x + 4, 2y$).
* Note the basis graph ($3^x$).
* Mark the asymptote (dotted line and labelled).

Now, try sketching a graph of $y = -\frac{1}{2}(2)^{\frac{1}{5}x} - 5$.

* Note the transformations ($5x, -\frac{1}{2}y - 5$).
* Note the basis graph ($2^x$).
* Mark the asymptote ($y = -5$, dotted line and labelled).

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%203%20(Rational%20Functions).html)

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">