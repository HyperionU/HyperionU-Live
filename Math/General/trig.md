---
marp: true
theme: uncover
class: invert
math: mathjax
style: |
    :root{
        --que: rgb(25,7,12);
        --ans: rgb(12,25,7);
    }
    .darken{
        color: gray;
    }
backgroundColor: rgb(7,12,25)
---

$\def\half{\frac{1}{2}}$
$\def\posR{\mathbb{R}^+}$
# <!--fit--> Hyperion University Lectures

<span class="darken">By</span> Gen L.

<!--_footer: Provided by Hyperion University, © 2023--> 
$\def\csq{\cos(x)^2}$
$\def\deg{^\circ}$

---
<!--paginate: true-->

# 2. Trigonometry Fundamentals

---

## Notes

* All angles or values are in radians, unless otherwise stated.

---

## Graphs of Trig Functions

Trig functions can be affected by a multitude of factors, including:
* Amplitude
* Phase
* Period
* Vertical Shift

---
<!--_backgroundColor: var(--que)-->
## Other Factors

How about squaring the function?

1. What is the graph of $f(x)=(\cos(x))^2$?

![w:1000](https://public.itempooluserdata.com/yfFtME_lZCCHwhQWANUIv-600.webp)

---
<!--_backgroundColor: var(--ans)-->
# Answer

$f(x)=\cos(x)^2$ is similar to C.

* D can be ruled out, as there is negative values.
* Squaring smooth functions never create cusps, so we can rule out B.
* Around $x=\pi/2$, the curvature is positive, whereas A appears to have little to no curvature at all.

---
<!--_backgroundColor: var(--que)-->
## Scaled Versions

2. Working from the assumption that the graph of $\csq$ is a scaled version of $\cos(x)$, which equation is true?

* $\csq=\half(\cos(x)+1)$
* $\csq=\half(\cos(2x)+1)$
* $\csq=\half\cos(x)+1$
* $\csq=\half\cos(2x)+1$

---
<!--_backgroundColor: var(--ans)-->
# Answer
$\csq=\half(\cos(2x)+1)$

* $\csq\in\posR$, so we add 1 to get $\cos(x)+1,x\in\posR$.
* However, $\max(\cos(x)+1)=2$, so we squish by 2 to get $\half(\cos(x)+1),\max(\half(\cos(x))+1)=1$
* Then, squish the phase by 2 to get $\half(\cos(2x)+1)$.

---
<!--_backgroundColor: var(--que)-->
## Unrelated Question

3. Which of the following satisfies the equation $f(2x)=f(x)^2$?

* $f(x)=\sqrt{1-x^2}$
* $f(x)=\log(x)$
* $f(x)=x^2$
* $f(x)=2^x$

---
<!--_backgroundColor: var(--ans)-->

# Answer

$f(x)=2^x$

* $f(2x)=2^{2x}=(2^x)^2=f(x)^2$

---

## The Unit Circle

Most Trig Functions relate to this circle:

![w:500](https://giangioppo-ba-mathematics.weebly.com/uploads/4/6/7/5/46757475/unit-circle-radian.jpg?463)

---
<!--_backgroundColor: var(--que)-->
## Question 
4. Without looking it up or using a calculator, which of the following is true?

* $\sin(3)\approx0.14$ & $\cos(3)\approx0.99$
* $\sin(3)\approx0.14$ & $​\cos(​3)\approx−0.99$
* ​$\sin(3)\approx0.99$ & $\cos(3)\approx0.14$
* $\sin(3)\approx-0.99$ & $\cos(3)\approx0.14$

---
<!--_backgroundColor: var(--ans)-->
# Answer

$\sin(3)\approx0.14,\cos(3)\approx-0.99$

* Imagine starting at (1,0) on a circle with radius 1 & walking around it counterclockwise until you’ve traversed a distance of θ units along the circumference.
* $\sin(\theta)=y,\cos(\theta)=x$

---

## The Triangles

![w:750](https://cdn.kastatic.org/googleusercontent/jmY_4JbfbZhffU-tehV84DZIcmCKn1IfNAgSK8bkDRxBEd_mZNvhhaXQ2FaeUXqlQYi032pGsyF265nbejlrMD0C)

---
<!--_backgroundColor: var(--que)-->
## A Leaning Tower

5. Suppose a tower is $100\text{m}$ high. After several years, the tower starts to lean, so instead of making a $90\deg$
angle with the ground, it makes an $80\deg$ angle. When the sun is directly overhead, what is the length of the shadow cast by this leaning tower?

* $100\cdot\sin(80\deg)$
* $100\cdot\cos(80\deg)$
* $100/\sin(80\deg)$
* $100/\cos(80\deg)$

---
<!--_backgroundColor: var(--ans)-->
# Answer

$100\cdot\cos(80\deg)$

* The height of the tower of $100\text{m}$ makes the hypotenuse of a right triangle with an angle of $80\deg$. 
* The side adjacent to this angle gives the shadow of the tower, so from SOH-CAH-TOA, we can write $\cos(80\deg)=\frac{A}{H}=\frac{S}{100\text{m}}$
* After rearranging, we get $S=100\cdot\cos(80\deg)$.

---

