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

# <!--fit--> Hyperion University Lectures

<span class="darken">By</span> Gen L.

<!--_footer: Provided by Hyperion University, © 2023--> 

---
<!--paginate: true-->

# 4. Euler's Formula

---
<!--_backgroundColor: var(--que)-->
## Poll

1. What best describes your relationship with the formula $e^{i\theta}=\cos\theta+i\sin\theta$?

* I had never seen it before.
* I've seen it, but I'm confused about it.
* I still don't understand it, but have grown used to it.
* I completely understand it.

---

## What is $e^x$?

* $e^x$ is, commonly shorthand for another function, $\exp(x)$.
* This $\exp(x):=1+x+\frac{x^2}{2}+\frac{x^3}{6}+\cdots+\frac{x^n}{n!}$.
* This is very different to how exponents work in general.

---

## Exploring $\exp(x)$

* What are some properties of this function?
* Take $\exp(1)$, which is equal to thus:
$\exp(1)=1+1+\frac{1}{2}+\frac{1}{6}+\cdots+\frac{1}{n!}+\cdots$
    * Eventually, this series converges to $\exp(1)=2.71828...$.
* Or, take $\exp(2)=7.38905...$
* Of note is that $\exp(a+b)=\exp(a)\times\exp(b)$

---
<!--_backgroundColor: var(--que)-->

## Properties

2. Let $f(x)$ be a function that $f(x)=y\in\mathbb{R}^+>0$. 
If $f(x)$ has the property that $f(a+b)=f(a)f(b)$, which of the following is true?
a. $f(5)=f(1)^5$
b. $f(\frac{1}{2})=\sqrt{f(1)}$
c. $f(-1)=\frac{1}{f(1)}$

---
<!--_backgroundColor: var(--ans)-->
# Answer

* A, B & C

* To prove A: $f(5)=f(5(1))=f(1)f(1)f(1)f(1)f(1)=f(1)^5$
* To prove B: $f(1)=f(\frac{1}{2}+\frac{1}{2})=f(\frac{1}{2})^2$. Since $f(x)$ outputs $\mathbb{R}^+,\ \therefore{f(\frac{1}{2})=\sqrt{f(1)}}$.
* To prove C: $f(x)=f(x+0)=f(x)f(0)$. Dividing both sides by $f(x)$ gives $f(0)=1$. Since $f(0)=1$, $f(0)=f(-1+1)=f(-1)f(1)\implies{f(-1)=\frac{1}{f(1)}}$

---
<!--_backgroundColor: var(--que)-->
## Powers of $i$

3. Remember how $i$ was defined such that $i^2=-1$? What values of $i^n=-i$?

* $\{n|n\mod3=0\}$
* $\{n|n\mod3=0,n=+\}$
* $\{n|n\in\mathbb{Z}_4-1\}$
* $\{n|n\in\mathbb{Z}^+_4-1\}$

---
<!--_backgroundColor: var(--ans)-->
# Answer

* $\{n|n\in\mathbb{Z}_4-1\}$
* Here's the values of powers of $i$.
* $i^0=1,i^1=i,i^2=-1,i^3=-1,i^4=1$.
* Since $i^4=1$, this cycles with a period of 4, and every integer $n$ one less than a multiply of 4 gives $i^n=-i$.

---

# $e^{i\theta}$ and rotation

* $e^{i\theta}$, when extended to the complex plane rotates around the unit circle $\theta$ radians.
* This explains the periodic nature of the powers of $i$. 

[More Info Here](https://youtu.be/v0YEaeIClKY "e^iπ in π minutes")

---
<!--_backgroundColor: var(--que)-->
## Determining Values

4. Which of the following is closest to $e^{3i}$? *note: $3$ is in radians*

* $0.99+0.14i$
* $-0.99+0.14i$
* $0.14+0.99i$
* $-0.14+0.99i$

---
<!--_backgroundColor: var(--ans)-->
# Answer

![invert bg left](https://public.itempooluserdata.com/5o8sge7tMZe2buO7zz-4W-398.webp)

* $-0.99+0.14i$
* $e^{i\theta}$ describes a point on the unit circle by walking a distance $\theta$.
* $3$ radians is barely less than $\pi$ radians, so the real part should be very close to $-1$.

