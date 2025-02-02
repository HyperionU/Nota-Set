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

# Lesson 3: Sum & Difference Identities

---

## Sum & Difference

Is $\cos(A + B) = \cos A + \cos B$? 
* **No!**
* Remember, cosine is a function, but without an angle, it means nothing. 
* Therefore, we cannot distribute the function through.

---

## The Identities

9. $\cos(A \pm B) = \cos A \cos B \mp \sin A \sin B$
Check using $A = \frac{\pi}{6}, B = \frac{\pi}{3}$
    * $\cos(\frac{\pi}{6} + \frac{\pi}{3}) = \cos \frac{\pi}{6} \cos \frac{\pi}{3} - \sin \frac{\pi}{6} \sin \frac{\pi}{3}$
    * $\cos(\frac{\pi}{2}) = \frac{\sqrt{3}}{6} (\frac{1}{2}) - \frac{1}{2} (\frac{\sqrt{3}}{2})$
    * $0 = 0$
10. $\sin(A \pm B) = \sin A \cos B \pm \cos A \sin B$
11. $\tan(A \pm B) = \frac{\tan A \pm \tan B}{1 \mp \tan A \tan B}$

What can we do with these?

---

## Simplification

Write as a single trig function: $\sin \frac{5\pi}{6} \cos \frac{3\pi}{8} - \cos \frac{5\pi}{6} \sin \frac{3\pi}{8}$

$\sin(\frac{5\pi}{6} - \frac{3\pi}{8})$
$\sin(\frac{11\pi}{24})$

Write as a single trig function: $\frac{\tan 30^\circ + \tan 45^\circ}{1 - \tan 30^\circ \tan 45^\circ}$

$\tan(30^\circ + 45^\circ)$
$\tan(75^\circ)$

---

## Exact Values

If the angle is a sum or difference of 2 special angles, we can find the exact value.

$\sin 75^\circ$
$\sin(30^\circ + 45^\circ)$
$\sin 30^\circ \cos 45^\circ + \cos 30^\circ \sin 45^\circ$
$\frac{1}{2} (\frac{1}{\sqrt{2}}) + \frac{\sqrt{3}}{2} (\frac{1}{\sqrt{2}})$
$\frac{1 + \sqrt{3}}{2 \sqrt{2}}$

---

## Proofs

Let's try proving more identities.

$\frac{\cos(x - y)}{\sin x \cos y} = \cot x + \tan y$

$$
    \begin{array}{c|c}
        \hline
        \frac{\cos(x - y)}{\sin x \cos y} & \cot x + \tan y \\
        \frac{\cos x \cos y + \sin x \sin y}{\sin x \cos y} & \frac{\cos x}{\sin x} + \frac{\sin y}{\cos y} \\
        \frac{\cos x \cos y + \sin x \sin y}{\sin x \cos y} & \frac{\cos x \cos y + \sin x \sin y}{\sin x \cos y}
    \end{array}
$$

---

## Simplification

Simplify $\sin(\frac{3\pi}{2} - x)$

$\sin \frac{3\pi}{2} \cos x - \cos \frac{3\pi}{2} \sin x$
$-1 (\cos x) - 0 (\sin x)$
$-\cos x$

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%204%20(Double%20Angle).html)

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">