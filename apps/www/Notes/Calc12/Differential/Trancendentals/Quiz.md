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
$\newcommand\limit[2]{\displaystyle\lim_{#1 \to #2}}$

<!--_footer: In partnership with Hyperion University, 2025-->

---

# Unit 4 Practice Quiz

---

## Differentiation Laws

All questions here use these laws:

1. Constant: $\diff{x} c = 0$
2. Power: $\diff{x} x^n = nx^{n - 1}$
3. Sum / Difference: $\diff{x} [f(x) \pm g(x)] = \diff{x} [f(x)] \pm \diff{x} [g(x)]$
4. Product: $\diff{x} f(x) = g(x) [\diff{x} h(x)] + h(x) [\diff{x} g(x)]$
5. Quotient: $\diff{x} f(x) = \frac{h(x) (\diff{x} g(x)) - g(x) (\diff{x} h(x))}{(h(x))^2}$
6. Chain: $\diff{x} f(x) = \diff{x} g(h(x)) [\diff{x} h(x)]$ or $\diff{x} y = \diff{u} y (\diff{x} u)$
7. Sine: $\diff{x} \sin x = \cos x$
8. Cosine: $\diff{x} \cos x = \sin x$

---

<!--paginate: true-->

## Questions

1. Evaluate $\limit{x}{0} \frac{\sin^2 (4x)}{2x^2}$
2. Evaluate $\limit{x}{0} \frac{\cos x - 1}{3x}$
3. Differentiate $y = 4 \sin^2 x$
4. Differentiate $f(x) = \tan^3 5x$
5. Differentiate $y = x \cos 4x$
6. Differentiate $f(x) = \frac{\sec x}{\tan x}$
7. Differentiate $y = \csc^3 (x^2 - 1)$
8. Differentiate $y \sin x = 3x - \cos y$

---

## Question 1 Answer

1. Evaluate $\limit{x}{0} \frac{\sin^2 (4x)}{2x^2}$
    * $\limit{x}{0} \frac{\sin^2 (4x)}{2x^2}$
    * $\limit{x}{0} \frac{\sin (4x)}{2x} \limit{x}{0} \frac{\sin 4x}{x}$
    * $\limit{x}{0} \frac{2\sin (4x)}{2(2x)} \limit{x}{0} \frac{4\sin 4x}{4x}$
    * $\limit{x}{0} \frac{2\sin (4x)}{4x} \limit{x}{0} \frac{4\sin 4x}{4x}$

---

## Question 1 Answer

1. Evaluate $\limit{x}{0} \frac{\sin^2 (4x)}{2x^2}$
    * $\limit{x}{0} \frac{2\sin (4x)}{4x} \limit{x}{0} \frac{4\sin 4x}{4x}$
    * $2 (\limit{x}{0} \frac{\sin (4x)}{4x})(4)(\limit{x}{0} \frac{\sin 4x}{4x})$
    * $2(4)$
    * $8$

---

## Question 2 Answer

2. Evaluate $\limit{x}{0} \frac{\cos x - 1}{3x}$
    * $\limit{x}{0} \frac{\cos x - 1}{3x}$
    * $\limit{x}{0} \frac{1}{3} \frac{\cos x - 1}{x}$
    * $\frac{1}{3} \limit{x}{0} \frac{\cos x - 1}{x}$
    * $\frac{1}{3}(0)$
    * $0$

---

## Question 3 Answer

3. Differentiate $y = 4 \sin^2 x$
    * $u = 4v^2$
    * $v = \sin x$
    * $\diff{x} y = \diff{v} 4v^2 (\diff{x} \sin x)$
    * $\dd[y]{x} = 4(2v)(\cos x)$
    * $\dd[y]{x} = 4(2\sin x \cos x)$
    * $\dd[y]{x} = 4\sin 2x$

---

## Question 4 Answer

4. Differentiate $f(x) = \tan^3 5x$
    * $y = u^3$
    * $u = \tan v$
    * $v = 5x$
    * $\diff{x} f(x) = \diff{u} u^3 (\diff{v} \tan v)(\diff{x} 5x)$
    * $f'(x) = 3u^2 (\sec^2 v)(5)$
    * $f'(x) = 15(\tan^2 5x)(\sec^2 5x)$

---

## Question 5 Answer

5. Differentiate $y = x \cos 4x$
    * $g(x) = x$
    * $h(x) = \cos 4x$
    * $u = \cos v$
    * $v = 4x$
    * $\diff{x} y = x [\diff{v} (\cos v) (\diff{x} 4x)] + (\cos 4x)(\diff{x} x)$
    * $\dd[y]{x} = -4x(\sin 4x) + \cos 4x$
    * $\dd[y]{x} = \cos 4x - 4x(\sin 4x)$

---

## Question 6 Answer

6. Differentiate $f(x) = \frac{\sec x}{\tan x}$
    * $f(x) = \sec x \cot x$
    * $f(x) = \frac{1}{\cos x} \cdot \frac{\cos x}{\sin x}$
    * $f(x) = \frac{1}{\sin x}$
    * $f(x) = \csc x$
    * $\diff{x} f(x) = \diff{x} \csc x$
    * $f'(x) = -\cot x \csc x$

---

## Question 7 Answer

7. Differentiate $y = \csc^3 (x^2 - 1)$
    * $u = v^3$
    * $v = \csc w$
    * $w = x^2 - 1$
    * $\diff{x} y = \diff{v} v^3 (\diff{w} \csc w)[\diff{x} (x^2 - 1)]$
    * $\diff{x} y = \diff{v} v^3 (\diff{w} \csc w)[\diff{x} (x^2) - \diff{x} (1)]$
    * $\dd[y]{x} = 3v^2 (-\cot w \csc w)(2x)$
    * $\dd[y]{x} = 3\csc^2(x^2 - 1) [-\cot(x^2 - 1) \csc(x^2 - 1)](2x)$
---

## Question 7 Answer

7. Differentiate $y = \csc^3 (x^2 - 1)$
    * $\dd[y]{x} = 3\csc^2(x^2 - 1) [-\cot(x^2 - 1) \csc(x^2 - 1)](2x)$
    * $\dd[y]{x} = -6x\csc^3(x^2 - 1) \cot(x^2 - 1)$

---

## Question 8 Answer

8. Differentiate $y \sin x = 3x - \cos y$
    * $g(y) = y$
    * $h(x) = \sin x$
    * $y (\diff{} \sin x) + (\sin x) (\diff{} y) = \diff{}(3x - \cos y)$
    * $y (\diff{} \sin x) + (\sin x) (\diff{} y) = \diff{}(3x) - \diff{}(\cos y)$
    * $y(\cos x)dx + (\sin x)dy = 3dx + \sin y(dy)$
    * $\sin x(dy) - \sin y(dy) = 3dx - y(\cos x)dx$
    * $dy(\sin x - \sin y) = dx(3 - y(\cos x))$
    * $\dd[y]{x} = \frac{3 - y(\cos x)}{\sin x - \sin y}$

---

# [Next Lesson](Lesson%204)