---
marp: true
theme: uncover
class: invert
math: mathjax
---

$\newcommand\diff[1]{\mathcal{d}_{#1}}$
$\newcommand\limit[2]{\displaystyle\lim_{#1 \to #2}}$

# <!--fit--> Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2025-->

$\newcommand\dd[3][]{\displaystyle\frac{d^{#1}#2}{d#3^{#1}}}$

---

# Lesson 6: Vertical Asymptotes

---

<!--paginate: true-->

## Intro 

* An asymptote is a line that a function approaches, but never reaches.
* Vertical asymptotes *can* occur whenever a function is undefined.
* However, the existence of the asymptote must be confirmed by examining the behaviour of the function as it approaches the undefined value.
* For this, we can use our handed limits.

---

## Defining Vertical Asymptotes

* A function $y = f(x)$ has a vertical asymptote at $x = c$ if $f(c)$ is undefined and the following is true:
    * $\limit{x}{c^+} f(x) = \infty$
    * $\limit{x}{c^-} f(x) = \infty$
    * $\limit{x}{c^+} f(x) = -\infty$
    * $\limit{x}{c^-} f(x) = -\infty$

---

## Example 1

1. Find any vertical asymptotes of $y = \frac{3}{x - 2}$, and describe the function's behaviour near the asymptotes.
    * $x - 2 \ne 0$
    * $x \ne 2$ (This is our critical value.)
    * $\limit{x}{2^+} \frac{3}{x - 2}$
    * $\frac{3}{\epsilon} \to \infty$
    * $\limit{x}{2^-} \frac{3}{x - 2}$
    * $\frac{3}{-\epsilon} \to -\infty$

---

## Example 1, cont.

1. Find any vertical asymptotes of $y = \frac{3}{x - 2}$, and describe the function's behaviour near the asymptotes.
    * VA: $x = 2$
    * $\limit{x}{2^+} \frac{3}{x - 2} = \infty$
    * $\limit{x}{2^-} \frac{3}{x - 2} = -\infty$

* Determine the location of any vertical asymptotes of $f(x) = \frac{1}{x + 1}$, and describe the function's behaviour near the asymptotes. (Ex. for Reader)

---

## Example 2

2. Find any vertical asymptotes of $f(x) = \frac{4}{x^2 - x - 12}$, and describe the function's behaviour near the asymptotes.
    * $f(x) = \frac{4}{(x - 4)(x + 3)}$
    * $x - 4 \ne 0, x + 3 \ne 0$
    * $x \ne 4, -3$ (This is our critical values.)

---

## Example 2, cont.

2. Find any vertical asymptotes of $f(x) = \frac{4}{x^2 - x - 12}$, and describe the function's behaviour near the asymptotes.
    * $\limit{x}{-3^+} \frac{4}{x^2 - x - 12} = \frac{4}{-\epsilon} = -\infty$
    * $\limit{x}{-3^-} \frac{4}{x^2 - x - 12} = \frac{4}{\epsilon} = \infty$
    * $\limit{x}{4^+} \frac{4}{x^2 - x - 12} = \frac{4}{\epsilon} = \infty$
    * $\limit{x}{4^-} \frac{4}{x^2 - x - 12} = \frac{4}{-\epsilon} = \infty$

---

## Example 3

3. Find any vertical asymptotes of $f(x) = \frac{x + 2}{x^2 + 3x - 18}$, and describe the function's behaviour near the asymptotes.
    * $f(x) = \frac{x + 2}{(x + 6)(x - 3)}$
    * $x - 3 \ne 0, x + 6 \ne 0$
    * $x \ne 3, -6$ (This is our critical values.)

---

## Example 3, cont.

3. Find any vertical asymptotes of $f(x) = \frac{4}{x^2 - x - 12}$, and describe the function's behaviour near the asymptotes.
    * $\limit{x}{3^+} \frac{x + 2}{(x + 6)(x - 3)} = \frac{5}{\epsilon} = \infty$
    * $\limit{x}{3^-} \frac{x + 2}{(x + 6)(x - 3)} = \frac{5}{-\epsilon} = -\infty$
    * $\limit{x}{-6^+} \frac{x + 2}{(x + 6)(x - 3)} = \frac{4}{\epsilon} = \infty$
    * $\limit{x}{-6^-} \frac{x + 2}{(x + 6)(x - 3)} = \frac{-4}{\epsilon} = -\infty$

---

## Example 4

4. Find any vertical asymptotes of $y = \frac{x^2 - 9}{x - 3}$, and describe the function's behaviour near the asymptotes.
    * $y = \frac{(x - 3)(x + 3)}{x - 3}$
    * $y = x + 3$
    * No VA, but there is a removable discontinuity at $x = 3$.

* Determine the location of any vertical asymptotes of $f(x) = \frac{2}{x^2 + 2x - 3}$, and describe the function's behaviour near the asymptotes. (Ex. for Reader)

---

## Exercise for Readers

* Determine the location of any vertical asymptotes of $f(x) = \sec x, x \in (0, 2\pi)$, and describe the function's behaviour near the asymptotes.
* Determine the location of any vertical asymptotes of $f(x) = \frac{x + 5}{x - 4}$, and describe the function's behaviour near the asymptotes.

---

# [Next Lesson](Lesson%207)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Determine the location of any vertical asymptotes of $f(x) = \frac{1}{x + 1}$, and describe the function's behaviour near the asymptotes.
    * $x + 1 \ne 0$
    * $x \ne -1$
    * $\limit{x}{-1^+} \frac{1}{x + 1} = \frac{1}{\epsilon} = \infty$
    * $\limit{x}{-1^-} \frac{1}{x + 1} = \frac{1}{-\epsilon} = -\infty$

---

## Answers to Exercises, cont.

* Determine the location of any vertical asymptotes of $f(x) = \frac{2}{x^2 + 2x - 3}$, and describe the function's behaviour near the asymptotes.
    * $f(x) = \frac{2}{(x + 3)(x - 1)}$
    * $x + 3 \ne 0, x - 1 \ne 0$
    * $x \ne 1, -3$
    * $\limit{x}{-3^+} \frac{2}{(x + 3)(x - 1)} = \frac{2}{-\epsilon} = -\infty$
    * $\limit{x}{-3^-} \frac{2}{(x + 3)(x - 1)} = \frac{2}{\epsilon} = \infty$

---

## Answers to Exercises, cont.

* Determine the location of any vertical asymptotes of $f(x) = \frac{2}{x^2 + 2x - 3}$, and describe the function's behaviour near the asymptotes.
    * $f(x) = \frac{2}{(x + 3)(x - 1)}$
    * $\limit{x}{1^+} \frac{2}{(x + 3)(x - 1)} = \frac{2}{\epsilon} = \infty$
    * $\limit{x}{1^-} \frac{2}{(x + 3)(x - 1)} = \frac{2}{-\epsilon} = -\infty$

---

## Answers to Exercises, cont.

* Determine the location of any vertical asymptotes of $f(x) = \sec x, x \in (0, 2\pi)$, and describe the function's behaviour near the asymptotes.
    * $f(x) = \frac{1}{\cos x}$
    * $\cos x \ne 0$
    * $x \ne \frac{\pi}{2}, \frac{3\pi}{2}$
    * $\limit{x}{(\frac{\pi}{2})^+} \frac{1}{\cos x} = \frac{1}{-\epsilon} = -\infty$
    * $\limit{x}{(\frac{\pi}{2})^-} \frac{1}{\cos x} = \frac{1}{\epsilon} = \infty$

---

## Answers to Exercises, cont.

* Determine the location of any vertical asymptotes of $f(x) = \sec x, x \in (0, 2\pi)$, and describe the function's behaviour near the asymptotes.
    * $f(x) = \frac{1}{\cos x}$
    * $\limit{x}{(\frac{3\pi}{2})^+} \frac{1}{\cos x} = \frac{1}{\epsilon} = \infty$
    * $\limit{x}{(\frac{3\pi}{2})^-} \frac{1}{\cos x} = \frac{1}{-\epsilon} = -\infty$

---

## Answers to Exercises, cont.

* Determine the location of any vertical asymptotes of $f(x) = \frac{x + 5}{x - 4}$, and describe the function's behaviour near the asymptotes.
    * $x - 4 \ne 0$
    * $x \ne 4$
    * $\limit{x}{4^+} \frac{x + 5}{x - 4} = \frac{9}{\epsilon} = \infty$
    * $\limit{x}{4^-} \frac{x + 5}{x - 4} = \frac{9}{-\epsilon} = -\infty$

---

# [Next Lesson](Lesson%207)