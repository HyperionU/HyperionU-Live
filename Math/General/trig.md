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
$\def\csq{\cos^2(x)}$
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

1. What is the graph of $f(x)=\cos^2(x)$?

![w:1000](https://public.itempooluserdata.com/yfFtME_lZCCHwhQWANUIv-600.webp)

---
<!--_backgroundColor: var(--ans)-->
# Answer

$f(x)=\cos^2(x)$ is similar to C.

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
* Then, squish the period by 2 to get $\half(\cos(2x)+1)$.

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

## How to Compute Values

* Some values of radians are special.
* $\pi=180\deg,2\pi=360\deg$
* $90\deg=\frac{\pi}{2}$, so every 90 degrees add $\pi/2$.

---
<!--_backgroundColor: var(--que)-->
## On Computing Values

6. What is $\sin(\frac{\pi}{6})$?

* $\half$
* $\frac{\sqrt{2}}{2}$
* $\frac{\sqrt{3}}{2}$
* $\frac{\sqrt{5}}{2}$

---
<!--_backgroundColor: var(--ans)-->
# Answer

$\sin(\frac{\pi}{6})=\frac{1}{2}$

* $\frac{\pi}{6}\text{ radians}\equiv30\deg$
* Using 30-60-90 triangles and SOH-CAH-TOA, $\sin(30\deg)=\half$
* $\therefore\sin(\frac{\pi}{6})=\half$ 

---
<!--_backgroundColor: var(--que)-->
## Cosine

7. What is $\cos(\frac{\pi}{6})$?

* $\half$
* $\frac{\sqrt{2}}{2}$
* $\frac{\sqrt{3}}{2}$
* $\frac{\sqrt{5}}{2}$

---
<!--_backgroundColor: var(--ans)-->
# Answer

$\cos(\frac{\pi}{6})=\frac{\sqrt{3}}{2}$

* $\frac{\pi}{6}\text{ radians}\equiv30\deg$
* Using 30-60-90 triangles and SOH-CAH-TOA, $\cos(30\deg)=\frac{\sqrt{3}}{2}$
* $\therefore\cos(\frac{\pi}{6})=\frac{\sqrt{3}}{2}$ 

---
<!--_backgroundColor: var(--que)-->
## 'Circle' Back

8. What is $\cos(-\frac{2\pi}{3})$?

* $\half$
* $-\half$
* $\frac{\sqrt{3}}{2}$
* $-\frac{\sqrt{3}}{2}$

---
<!--_backgroundColor: var(--ans)-->
# Answer
* $-\half$
* This diagram illustrates the point $-\frac{2\pi}{3}$ radians around the circle. 
* This forms a 30-60-90 triangle revealing that the x-coordinate of the point is $-\half$.

![bg left invert:100%](https://public.itempooluserdata.com/lPNaQMCu4sLYdHGlo7j4F-398.webp)

---
<!--_backgroundColor: var(--que)-->
## Exact Values of Non-Exact Angles

9. What is $\cos(\frac{\pi}{12})$?

* $\sqrt{(\frac{1-\sqrt{3}/2}{2})}$
* $\sqrt{(\frac{1+\sqrt{3}/2}{2})}$
* $\sqrt{\frac{\sqrt{3}}{4}}$
* $\frac{\sqrt{3}}{4}$

---
<!--_backgroundColor: var(--ans)-->
# Answer

* $\sqrt{(\frac{1+\sqrt{3}/2}{2})}$
* Noting that $\cos^2(x)=\frac{1+\cos(2x)}{2}$, that we found by playing with graphs, then let $x=\frac{\pi}{12}$. 
* Together with the fact that $\cos(\frac{\pi}{6})=\frac{\sqrt{3}}{2}$, we get: $\cos^2(\frac{\pi}{12})=\frac{1+\sqrt{3}/2}{2},\ \therefore\cos(\frac{\pi}{12})=\sqrt{(\frac{1+\sqrt{3}/2}{2})}$.

---
<!--_backgroundColor: var(--que)-->
## Advanced Trig Functions

10. Which is the graph of $\tan(x)$?

![h:300](https://public.itempooluserdata.com/QjhF7lIZ1NTQbhi5AfJhy-600.webp)

---
<!--_backgroundColor: var(--ans)-->
# Answer
* A
* The key is to note that $\tan(0)=0$, and as $\theta\to\frac{\pi}{2},\tan(\theta)\to\infty$. Only graph A exhibits this pattern.

---

## Determining $\tan(x)$: Visual 1

* There are two ways to see this.  One is to look at the visual below and to see how the relevant tangent line off the circle has a length $\ell=[0,\infty]$.
![invert:1](https://public.itempooluserdata.com/K82qKhn-rLKDdCy9WYjHW-1120.webp)

---

## Determining $\tan(x)$: Visual 2

The other way is that $\tan(\theta)=\frac{\sin(\theta)}{\cos(\theta)}$, and consider this fraction as we range $\theta=[0,\frac{\pi}{2}]$. At 
$\theta=0,\sin(\theta)=0$, so the fraction equals 0, while at $\theta=\frac{\pi}{2},\cos(\theta)\to0\therefore\tan(\theta)\to\infty$.

---

## Challenge:

* Pick an integer: $x\in\mathbb{Z}$. Which integer will be the most popular choice?