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

$\def\setR{\mathbb{R}}$
$\def\pis{\frac{\pi}{6}}$
# <!--fit--> Hyperion University Lectures

<span class="darken">By</span> Gen L.

<!--_footer: Provided by Hyperion University, © 2023--> 
$\def\setC{\mathbb{C}}$
$\newcommand\zro[2]{\cos({#1})+i\sin({#2})}$

---

$\def\deg{^\circ}$
$\def\cfour{\frac{\sqrt{2}}{2}}$

<!--paginate: true-->

# 3. Complex Numbers Fundamentals

$\newcommand\zid[1]{\cos({#1})+i\sin({#1})}$
$\def\ext{\frac{\sqrt{3}}{2}+i\frac{1}{2}}$

---

## What are Complex Numbers?

* Take the equation $x^2+1=0$. 
* Using square root principle, we get $x=\pm\sqrt{-1}$, which is not possible in the real numbers. 
* We write in this case that $x\notin\setR$, but actually, $x\in\setC$.
* These complex numbers extend the real number line into a plane with a lateral unit, $i$, where $i=\sqrt{-1}$.

---
<!--_backgroundColor: var(--que)-->
## Question

![invert w:800 bg left:50%](https://public.itempooluserdata.com/3lTpk2b9QlVZf7iHIxysE-435.webp)

1. What is $(4+i)+(-2+2i)$?

---
<!--_backgroundColor: var(--ans)-->
# Answer

* $2+3i$
* By combining like terms, we get $(4-2)+(i+2i)=2+3i$.
* This is similar to adding polynomials, maybe there's a similarity...

---
<!--_backgroundColor: var(--que)-->
## Rotations

![invert bg left](https://public.itempooluserdata.com/EQIYfjAMsANO9Kw-AUhz5-313.webp)

2. If you rotate the point $(3,2)$ by $90\deg$ counterclockwise, about the origin, where does it land?

* $(-3,2)$
* $(3,-2)$
* $(-2,3)$
* $(2,-3)$

---
<!--_backgroundColor: var(--ans)-->
# Answer

* $(-2,3)$

* Rotating the whole picture $90\deg$
counterclockwise, you can read off the vector as now being at $(-2,3)$.
* Generally, a point $(x,y)$ when rotated by $90\deg$, will become $(-y,x)$. 
* The point of this exercise is to emphasise how swapping the coordinates and negating one like this corresponds to a $90\deg$ rotation.

---
<!--_backgroundColor: var(--que)-->
## Complex Multiplication

![invert w:600 bg left](https://public.itempooluserdata.com/AlaFKVHTSAqD0kQ-VGmZg-361.webp)

3. What is $i(3+2i)$?

---
<!--_backgroundColor: var(--ans)-->
# Answer

* $-2+3i$
* Distributing, and using the fact that $i^2=-1$, we get: $i(3+2i)=3i+2i^2=3i+2(-1)=-2+3i$
Notice how simply by virtue of the rule $i^2=-1$, the effect of this product was to swap the coordinates and negate one of them.  And just a moment ago we saw that this operation corresponds to the $90\deg$ rotation even before imaginary numbers are brought into the mix.

---
<!--_backgroundColor: var(--que)-->
## **More** Complex Multiplication

![invert bg left](https://public.itempooluserdata.com/L5BcBIgvjzj7ZUvp6cAmx-327.webp)

4. What is $(2-i)(2+i)$

---
<!--_backgroundColor: var(--ans)-->
# Answer

* 5 (*yes, this is the answer*)
* Using FOIL, we get: $(2-i)(2+i)=2^2+2i-2i-i^2$
* Simplifying, we get: $4-(-1)=4+1=5$

---
<!--_backgroundColor: var(--que)-->
## Converting Rotations to Complex

5. What is the complex number $z$ such that multiplying by $z$ has a similar effect to rotating $30\deg$ or $\frac{\pi}{6}$ radians?

* $z=1+\pis{i}$
* $z=\sqrt{1-(\pis)^2}+\pis{i}$
* $z=\sin(\pis)+i\cos(\pis)$
* $z=\zro{\pis}{\pis}$

---
<!--_backgroundColor: var(--ans)-->
# Answer

![invert bg left](https://public.itempooluserdata.com/WXL2x2Ivge1gphWrUR2qv-398.webp)

* $z=\zro{\pis}{\pis}$
* Multiplication by a complex number $z$ has the effect of scaling and rotating other values.

---
<!--_backgroundColor: var(--que)-->
## Trigonometry

6. What is the exact value of $\cos(75\deg)$?

* $\frac{\sqrt{6}-\sqrt{3}}{4}$
* $\frac{\sqrt{6}-\sqrt{2}}{4}$
* $\frac{\sqrt{6}+\sqrt{3}}{4}$
* $\frac{\sqrt{6}+\sqrt{2}}{4}$

---
<!--_backgroundColor: var(--ans)-->

# Answer

* $\frac{\sqrt{6}-\sqrt{2}}{4}$
* The complex number with the effect of rotating $45\deg$: $z=\zid{45\deg}=\cfour+i\cfour$
* The complex number with the effect of rotating $30\deg$: $w=\zid{30\deg}=\ext$.

---
<!--_backgroundColor: var(--ans)-->
# Answer, cont.

* Taking the product directly, we get: $zw=(\cfour+i\cfour)(\ext)$
$zw=\frac{\sqrt{2\cdot3}}{4}-\frac{\sqrt{2}}{4}+(\frac{\sqrt{2\cdot3}}{4}-\frac{\sqrt{2}}{4})i$
$zw=\frac{\sqrt{6}-\sqrt{2}}{4}+\frac{\sqrt{6}-\sqrt{2}}{4}i$

---
<!--_backgroundColor: var(--que)-->
## Complex Quadratics

7. Which of the following values of $z$ satisfies the equation $z^2=i$?

* $\cfour+\cfour{i}$
* $-\frac{1}{2}+\frac{\sqrt{3}}{2}i$ 
* $1-i$
* $z\notin\setC$

---
<!--_backgroundColor: var(--ans)-->
# Answer

![invert bg left](https://public.itempooluserdata.com/gn9lv3PDF49mFSKvJPkpC-398.webp)

* $\cfour+\cfour{i}$
* Since multiplying by $i$ is similar to a $90\deg$ rotation, using trigonometry: $z=\zid{45\deg}$
$=\cfour+\cfour{i}$

---
<!--_backgroundColor: var(--que)-->
## Complex Cubics

8. The equation $x^3=1$ has a real solution, $x=1$. Among the complex numbers, there are two more solutions.  Which of the following is one of them?

* $\frac{1}{2}+\frac{\sqrt{3}}{2}i$
* $-\frac{1}{2}+\frac{\sqrt{3}}{2}i$
* $\frac{\sqrt{3}}{2}+\frac{1}{2}i$
* None of the Above

---
<!--_backgroundColor: var(--ans)-->
## Answer

![invert bg left](https://public.itempooluserdata.com/KTAfl2ecIqYxojrq4JGQI-398.webp)

* $-\frac{1}{2}+\frac{\sqrt{3}}{2}i$
* Thinking in terms of rotations, a number which has the effect of rotating by a third of a turn, is what we need.
* Using trigonometry, we get: $x=\zid{\frac{2\pi}{3}}$
$=-\frac{1}{2}+\frac{\sqrt{3}}{2}$

---
<!--_backgroundColor: var(--que)-->
## Functional Properties

9. Which function has this property: $f(a+b)=f(a)f(b), f:x\to{y}$

* $f(x)=\log(x)$
* $f(x)=2^x$
* $f(x)=\cos(x)$
* $f(x)=\tan(x)$

---
<!--_backgroundColor: var(--ans)-->
# Answer

* $f(x)=2^x$
* The only answer with this property, since $f(a+b)=2^{a+b}=2^a2^b=f(a)f(b)$
* The point is that the property we see in the expression $\zid{\theta}$ where squaring it is the same as replacing $\theta$ with $2\theta$ suggests that it might be related to exponential functions like $2^x$ somehow. 

