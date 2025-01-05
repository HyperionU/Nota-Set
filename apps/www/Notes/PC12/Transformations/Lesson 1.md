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

# Lesson 1: Translations

---

## Vertical Translations

A *Vertical Translation* is basically sliding a graph up and down.

---

## Example: $x^2$

* Consider the function $f(x)=x^2$. It has this table of values:

| x | -2 | -1 | 0 | 1 | 2 |
|---|---|---|---|---|---|
| y | 4 | 1 | 0 | 1 | 4 |

* Desmos: Graph $f(x) = x^2$

---

## Example: Vertical Translation I

* Consider the function $y+3 = x^2$. How does its table and graph change?
* Well, we can rewrite it as $y = x^2-3$, and that gives us a hint.

| x | -2 | -1 | 0 | 1 | 2 |
|---|---|---|---|---|---|
| y | 1 | -2 | -3 | -2 | 1 |

* Congrats, we have transformed a graph!

---

## Vertical Translation II

* Consider the function $y-1 = x^2$. How does its table and graph change?
* We know that $y + n$ shifts a graph down, $\therefore y-n$ must shift it up.

| x | -2 | -1 | 0 | 1 | 2 |
|---|---|---|---|---|---|
| y | 5 | 2 | 1 | 2 | 5 |

* Congrats, you can shift a graph vertically.

---

# Review:

* A vertical translation shifts a graph up and down.
* How we write a vertical translation:

$y \mp k = f(x)$ or $y = f(x) \pm k$

---

## Horizontal Translations

A *Horizontal Translation* is basically sliding a graph left and right.

---

## Example: $|x|$

* Consider the function $f(x) = |x|$. It has this table of values:

| x | -2 | -1 | 0 | 1 | 2 |
|---|---|---|---|---|---|
| y | 2 | 1 | 0 | 1 | 2 |

* Desmos: Graph $f(x) = |x|$

---

## Example: Horizontal Translation I

* Consider the function $y = |x-2|$. How does its table and graph change?

| x | -2 | -1 | 0 | 1 | 2 |
|---|---|---|---|---|---|
| y | 4 | 3 | 2 | 1 | 0 |

* *Hmm...* It shifts it right 2.

---

## Example: Horizontal Translation II

* Consider the function $y = |x+1|$. How does its table and graph change?

| x | -2 | -1 | 0 | 1 | 2 |
|---|---|---|---|---|---|
| y | 1 | 0 | 1 | 2 | 3 |

* *Oh!* It's opposite if its next to the $x$.

---

# Review:

* A Horizontal Translation shifts a graph left and right.
* How we write a horizontal translation:
$y = f(x \mp h)$

---

## Translations:

* Now, we have a way to write any translation as a function.

$y - k = f(x - h)$ or $y = f(x - h) + k$

* Translations **DO NOT** change the shape of your graph, just the location of the points.

---

## Practice Question:

* Graph $y + 2 = f(x - 1)$
* For $f(x)$, pick any function.

---

## Image Points and Mapping Notation

* Image Points:
    * The new points created *after* a transformation.
* Mapping Notation:
    * A way to write out how tranformations map a function to its image.
    * $(x,y) \mapsto (x \mp h, y \pm k)$

---

## Example

What would the following functions look like if they were translated left 4 and up 6?

* $y = \frac{1}{x} \mapsto y - 6 = \frac{1}{x+4}$
* $y = \log{x} \mapsto y = \log{(x+4)}+6$
* $y = x^3-3x^2 \mapsto y - 6 = (x+4)^3 - 3(x+4)^2$
* $y = \frac{5}{x^2} \mapsto y = \frac{5}{(x+4)^2} + 6$

---

## Going Backwards

If $f(x) = |x|$, what is our function $g(x)$ if the vertex is translated 2 right and 3 up?

* Starting with $f(x)$, we can remember our transformation formula: $y - k = f(x - h)$ or $y = f(x - h) + k$
* Now, we know that $h = 2, k = 3$, so we just plug them in.
* $y = f(x - 2) + 3$, rewrite in terms of the function:
* $y = |x - 2| + 3$

---

# Note:
* You may think this is very easy (it is).
* But trust me, it gets harder from here.

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%202%20(Reflections).html) 

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">