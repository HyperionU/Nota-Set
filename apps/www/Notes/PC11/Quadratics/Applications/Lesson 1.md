---
marp: true
theme: uncover
class: invert
paginate: true
math: mathjax
---

# <!--fit--> Pre-Calculus 11 Notes
<span style="color:grey">By:</span> Gen L.

<!--_footer: In partnership with Hyperion University, 2023-->

---

## Lesson 1: Applications, Part 1

---

## Example 1: Maximum Revenue (w/ Function)

* A tractor company has found that the revenue from sales of their heavy-duty tractors is a function of the unit price ($p$) charged. The revenue ($R$) is:
* $R=-\frac{1}{2}p^2+1900p$
1) What unit price ($p$) should be charged to maximise revenue?
2) What is the maximum revenue ($\max(R)$)?

---

## Solving Example 1

* Whenever you are dealing with a maximum revenue question, **ALWAYS** put the function into vertex form. (Complete the Square)
   
* $R=-\frac{1}{2}p^2+1900p$
    * $R=-0.5(p^2-3800p+c)-(-0.5c)$
    * $R=-0.5(p^2-3800p+3610000)+1805000$
    * $R=-0.5(p-1900)^2+1805000$
    * $V(1900,1.805\cdot10^6)$
* To maximise revenue, they should charge $1900, The maximum revenue would be $1 805 000.

---

## Example 2: Maximum Revenue (w/o Function)
* Calculators are sold to students for $20 each. 300 students are willing to buy them at that price. For every $5 increase in price, there are 30 fewer students willing to buy a calculator.
1) What selling price ($p$) will produce the maximum sales?
2) What will the maximum revenue be? ($\max(R)$)

---

## Solving Example 2

* *Note*: Revenue ($R$) is equal to Price ($p$) multiplied by Quantity ($q$).
* $\text{let }x=\text{amount of price increases by } 5$.
    * $P=20+5x,Q=300-30x$.
    * $R=(20+5x)(300-30x)$
        * FOIL, then complete the square.
    * $R=-150x^2+900x+6000$
    * $R=-150(x^2-6x+c)+6000-(-150c)$
    * $R=-150(x^2-6x+9)+6000+1350$
    * $R=-150(x-3)^2+7350$

---

## Solving Example 2, cont.

* From this, we see that $\max(R)=7350, \text{when } x=3$.
* We can determine that $p=35,q=210$.

---

## Example 3: Simple Area

* At a concert, organisers are roping off a rectangular area for sound equipment. There is 160m of fencing available to create the perimeter.
1) What dimensions will give the maximum area ($lw$)?
2) What is the Maximum Area ($\max(A)$)?

---

## Solving Example 3

* We know that both Perimeter ($P$) is $2(\ell+w)$, where $\ell$ is the length, $w$ is the width, and Area ($A$) is $\ell w$.
    * $160=2(\ell+w)$
    * $80=\ell+w$
    * $80-\ell=w$
    * $A=\ell(80-\ell)$
    * $A=-\ell^2+80\ell$

---

## Solving Example 3, cont.

* Now, we've combined the two equations, and are attempting to solve for $\max(A),\ell, w$.
    * $A=-(\ell^2-80\ell+c)-(-c)$
    * $A=-(\ell^2-80\ell+1600)+1600$
    * $A=-(\ell-40)^2+1600$
    $\therefore$
* $\max(A)=1600m^2, w=40m, \ell=40$

---

# [Next Lesson <i class="fa-solid fa-circle-arrow-right"></i>](Lesson%202%20(Applications%20Part%202).html) 

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css">
