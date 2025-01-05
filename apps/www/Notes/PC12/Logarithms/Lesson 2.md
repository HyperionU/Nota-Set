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

# Lesson 2: Intro to Logarithms

---

## The Logarithm

Remember the definition in Lesson 1?

* $y = \log_b x, b > 0, b \neq 1, x > 0$
* We have many forms:
* The Common Logarithm: $\log_10 x = \log x$ (assume 10 if no base).
* The Natural Logarithm: $\ln x = \log_e x$. This makes more sense in calculus.

---

## Conversion

<div class = "columns">

<span>

* to Logarithmic Form
    * $x = 1.3^y$
        * $y = \log_{1.3} x$
    * $x = 4^y$ 
        * $y = \log_4 x$
    * $x = (\frac{1}{2})^y$ 
        * $y = \log_{\frac{1}{2}} x$
    * $x + 3 = 3^{y - 1}$ 
        * $y - 1 = \log_3 (x - 3)$

</span>
<span>

* to Exponential Form
    * $\log_5 125 = 3$ 
        * $125 = 5^3$
    * $\log_r s = t$
        * $s = r^t$
    * $\log_x (3 - t) = 5$ 
        * $3 - t = 5^x$
    * $\log_6 x^{4x - 7}$
        * $x^{4x - 7} = 6^{2x}$

</span>
</div>

---

## Evaluating

Logarithms answer the question: What power of $b$ results in $x$?

<div class = "columns">
<span>

1) $\log_7 49$
    * 2
2) $\log_6 1$
    * 0
3) $\log_{10} 10000$
    * 4
4) $\log_2 \sqrt{8}$
    * $\frac{3}{2}$

</span>
<span>

5) $\log_{10} 0.001$
    * -3
6) $\log_2 \frac{1}{32}$
    * -5
7) $\log_5 625$
    * 4
8) $\log_2 0.25$
    * -2

</span>
</div>

---

## Exponential Growth / Applications

* Exponential Growth is a relatively rapid rate of growth. *I mean, look at the graph of $b^x$.*
* As a result, in some situations, a logarithmic scale is applied to deal with large numbers.

---

## Applications I: Earthquakes

![bg left:45% invert](https://byjus-answer-creation.s3.amazonaws.com/uploads/7886Physics_629f2fae5fa413c6820ee83e.jpg_img_upload_solution_2022-07-30%2006:59:04.511183.png)

* You may be familar with the **Richter Scale**, which measures the intensity of the earthquake.

---

## Examples

* Turkey in 1999 measured 7.4 on the Richter Scale, while Seatle in 1996 measured 5.3. How many times as intense was the Turkey earthquake?
* Start with the difference, then exponentiate.
* $7.4 - 5.3$
* $10^{2.1} \approx 126\times$ more intense

---

## Working Backwards

* If Earthquake A was measured at 2.5, and Earthquake B is 800$\times$ more intense, what is the measurement.
* Start with the logarithm, then add.
* $10^R = 800$
* $\log 800 = R$
* $R = 2.9$
* $2.5 + 2.9 = 5.4$

---

## Applications II: pH

![bg left invert](https://chem.libretexts.org/@api/deki/files/79452/CK12_Screenshot_21-9-1.png?revision=1&size=bestfit&width=402&height=502)

Another example is the pH scale.

---

## Example

* A banana has a pH of 5.2, while vinegar has a pH of 2.3. How many times as acidic is the vinegar?
* Same as Richter Scale.
* $5.2 - 2.3 = 2.9$
* $A = 10^{2.9}$
* $A \approx 794\times$ more acidic.

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%203%20(Law%20of%20Logs%20I).html)

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">