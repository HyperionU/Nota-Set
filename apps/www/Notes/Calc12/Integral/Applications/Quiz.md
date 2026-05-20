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

<!--_footer: In partnership with Hyperion University, 2026-->

---

# Unit 8 Practice Quiz

---

<!--paginate: true-->

## Questions

1. Evaluate $\int_0^\pi (x + \cos x) dx$.
2. Solve $\int 2 \tan x dx$ using substitution.
3. Solve $\int \frac{(x^2 - 1)}{(x^2 - 1)^2(x - 1)}dx$ using partial fractions.
4. Solve $\int 2x \cos x dx$ using integration by parts.
5. Evaluate $\int_1^2 \frac{e^x}{1 - e^x} dx$
6. Determine $\int (4 - x^2) dx - \int (x - x^2) dx$

---

## Question 1 Answer

1. Evaluate $\int_0^\pi (x + \cos x) dx$
    * $[\frac{x^2}{2} + \sin x]_0^\pi$
    * $[\frac{\pi^2}{2} + \sin \pi] - [\frac{0^2}{2} + \sin 0]$
    * $\frac{\pi^2}{2}$

---

## Question 2 Answer

2. Solve $\int 2 \tan x dx$ using substitution.
    * $u = \tan x \implies du = \sec^2 x dx$
    * $\frac{2}{\sec^2 x} \int u du$
    * $\frac{2}{\sec^2 x} \frac{u^2}{2} + C$
    * $\cos^2 x \frac{\sin^2 x}{\cos^2 x} + C$
    * $\sin^2 x + C$

---

## Question 3 Answer

3. Solve $\int \frac{(x^2 - 1)}{(x^2 - 1)^2(x - 1)}dx$ using partial fractions.
    * $\int \frac{1}{(x^2 - 1)(x - 1)}dx$
    * $\int \frac{1}{(x + 1)(x - 1)^2} dx$
    * $\frac{1}{(x + 1)(x - 1)^2} = \frac{A}{x + 1} + \frac{B}{x - 1} + \frac{C}{(x - 1)^2}$
    * $1 = A(x - 1)^2 + B(x^2 - 1) + C(x + 1)$
    * $1 = Ax^2 - 2Ax + A + Bx^2 - B + Cx + C$
    * $1 = (A + B)x^2 + (-2A + C)x + (A - B + C)$

---

## Question 3 Answer, cont.

3. Solve $\int \frac{(x^2 - 1)}{(x^2 - 1)^2(x - 1)}dx$ using partial fractions.
    * $\int \frac{1}{(x + 1)(x - 1)^2} dx$
    * $1 = (A + B)x^2 + (-2A + C)x + (A - B + C)$
    * $\begin{cases}A + B & = 0 \\ -2A + C & = 0 \\ A - B + C & = 1\end{cases}$
    * $\begin{cases}A & = -B \\ C & = 2A \\ 4B & = -1\end{cases}$

---

## Question 3 Answer, cont.

3. Solve $\int \frac{(x^2 - 1)}{(x^2 - 1)^2(x - 1)}dx$ using partial fractions.
    * $\int \frac{1}{(x + 1)(x - 1)^2} dx$
    * $\begin{cases}A & = -B \\ C & = 2A \\ 4B & = -1\end{cases}$
    * $\begin{cases}A & = \frac{1}{4} \\ C & = \frac{1}{2} \\ B & = -\frac{1}{4}\end{cases}$

---

## Question 3 Answer, cont.

3. Solve $\int \frac{(x^2 - 1)}{(x^2 - 1)^2(x - 1)}dx$ using partial fractions.
    * $\begin{cases}A & = \frac{1}{4} \\ C & = \frac{1}{2} \\ B & = -\frac{1}{4}\end{cases}$
    * $\frac{1}{4}\int \frac{1}{x + 1} dx - \int \frac{1}{4}\frac{1}{x - 1} dx + \frac{1}{2} \int \frac{1}{(x - 1)^2} dx$
    * $\frac{1}{4}\ln |x + 1| - \frac{1}{4} \ln |x - 1| + \frac{1}{2(1 - x)} + C$

---

## Question 4 Answer

4. Solve $\int 2x \cos x dx$ using integration by parts.
    * $f(x) = 2x, f'(x) = 2dx, g'(x) = \cos x dx, g(x) = \sin x$
    * $2x \sin x - 2\int \sin x dx$
    * $2x \sin x + 2\cos x + C$

---

## Question 5 Answer

5. Evaluate $\int_1^2 \frac{e^x}{1 - e^x} dx$
    * $u = 1 - e^x, du = -e^x dx$
    * $\int_{1 - e}^{1 - e^2} \frac{-1}{u} du$
    * $-\ln |u|_{1 - e}^{1 - e^2}$
    * $\ln |1 - e| - \ln |1 - e^2|$
    * $-\ln |1 + e|$

---

## Question 6 Answer

6. Determine $\int (4 - x^2) dx - \int (x - x^2) dx$
    * $\int (4 - x^2 - x + x^2) dx$
    * $\int (4 - x) dx$
    * $4x - \frac{x^2}{2} + C$

---

# [Next Lesson](Lesson%205)