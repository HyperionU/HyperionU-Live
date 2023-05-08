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

# 1. The Simpler Quadratic Formula

---

## Mental Math Tricks

* In some cases, finding prime factors of numbers is easy.
* For example: What are the prime factors of $35$?
    * $5\ \&\ 7$ right? Let's try something more challenging.
* What is $143$'s prime factors?

---

## Mental Math Tricks, cont.

* What is $143$'s prime factors?

Probably the first thing that's in your mind is to iterate over all of the factors. But there's a quicker way.

---
<!--_backgroundColor: var(--que)-->
## Finding 143's Factors

1. First, Which of these is true?

* $143$ is prime.
* $143$ has $2$ prime factors.
* $143$ has $3$ prime factors.
* $143$ has $>3$ prime factors.

---
<!--_backgroundColor: var(--ans)-->
# Answer:
* $143$ has $2$ prime factors: $11\times13$.
* Note: both factors are $1$ above and below 12, and $143=12^2-1=144-1$. *Why is this notable?*

---
<!--_backgroundColor: var(--que)-->
## Challenge
* Let's try a more challenging one.
* What is $3\ 599$'s prime factors?

2. Which of these is true?
* $3599$ is prime.
* $3599$ has $2$ prime factors.
* $3599$ has $3$ prime factors.
* $3599$ has $>3$ prime factors.

---
<!--_backgroundColor: var(--ans)-->
# Answer:
* $3599$ has $2$ prime factors: $59\times61$.
* This would take a long time to factor by hand, but there's a trick: 
    * Any number 1 less than a perfect square will always have factors $(n+1)(n-1)=n^2-1$.

---

## Factoring: Difference of Squares

* Most numbers in some cases will always factor.
* For example: 35, 3599 & 143.
    * *What do these have in common?*
    * They are all equal to $n-1$, where $n$ is a perfect square.
    * These factor as Differences of Squares.

---
<!--_backgroundColor: var(--que)-->
## Challenge:

3. Expand $(m+d)(m-d)$

* $m^2+d^2$
* $m^2+2md+d^2$
* $m^2-d^2$
* $m^2-2md-d^2$

---
<!--_backgroundColor: var(--ans)-->
# Answer:

* $m^2-d^2=(m+d)(m-d)=m^2+md-md-d^2$
* This emphasises that mulitplying two numbers is the same as a difference of squares.
* For any two numbers $a,b\in\mathbb{R}$, there will be a midpoint $m$ equidistant to $a\ \&\ b$, such that the product $ab=m^2-d^2$.
* This may appear a hack, but it works.

---
