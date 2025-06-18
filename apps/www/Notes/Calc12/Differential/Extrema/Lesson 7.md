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
$\newcommand\case[2]{#1 & \text{if} & #2}$

---

# Lesson 7: Horizontal Asymptotes

---

<!--paginate: true-->

## Intro 

* An asymptote is a line that a function approaches, but never reaches.
* We noticed that, when studying vertical asymptotes, the limits were as follows:
    * $x \to c, y \to \pm \infty$
* Now, if we invert these, what happens?
    * $x \to \pm \infty, y \to l$
* If this is the case, we can state that there is a *Horizontal* asymptote at $y = l$.

---

## Note: Crossing The Line

* Horizontal asymptotes are very similar to Vertical asymptotes.
* However, they behave quite differently.
* In fact, graphs of functions *can* cross the horizontal asymptote, but they don't have to.

---

## Example 1

1. Find the horizontal asymptotes for $f(x) = \frac{5}{x}$
    * $\limit{x}{\infty} \frac{5}{x}$
    * $\limit{x}{-\infty} \frac{5}{x}$
    * $\limit{x}{\infty} \frac{5}{x} = 0$
    * $\limit{x}{-\infty} \frac{5}{x} = 0$
    * HA: $y = 0$

---

## Handling Complexity

* For more complex rational functions, we'll need some more structure.
* First, some facts:
    * $\forall a \in \mathbb{Z} \wedge n \in \mathbb{Z}^+, \limit{x}{\pm \infty} \frac{a}{x^n} = 0$
    * Translation: for all integers $a$ and positive integers $n$, the limit as $x \to \pm \infty$ of $\frac{a}{x^n}$ is zero.
* This requires us to divide each term by the greatest power of $x$ in the denominator, split each term into separate limits, and evaluate seperately.

---

## Example 2

2. Find the horizontal asymptotes for $f(x) = \frac{2x^2 + x - 5}{7x^2 - 2x + 4}$
    * $\limit{x}{\infty} \frac{2x^2 + x - 5}{7x^2 - 2x + 4}$
    * $\limit{x}{\infty} \frac{\frac{2x^2 + x - 5}{x^2}}{\frac{7x^2 - 2x + 4}{x^2}}$
    * $\limit{x}{\infty} \frac{\frac{2x^2}{x^2} + \frac{x}{x^2} - \frac{5}{x^2}}{\frac{7x^2}{x^2} - \frac{2x}{x^2} + \frac{4}{x^2}}$

---

## Example 2, cont.

2. Find the horizontal asymptotes for $f(x) = \frac{2x^2 + x - 5}{7x^2 - 2x + 4}$
    * $\limit{x}{\infty} \frac{\frac{2x^2}{x^2} + \frac{x}{x^2} - \frac{5}{x^2}}{\frac{7x^2}{x^2} - \frac{2x}{x^2} + \frac{4}{x^2}}$
    * $\limit{x}{\infty} \frac{2 + \frac{1}{x} - \frac{5}{x^2}}{7 - \frac{2}{x} + \frac{4}{x^2}}$
    * $\frac{\limit{x}{\infty} (2 + \frac{1}{x} - \frac{5}{x^2})}{\limit{x}{\infty} (7 - \frac{2}{x} + \frac{4}{x^2})}$

---

## Example 2, cont.

2. Find the horizontal asymptotes for $f(x) = \frac{2x^2 + x - 5}{7x^2 - 2x + 4}$
    * $\frac{\limit{x}{\infty} (2 + \frac{1}{x} - \frac{5}{x^2})}{\limit{x}{\infty} (7 - \frac{2}{x} + \frac{4}{x^2})}$
    * $\frac{2 + \limit{x}{\infty} \frac{1}{x} - \limit{x}{\infty}\frac{5}{x^2}}{7 - \limit{x}{\infty} \frac{2}{x} + \limit{x}{\infty} \frac{4}{x^2}}$

---

## Example 2, cont.

2. Find the horizontal asymptotes for $f(x) = \frac{2x^2 + x - 5}{7x^2 - 2x + 4}$
    * $\frac{2 + \limit{x}{\infty} \frac{1}{x} - \limit{x}{\infty}\frac{5}{x^2}}{7 - \limit{x}{\infty} \frac{2}{x} + \limit{x}{\infty} \frac{4}{x^2}}$
    * $\frac{2}{7}$
    * HA: $y = \frac{2}{7}$

---

## Example 3

3. Find the horizontal asymptotes for $f(x) = \frac{5x^2 - 2x + 1}{3x + 1}$
    * $\limit{x}{\infty} \frac{5x^2 - 2x + 1}{3x + 1}$
    * $\limit{x}{\infty} \frac{\frac{5x^2}{x^2} - \frac{2x}{x^2} + \frac{1}{x^2}}{\frac{3x}{x^2} + \frac{1}{x^2}}$
    * $\limit{x}{\infty} \frac{5 - \frac{2}{x} + \frac{1}{x^2}}{\frac{3}{x} + \frac{1}{x^2}}$
    * $\frac{5}{0} \therefore$ No HA.

---

## Determining Asymptotes

$$
A_H = \limit{x}{\infty} \frac{N}{D} = 
\begin{cases}
    \case{0}{\deg N > \deg D} \\
    \case{\emptyset}{\deg N < \deg D} \\
    \case{\frac{a_N}{a_D}}{\deg N = \deg D}
\end{cases}
$$
Where $\deg f(x)$ is the greatest power of $x$, and $a$ is the $\deg f(x)$ term's coefficient.

---

## Example 4

4. Find the horizontal asymptotes for $f(x) = \frac{-3x^3 - 2x^2 + 1}{6x^3 - x^2 + 6}$
    * $\limit{x}{\infty} \frac{-3x^3 - 2x^2 + 1}{6x^3 - x^2 + 6}$
    * $\limit{x}{\infty} \frac{\frac{-3x^3}{x^3} - \frac{2x^2}{x^3} + \frac{1}{x^3}}{\frac{6x^3}{x^3} - \frac{x^2}{x^3} + \frac{6}{x^3}}$
    * $\limit{x}{\infty} \frac{-3 - \frac{2}{x} + \frac{1}{x^3}}{6 - \frac{1}{x} + \frac{6}{x^3}}$
    * $\frac{-3}{6}$
    * HA: $y = -\frac{1}{2}$

---

## Example 5

5. Find the horizontal and vertical asymptotes for $f(x) = \frac{x^2 + x - 7}{3x^2 - 3}$
    * Vertical
        * $f(x) = \frac{x^2 + x - 7}{3(x^2 - 1)}$
        * $f(x) = \frac{x^2 + x - 7}{3(x - 1)(x + 1)}$
        * $x \pm 1 \ne 0$
        * $x \ne \pm 1$

---

## Example 5

5. Find the horizontal and vertical asymptotes for $f(x) = \frac{x^2 + x - 7}{3x^2 - 3}$
    * Vertical
        * $x = 1$
        * $\limit{x}{1^+} \frac{x^2 + x - 7}{3(x - 1)(x + 1)} =  \frac{-5}{\epsilon} = -\infty$
        * $\limit{x}{1^-} \frac{x^2 + x - 7}{3(x - 1)(x + 1)} = \frac{5}{\epsilon} = \infty$

---

## Example 5, cont.

5. Find the horizontal and vertical asymptotes for $f(x) = \frac{x^2 + x - 7}{3x^2 - 3}$
    * Vertical
        * $x = -1$
        * $\limit{x}{-1^+} \frac{x^2 + x - 7}{3(x - 1)(x + 1)} = \frac{7}{\epsilon} = \infty$
        * $\limit{x}{-1^-} \frac{x^2 + x - 7}{3(x - 1)(x + 1)} = \frac{-7}{\epsilon} = -\infty$

---

## Example 5, cont.

5. Find the horizontal and vertical asymptotes for $f(x) = \frac{x^2 + x - 7}{3x^2 - 3}$
    * Horizontal
        * $\limit{x}{\infty} \frac{x^2 + x - 7}{3x^2 - 3}$
        * $\limit{x}{\infty} \frac{\frac{x^2}{x^2} + \frac{x}{x^2} - \frac{7}{x^2}}{\frac{3x^2}{x^2} - \frac{3}{x^2}}$
        * $\limit{x}{\infty} \frac{1 + \frac{1}{x} - \frac{7}{x^2}}{3 - \frac{3}{x^2}}$
        
---

## Example 5, cont.

5. Find the horizontal and vertical asymptotes for $f(x) = \frac{x^2 + x - 7}{3x^2 - 3}$
    * Horizontal
        * $\limit{x}{\infty} \frac{1 + \frac{1}{x} - \frac{7}{x^2}}{3 - \frac{3}{x^2}}$
        * $\frac{\limit{x}{\infty} 1 + \limit{x}{\infty} \frac{1}{x} - \limit{x}{\infty} \frac{7}{x^2}}{\limit{x}{\infty} 3 - \limit{x}{\infty} \frac{3}{x^2}}$

---

## Example 5, cont.

5. Find the horizontal and vertical asymptotes for $f(x) = \frac{x^2 + x - 7}{3x^2 - 3}$
    * Horizontal
        * $\frac{\limit{x}{\infty} 1 + \limit{x}{\infty} \frac{1}{x} - \limit{x}{\infty} \frac{7}{x^2}}{\limit{x}{\infty} 3 - \limit{x}{\infty} \frac{3}{x^2}}$
        * HA: $y = \frac{1}{3}$

---

## Exercise for Readers

* Determine the horizontal asymptotes of 
    * $f(x) = \frac{x^2}{x^3 - 4}$
    * $f(x) = \frac{2x^2 - x}{4x^2 - 3}$
    * $f(x) = \frac{-5x^3 - 4x^2}{3x^2 + x}$
    * $f(x) = \frac{-4x^3 + 2x^2 - 1}{6x^3 - x + 5}$
* Determine the horizontal and vertical asymptotes of 
    * $f(x) = \frac{2x + 1}{x - 3}$
    * $f(x) = \frac{-4x^2 - x}{x^2 - 2x - 15}$

---

# [Next Lesson](Lesson%208)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Determine the horizontal asymptotes of  $f(x) = \frac{x^2}{x^3 - 4}$
    * $\limit{x}{\infty} \frac{x^2}{x^3 - 4}$
    * $\limit{x}{\infty} \frac{\frac{x^2}{x^3}}{\frac{x^3}{x^3} - \frac{4}{x^3}}$
    * $\limit{x}{\infty} \frac{\frac{1}{x}}{1 - \frac{4}{x^3}}$
    * HA: $y = 0$

---

## Answers to Exercises, cont.

* Determine the horizontal asymptotes of  $f(x) = \frac{2x^2 - x}{4x^2 - 3}$
    * $\limit{x}{\infty} \frac{2x^2 - x}{4x^2 - 3}$
    * $\limit{x}{\infty} \frac{\frac{2x^2}{x^2} - \frac{x}{x^2}}{\frac{4x^2}{x^2} - \frac{3}{x^2}}$
    * $\limit{x}{\infty} \frac{2 - \frac{1}{x}}{4 - \frac{3}{x^2}}$
    * HA: $y = \frac{2}{4}$

---

## Answers to Exercises, cont.

* Determine the horizontal asymptotes of  $f(x) = \frac{-5x^3 - 4x^2}{3x^2 + x}$
    * $\limit{x}{\infty} -\frac{5x^3 + 4x^2}{3x^2 + x}$
    * $\limit{x}{\infty} -\frac{\frac{5x^3}{x^3} + \frac{4x^2}{x^3}}{\frac{3x^2}{x^3} + \frac{x}{x^3}}$
    * $\limit{x}{\infty} -\frac{5 + \frac{4}{x}}{\frac{3}{x} + \frac{1}{x^2}}$

---

## Answers to Exercises, cont.

* Determine the horizontal asymptotes of  $f(x) = \frac{-5x^3 - 4x^2}{3x^2 + x}$
    * $\limit{x}{\infty} -\frac{5 + \frac{4}{x}}{\frac{3}{x} + \frac{1}{x^2}}$
    * $y = -\frac{5}{0} \therefore$ No HA.

---

## Answers to Exercises, cont.

* Determine the horizontal asymptotes of  $f(x) = \frac{-4x^3 + 2x^2 - 1}{6x^3 - x + 5}$
    * $\limit{x}{\infty} -\frac{4x^3 - 2x^2 + 1}{6x^3 - x + 5}$
    * $\limit{x}{\infty} -\frac{\frac{4x^3}{x^3} - \frac{2x^2}{x^3} + \frac{1}{x^3}}{\frac{6x^3}{x^3} - \frac{x}{x^3} + \frac{5}{x^3}}$
    * $\limit{x}{\infty} -\frac{4 - \frac{2}{x} + \frac{1}{x^3}}{6 - \frac{1}{x^2} + \frac{5}{x^3}}$

---

## Answers to Exercises, cont.

* Determine the horizontal asymptotes of  $f(x) = \frac{-4x^3 + 2x^2 - 1}{6x^3 - x + 5}$
    * $\limit{x}{\infty} -\frac{4 - \frac{2}{x} + \frac{1}{x^3}}{6 - \frac{1}{x^2} + \frac{5}{x^3}}$
    * HA: $y = -\frac{4}{6}$

---

## Answers to Exercises, cont.

* Determine the horizontal and vertical asymptotes of $f(x) = \frac{2x + 1}{x - 3}$
    * Horizontal:
        * $\limit{x}{\infty} \frac{2x + 1}{x - 3}$
        * $\limit{x}{\infty} \frac{\frac{2x}{x} + \frac{1}{x}}{\frac{x}{x} - \frac{3}{x}}$
        * $\limit{x}{\infty} \frac{2 + \frac{1}{x}}{1 - \frac{3}{x}}$

---

## Answers to Exercises, cont.

* Determine the horizontal and vertical asymptotes of $f(x) = \frac{2x + 1}{x - 3}$
    * Horizontal:
        * $\limit{x}{\infty} \frac{2 + \frac{1}{x}}{1 - \frac{3}{x}}$
        * HA: $y = 2$

---

## Answers to Exercises, cont.

* Determine the horizontal and vertical asymptotes of $f(x) = \frac{2x + 1}{x - 3}$
    * Vertical: 
        * CV: $x = 3$
        * $\limit{x}{3^+} \frac{2x + 1}{x - 3} = \frac{7}{\epsilon} = \infty$
        * $\limit{x}{3^-} \frac{2x + 1}{x - 3} = \frac{7}{-\epsilon} = -\infty$

---

## Answers to Exercises, cont.

* Determine the horizontal and vertical asymptotes of $f(x) = \frac{-4x^2 - x}{x^2 - 2x - 15}$
    * Horizontal:
        * $\limit{x}{\infty} -\frac{4x^2 + x}{x^2 - 2x - 15}$
        * $\limit{x}{\infty} -\frac{\frac{4x^2}{x^2} + \frac{x}{x^2}}{\frac{x^2}{x^2} - \frac{2x}{x^2} - \frac{15}{x^2}}$
        * $\limit{x}{\infty} -\frac{4 + \frac{1}{x}}{1 - \frac{2}{x} - \frac{15}{x^2}}$

---

## Answers to Exercises, cont.

* Determine the horizontal and vertical asymptotes of $f(x) = \frac{-4x^2 - x}{x^2 - 2x - 15}$
    * Horizontal:
        * $\limit{x}{\infty} -\frac{4 + \frac{1}{x}}{1 - \frac{2}{x} - \frac{15}{x^2}}$
        * HA: $y = -4$

---

## Answers to Exercises, cont.

* Determine the horizontal and vertical asymptotes of $f(x) = \frac{-4x^2 - x}{x^2 - 2x - 15}$
    * Vertical:
        * $f(x) = -\frac{4x^2 + x}{(x + 3)(x - 5)}$
        * CV: $x = 5, -3$

---

## Answers to Exercises, cont.

* Determine the horizontal and vertical asymptotes of $f(x) = \frac{-4x^2 - x}{x^2 - 2x - 15}$
    * Vertical:
        * CV: $x = -3$
        * $\limit{x}{-3^+} -\frac{4x^2 + x}{(x + 3)(x - 5)} = \frac{33}{\epsilon} = \infty$
        * $\limit{x}{-3^-} -\frac{4x^2 + x}{(x + 3)(x - 5)} = -\frac{33}{\epsilon} = -\infty$

---

## Answers to Exercises, cont.

* Determine the horizontal and vertical asymptotes of $f(x) = \frac{-4x^2 - x}{x^2 - 2x - 15}$
    * Vertical:
        * CV: $x = 5$
        * $\limit{x}{5^+} -\frac{4x^2 + x}{(x + 3)(x - 5)} = -\frac{95}{\epsilon} = -\infty$
        * $\limit{x}{5^-} -\frac{4x^2 + x}{(x + 3)(x - 5)} = \frac{95}{\epsilon} = \infty$

---

# [Next Lesson](Lesson%208)