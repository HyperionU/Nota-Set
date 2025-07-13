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

<!--_footer: In partnership with Hyperion University, 2025-->

---

# Lesson 5: Applications in Biological Sciences

---

<!--paginate: true-->

## Intro 

* For any function $f(x)$, its derivative $f'(x)$ represents the rate of change of the function for any value in the domain.
* For the Biological Sciences, we use these to model continuous changes like growth and decay.

---

## Exponential Growth and Decay

* For most cases, the function for continuous exponential growth and decay is $f(t) = Ae^{kt}$. We'll derive this when we get to Differential Equations.
* This function models growth and decay as a function of time where:
    * $t$ is time (in some time-based unit).
    * $A$ is the initial amount of substance.
    * $k$ is some constant. If $k > 0$, then the function will grow. If $k < 0$, then the function will decay.

---

## Growth and Decay, cont.

* We could therefore rewrite $f(t) = Ae^{kt}$ as $f(t) = f(0)e^{kt}$. 
(*I don't know why you would, but you can I guess.*)
* Many functions which grow or decay exponentially are discrete, but can be modeled with this continuous function.
* Because the growth and decay are exponential, the rate of growth or decay is also changing.
* Typically, we'd use the derivative to determine this rate at any particular time.

---

## Example 1

1. The number of bacteria in a particular culture after $t$ hours is known to be $f(t) = 1000e^{(\frac{1}{2} \ln 4)t}$.
    * What is the rate of the bacterial growth after $t$ hours?
        * $\diff{t} f(t) = \diff{t} (1000e^{(\frac{1}{2} \ln 4)t})$
        * $f'(t) = \frac{1}{2}\ln 4(1000e^{(\frac{1}{2} \ln 4)t})$
        * $f'(t) = 500\ln 4e^{(\frac{1}{2} \ln 4)t}$

---

## Example 1, cont.

1. The number of bacteria in a particular culture after $t$ hours is known to be $f(t) = 1000e^{(\frac{1}{2} \ln 4)t}$.
    * $f'(t) = 500\ln 4e^{(\frac{1}{2} \ln 4)t}$
    * What is the rate of the bacterial growth after 5 hours?
        * $f'(5) = 500\ln 4e^{(\frac{1}{2} \ln 4)5}$
        * $f'(5) \approx 22180.71$

* The answer to these questions is better as a decimal approximation than as an exact answer.

---

## Example 2

2. The mass of a radioactive substance, in grams, after $t$ days is known to be $f(t) = 100e^{-\frac{\ln 2}{125}t}$
    * What is the rate of radioactive decay after $t$ days?
        * $\diff{t} f(t) = \diff{t} (100e^{-\frac{\ln 2}{125}t})$
        * $f'(t) = -\frac{\ln 2}{125}(100e^{-\frac{\ln 2}{125}t})$
        * $f'(t) = -\frac{4\ln 2}{5}(e^{-\frac{\ln 2}{125}t})$
    * What is the rate of radioactive decay after 100 days?
        * $f'(100) = -\frac{4\ln 2}{5}e^{(-\frac{\ln 2}{125})100}$
        * $f'(100) = -\frac{4\ln 2}{5}e^{-\frac{4\ln 2}{5}}$

---

## Example 2, cont.

2. The mass of a radioactive substance, in grams, after $t$ days is known to be $f(t) = 100e^{-\frac{\ln 2}{125}t}$
    * What is the rate of radioactive decay after 100 days?
        * $f'(100) = -\frac{4\ln 2}{5}e^{-\frac{4\ln 2}{5}}$
        * $f'(100) \approx -0.318\text{g/day}$

---

## Example 3

3. The number of bacteria in a particular culture after $t$ hours is known to be $f(t) = 3000e^{(\frac{1}{4} \ln 5)t}$. How long will it take for the growth rate to be 10000 bacteria/hr?
    * $\diff{t} f(t) = \diff{t} (3000e^{(\frac{1}{4} \ln 5)t})$
    * $f'(t) = (\frac{3000}{4} \ln 5)e^{(\frac{1}{4} \ln 5)t}$
    * $f'(t) = (750 \ln 5)e^{(\frac{1}{4} \ln 5)t}$
    * $10000 = (750 \ln 5)e^{(\frac{1}{4} \ln 5)t}$
    * $\frac{10000}{750 \ln 5} =e^{(\frac{1}{4} \ln 5)t}$
    * $\frac{40}{3 \ln 5} = e^{(\frac{1}{4} \ln 5)t}$

---

## Example 3, cont.

3. The number of bacteria in a particular culture after $t$ hours is known to be $f(t) = 3000e^{(\frac{1}{4} \ln 5)t}$. How long will it take for the growth rate to be 10000 bacteria/hr?
    * $\frac{40}{3 \ln 5} = e^{(\frac{1}{4} \ln 5)t}$
    * $\ln (\frac{40}{3 \ln 5}) = (\frac{1}{4} \ln 5)t$
    * $t = \frac{\ln (\frac{40}{3 \ln 5})}{(\frac{1}{4} \ln 5)}$
    * $t = \frac{\ln (\frac{40}{3 \ln 5})}{(\frac{1}{4} \ln 5)}$
    * $t \approx 5.25\text{hrs}$

---

## Example 4a

4. A bacteria culture has an initial count of 500. After 4 hours, there are 2000 bacteria present.
    * What is the function for the amount of bacteria?
        * $f(4) = 2000$
        * $A = 500$
        * $2000 = 500e^{4k}$
        * $\frac{2000}{500} = e^{4k}$
        * $4 = e^{4k}$
        * $\ln 4 = 4k$
        * $k = \frac{\ln 4}{4}$

---

## Example 4b

4. A bacteria culture has an initial count of 500. After 4 hours, there are 2000 bacteria present.
    * $f(t) = 500e^{\frac{\ln 4}{4} t}$
    * What is the growth rate after t hours?
        * $\diff{t} f(t) = \diff{t} (500e^{\frac{\ln 4}{4} t})$
        * $f'(t) = \frac{\ln 4}{4}(500e^{\frac{\ln 4}{4} t})$
        * $f'(t) = 125\ln 4(e^{\frac{\ln 4}{4} t})$

---

## Example 4c

4. A bacteria culture has an initial count of 500. After 4 hours, there are 2000 bacteria present.
    * $f'(t) = 125\ln 4(e^{\frac{\ln 4}{4} t})$
    * What is the growth rate after 6 hours?
        * $f'(6) = 125\ln 4(e^{\frac{\ln 4}{4} 6})$
        * $f'(6) = 125\ln 4(e^{\frac{3\ln 4}{2}})$
        * $f'(6) \approx 1386.3$

---

## Example 4d

4. A bacteria culture has an initial count of 500. After 4 hours, there are 2000 bacteria present.
    * $f'(t) = 125\ln 4(e^{\frac{\ln 4}{4} t})$
    * How long does it take for the growth rate to reach 11000 bacteria / hr?
        * $11000 = 125\ln 4(e^{\frac{\ln 4}{4} t})$
        * $\frac{11000}{125\ln 4} = e^{\frac{\ln 4}{4} t}$
        * $\frac{88}{\ln 4} = e^{\frac{\ln 4}{4} t}$
        * $\ln \frac{88}{\ln 4} = \frac{\ln 4}{4} t$

---

## Example 4d, cont.

4. A bacteria culture has an initial count of 500. After 4 hours, there are 2000 bacteria present.
    * How long does it take for the growth rate to reach 11000 bacteria / hr?
        * $\ln \frac{88}{\ln 4} = \frac{\ln 4}{4} t$
        * $t = \frac{\ln \frac{88}{\ln 4}}{\frac{\ln 4}{4}}$
        * $t \approx 11.98\text{hrs}$

---

## Exercise for Readers

* The mass, in grams, of a radioactive substance remaining after $t$ days is given by $f(t) = 35e^{-\frac{\ln 3}{40} t}$
    * What is the decay rate after t days?
    * What is the decay rate after 20 days?
* The number of bacteria after $t$ hours is given by $f(t) = 1500e^{\frac{\ln 3}{7} t}$
    * What is the growth rate after 5 hours?
    * How long would it take for the rate to reach 2000 bacteria / hr?

---

## Exercise for Readers, cont.

* A sample of a radioactive substance has a mass of 100g. After 30 days, the mass has decreased to 25g.
    * What is the mass after t days?
    * What is the decay rate after t days?
    * How long until the rate reaches -3g / day?

---

# [Next Lesson](Lesson%206)

<!--_footer: Next page for exercise answers! -->

---

## Answers to Exercises

* The mass, in grams, of a radioactive substance remaining after $t$ days is given by $f(t) = 35e^{-\frac{\ln 3}{40} t}$
    * What is the decay rate after t days?
        * $\diff{t} f(t) = \diff{t} (35e^{-\frac{\ln 3}{40} t})$
        * $f'(t) = -\frac{\ln 3}{40}(35e^{-\frac{\ln 3}{40} t})$
        * $f'(t) = -\frac{7\ln 3}{8}e^{-\frac{\ln 3}{40} t}$
    * What is the decay rate after 20 days?
        * $f'(20) = -\frac{7\ln 3}{8}e^{-\frac{\ln 3}{40} 20}$
        * $f'(20) = -\frac{7\ln 3}{8}e^{-\frac{\ln 3}{2}}$

 ---

## Answers to Exercises, cont.

* The mass, in grams, of a radioactive substance remaining after $t$ days is given by $f(t) = 35e^{-\frac{\ln 3}{40} t}$
    * What is the decay rate after 20 days?
        * $f'(20) = -\frac{7\ln 3}{8}e^{-\frac{\ln 3}{2}}$
        * $f'(20) \approx -0.555\text{g/day}$

---

## Answers to Exercises, cont.

* The number of bacteria after $t$ hours is given by $f(t) = 1500e^{\frac{\ln 3}{7} t}$
    * What is the growth rate after 5 hours?
        * $\diff{t} f(t) = \diff{t} (1500e^{\frac{\ln 3}{7} t})$
        * $f'(t) = \frac{1500\ln 3}{7}e^{\frac{\ln 3}{7} t}$
        * $f'(5) = \frac{1500\ln 3}{7}e^{\frac{\ln 3}{7} 5}$
        * $f'(5) \approx 516\text{ bacteria/hr}$

---

## Answers to Exercises, cont.

* The number of bacteria after $t$ hours is given by $f(t) = 1500e^{\frac{\ln 3}{7} t}$
    * How long would it take for the rate to reach 2000 bacteria / hr?
        * $f'(t) = \frac{1500\ln 3}{7}e^{\frac{\ln 3}{7} t}$
        * $2000 = \frac{1500\ln 3}{7}e^{\frac{\ln 3}{7} t}$
        * $2000 / \frac{1500\ln 3}{7} = e^{\frac{\ln 3}{7} t}$
        * $\frac{28}{3\ln 3} = e^{\frac{\ln 3}{7} t}$
        * $\ln \frac{28}{3\ln 3} = \frac{\ln 3}{7} t$

---

## Answers to Exercises, cont.

* The number of bacteria after $t$ hours is given by $f(t) = 1500e^{\frac{\ln 3}{7} t}$
    * How long would it take for the rate to reach 2000 bacteria / hr?
        * $\ln \frac{28}{3\ln 3} = \frac{\ln 3}{7} t$
        * $t = \frac{\ln \frac{28}{3\ln 3}}{\frac{\ln 3}{7}}$
        * $t \approx 13.6\text{hrs}$

---

## Answers to Exercises, cont.

* A sample of a radioactive substance has a mass of 100g. After 30 days, the mass has decreased to 25g.
    * What is the mass after t days?
        * $25 = 100e^{30k}$
        * $\frac{1}{4} = e^{30k}$
        * $\ln 2^{-2} = 30k$
        * $k = \frac{-2 \ln 2}{30}$
        * $k = -\frac{\ln 2}{15}$
        * $f(t) = 100e^{-\frac{\ln 2}{15} t}$

---

## Answers to Exercises, cont.

* A sample of a radioactive substance has a mass of 100g. After 30 days, the mass has decreased to 25g.
    * $f(t) = 100e^{-\frac{\ln 2}{15} t}$
    * What is the decay rate after t days?
        * $\diff{t} f(t) = \diff{t} (100e^{-\frac{\ln 2}{15} t})$
        * $f'(t) = -\frac{\ln 2}{15} (100e^{-\frac{\ln 2}{15} t})$
        * $f'(t) = -\frac{20\ln 2}{3} e^{-\frac{\ln 2}{15} t}$

---

## Answers to Exercises, cont.

* A sample of a radioactive substance has a mass of 100g. After 30 days, the mass has decreased to 25g.
    * $f'(t) = -\frac{20\ln 2}{3}e^{-\frac{\ln 2}{15} t}$
    * How long until the rate reaches -3g / day?
        * $3 = \frac{20\ln 2}{3}e^{-\frac{\ln 2}{15} t}$
        * $3 / \frac{20\ln 2}{3} = e^{-\frac{\ln 2}{15} t}$
        * $\frac{9}{20\ln 2} = e^{-\frac{\ln 2}{15} t}$
        * $\ln \frac{9}{20\ln 2} = -\frac{\ln 2}{15} t$
        * $t = -\frac{\ln \frac{9}{20\ln 2}}{\frac{\ln 2}{15}}$

---

## Answers to Exercises, cont.

* A sample of a radioactive substance has a mass of 100g. After 30 days, the mass has decreased to 25g.
    * $f'(t) = -\frac{20\ln 2}{3}e^{-\frac{\ln 2}{15} t}$
    * How long until the rate reaches -3g / day?
        * $t = -\frac{\ln \frac{9}{20\ln 2}}{\frac{\ln 2}{15}}$
        * $t \approx 9.35\text{ days}$

---

# [Next Lesson](Lesson%206)