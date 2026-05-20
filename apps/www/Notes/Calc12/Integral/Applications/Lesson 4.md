---
marp: true
theme: uncover
class: invert
math: mathjax
---

$\newcommand\diff[1]{\mathcal{d}_{#1}}$

# <!--fit--> Calculus 12 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2025-->

$\newcommand\dd[2][]{\displaystyle\frac{d#1}{d#2}}$

---

# Lesson 4: Integration by Parts

---

<!--paginate: true-->

## Intro

* Another useful method for evaluating integrals comes from the Product Rule.
* This method (Integration by Parts) works quite well for products of elementary functions.

---

## Deriving the Process

* Starting from the Product Rule: $\diff{x}(f(x)g(x)) = f(x) \diff{x} g(x) + g(x) \diff{x} f(x)$
* If we take the antiderivative, we obtain a new formula: $\int \diff{x}(f(x)g(x)) dx = \int [f(x) \diff{x} g(x)] dx + \int [g(x) \diff{x} f(x)] dx$
    * $f(x)g(x) = \int [f(x) \diff{x} g(x)] dx + \int [g(x) \diff{x} f(x)] dx$
    * And with some rearranging: $\int [f(x) \diff{x} g(x)] dx = f(x)g(x) - \int [g(x) \diff{x} f(x)] dx$
    * $\int u dv = uv - \int vdu$

---

## Practical Applications

* The practical application of this technique becomes clear as we present a number of examples. 
* A general rule of thumb is to choose the differential part to be the more complicated part that we can integrate.
* Let's take $\int \frac{x}{2} e^{2x} dx$ as our example.
    * First, take the parts: $f(x) = \frac{x}{2}, f'(x) = \frac{1}{2}, g'(x) = e^{2x}$
    * $\int \frac{x}{2} e^{2x} dx = \frac{x}{2} g(x) - \frac{1}{2} \int g(x) dx$

---

## Practical Applications, cont. 

* Let's take $\int \frac{x}{2} e^{2x} dx$ as our example.
    * $f(x) = \frac{x}{2}, f'(x) = \frac{1}{2}, g'(x) = e^{2x}$
    * $\int \frac{x}{2} e^{2x} dx = \frac{x}{2} g(x) - \frac{1}{2} \int g(x) dx$
    * $g(x) = \int e^{2x} dx = \frac{e^{2x}}{2}$
    * $\int \frac{x}{2} e^{2x} dx = \frac{x}{2} \frac{e^{2x}}{2} - \frac{1}{2} \int \frac{e^{2x}}{2} dx$
    * $\int \frac{x}{2} e^{2x} dx = \frac{xe^{2x}}{4} - \frac{1}{4} \int e^{2x} dx$
    * $\int \frac{x}{2} e^{2x} dx = \frac{xe^{2x}}{4} - \frac{e^{2x}}{8} + C$
* Now, let's do some examples.

---

## Example 1

1. Determine $\int x \cos x dx$ using integration by parts.
    * $f(x) = x, f'(x) = dx, g'(x) = \cos x dx, g(x) = \sin x$
    * $\int x \cos x dx = x\sin x - \int \sin x dx$
    * $\int x \cos x dx = x\sin x - (-\cos x) + C$
    * $\int x \cos x dx = x\sin x + \cos x + C$
* This isn't just for indefinite integrals, we can calculate definite integrals using the same technique.

---

## Example 2

2. Find $\int_0^\pi x \sin 2x dx$
    * $f(x) = x, f'(x) = dx, g'(x) = \sin 2x dx, g(x) = - \frac{1}{2} \cos 2x$
    * $\int x \sin 2x dx = -\frac{1}{2}x\cos 2x + \frac{1}{2} \int \cos 2x dx$
    * $\int x \sin 2x dx = -\frac{1}{2}x\cos 2x + \frac{1}{4} \sin 2x$
    * $\int_0^\pi x \sin 2x dx = \left[-\frac{1}{2}x\cos 2x + \frac{1}{4} \sin 2x\right]_0^\pi$
    * $\int_0^\pi x \sin 2x dx = [-\frac{1}{2}\pi\cos 2\pi + \frac{1}{4} \sin 2\pi]$ $- [-\frac{1}{2}0\cos 2(0) + \frac{1}{4} \sin 2(0)]$
    * $\int_0^\pi x \sin 2x dx = -\frac{1}{2}\pi$
* We can verify this using a graphing calculator.

---

## Definite Integration by Parts

* We can use the same derivation to determine how to evaluate definite integrals using Integration by Parts.
    * $\int_a^b \diff{x}(f(x)g(x)) dx = \int_a^b [f(x) \diff{x} g(x)] dx$ $+ \int_a^b [g(x) \diff{x} f(x)] dx$
    * $[f(x)g(x)]_a^b = \int_a^b [f(x) \diff{x} g(x)] dx + \int_a^b [g(x) \diff{x} f(x)] dx$
    * And with some rearranging: $\int_a^b [f(x) \diff{x} g(x)] dx = [f(x)g(x)]_a^b - \int_a^b [g(x) \diff{x} f(x)] dx$
    * $\int_a^b u dv = uv\rvert_a^b - \int_a^b vdu$
* This means we can evaluate each part separately!

---

## Example 3

3. Find $\int x \ln x dx$
    * $f(x) = \ln x, f'(x) = \frac{1}{x} dx, g'(x) = x dx, g(x) = \frac{x^2}{2}$
    * $\int x \ln x dx = \ln x \frac{x^2}{2} - \int \frac{x^2}{2} \frac{1}{x} dx$
    * $\int x \ln x dx = \ln x \frac{x^2}{2} - \frac{1}{2} \int x dx$
    * $\int x \ln x dx = \frac{x^2 \ln x}{2} - \frac{x^2}{4} + C$
    * This works, but if we write it as a single fraction: $\int x \ln x dx = \frac{x^2 (2\ln x - 1)}{4} + C$

---

## Exercise for Readers

* Evaluate the following:
    * $\int (2x + 1)e^{-x} dx$
    * $\int x \cos 3x dx$
    * $\int x \sec^2 x dx, \int \tan x = - \ln |\cos x|$
    * $\int \frac{xe^x}{2} dx$
    * $\int_0^\pi 2x \cos x dx$
    * $\int_0^\frac{\pi}{2} 2x \cos x dx$

---

# [Next Lesson](Lesson%205)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* Evaluate $\int (2x + 1)e^{-x} dx$
    * $f(x) = 2x + 1, f'(x) = 2 dx, g'(x) = e^{-x} dx, g(x) = -e^{-x}$
    * $\int (2x + 1)e^{-x} dx = -(2x + 1)e^{-x} + 2 \int e^{-x} dx$
    * $\int (2x + 1)e^{-x} dx = -(2x + 1)e^{-x} - 2 e^{-x} + C$
* Evaluate $\int x \cos 3x dx$
    * $f(x) = x, f'(x) = dx, g'(x) = \cos 3x dx, g(x) = \frac{1}{3} \sin 3x$
    * $\int x \cos 3x dx = \frac{x}{3} \sin 3x - \frac{1}{3} \int \sin 3x dx$
    * $\int x \cos 3x dx = \frac{x}{3} \sin 3x + \frac{1}{9} \cos 3x + C$

---

## Answers to Exercises, cont.

* Evaluate $\int x \sec^2 x dx, \int \tan x = - \ln |\cos x|$
    * $f(x) = x, f'(x) = dx, g'(x) = \sec^2 x dx, g(x) = \tan x$
    * $\int x \sec^2 x dx = x \tan x - \int \tan x dx$
    * $\int x \sec^2 x dx = x \tan x + \ln |\cos x| + C$
* Evaluate $\int \frac{xe^x}{2} dx$
    * $f(x) = \frac{x}{2}, f'(x) = \frac{1}{2} dx, g'(x) = e^x dx, g(x) = e^x$
    * $\int \frac{xe^x}{2} dx = \frac{xe^x}{2} - \frac{1}{2}\int e^x dx$
    * $\int \frac{xe^x}{2} dx = \frac{(x - 1)e^x}{2} + C$

---

## Answers to Exercises, cont.

* Evaluate $\int_0^\pi 2x \cos x dx$
    * $f(x) = 2x, f'(x) = 2 dx, g'(x) = \cos x dx, g(x) = \sin x$
    * $\int_0^\pi 2x \cos x dx = 2[x \sin x]_0^\pi - 2\int_0^\pi \sin x dx$
    * $\int_0^\pi 2x \cos x dx = -2\int_0^\pi \sin x dx$
    * $\int_0^\pi 2x \cos x dx = 2(\cos \pi - \cos 0)$
    * $\int_0^\pi 2x \cos x dx = -4$

---

## Answers to Exercises, cont.

* Evaluate $\int_0^\frac{\pi}{2} 2x \cos x dx$
    * $f(x) = 2x, f'(x) = 2 dx, g'(x) = \cos x dx, g(x) = \sin x$
    * $\int_0^\frac{\pi}{2} 2x \cos x dx = 2[x \sin x]_0^\frac{\pi}{2} - 2\int_0^\frac{\pi}{2} \sin x dx$
    * $\int_0^\frac{\pi}{2} 2x \cos x dx = 2(\frac{\pi}{2}) - 2\int_0^\frac{\pi}{2} \sin x dx$
    * $\int_0^\frac{\pi}{2} 2x \cos x dx = 2(\frac{\pi}{2}) + 2(\cos \frac{\pi}{2} - \cos 0)$
    * $\int_0^\frac{\pi}{2} 2x \cos x dx = \pi - 2$

---

# [Next Lesson](Lesson%205)