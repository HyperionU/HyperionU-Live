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

$\newcommand{\mid}[1]{-\frac{#1}{2}}$
# <!--fit--> Hyperion University Lectures

<span class="darken">By</span> Gen L.

<!--_footer: Provided by Hyperion University, © 2023--> 
$\newcommand{\quad}[2]{#1\pm\sqrt{#1^2-#2}}$

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

## Quadratic Functions

* A function with a degree of 2.
* Often in the form $ax^2+bx+c$.
* Not helpful in this form, so we must reduce this function.

---

## Quadratic Reduction

* Reduces a function to have a leading coefficient of 1.
* Example: $ax^2+bx+c\rightarrow x^2+\frac{b}{a}x+\frac{c}{a}$
* To simplify, we rewrite the fractions as their reduced versions.
* Reduced example: $ax^2+bx+c\rightarrow x^2+b_rx+c_r$ or $x^2+b'x+c'$.

---
<!--_backgroundColor: var(--que)-->
## Challenge

4.  $let\ r,s$ be the roots of the function $f(x)=x^2+bx+c$. 
Which describes the relationship between the roots and coefficients?

* $b=r+s,c=rs$
* $b=rs,c=r+s$
* $b=-(r+s),c=rs$
* $b=rs,c=-(r+s)$

---
<!--_backgroundColor: var(--ans)-->
# Answer

$b=-(r+s),c=rs$
* $f(x)=(x-r)(x-s)$, which has roots $r,s$, since if $x=r,x=s$, you get zero.
* Once they are expanded, you get a quadratic with a leading coefficient of 1:
    * $f(x)=(x-r)(x-s)=x^2-(r+s)x+rs$
* Matching up the coefficients, we get $b=-(r+s),c=rs$.

---
<!--_backgroundColor: var(--que)-->
## Challenge

5. Now that we know that our midpoint $m=-\frac{b}{2}$, for any *reduced* quadratic $f(x)=x^2+bx+c$. 
What is the roots of $f(x)$?

* $m\pm\sqrt{m^2-c}$
* $m\pm\sqrt{m^2-4c}$
* $m\pm\sqrt{b^2-m}$
* $m\pm\sqrt{b^2-4m}$

---
<!--_backgroundColor: var(--ans)-->
# Answer

$m\pm\sqrt{m^2-c}$
* If we write our roots $r,s$ as $r=(m-d),s=(m+d)$, where $d$ is the distance their product is this:
    * $rs=(m-d)(m+d)=m^2-d^2$.
* Also, the product of the two roots must equal $c$.
* We can express the roots of $f(x)$ as thus:
* $m^2-d^2=c\implies d=m\pm\sqrt{m^2-c}$
$\therefore r,s=m\pm\sqrt{m^2-c}$

---

## Our Simpler Quadratic Formula: $r,s=m\pm\sqrt{m^2-c}$

---
<!--_backgroundColor: var(--que)-->
## Testing the formula

* Let's take the formula for a test drive with some quadratics.
6. Find the roots of $f(x)=x^2+10x+3$

* $5\pm4$
* $5\pm\sqrt{22}$
* $-5\pm4$
* $-5\pm\sqrt{22}$

---
<!--_backgroundColor: var(--ans)-->
# Answer

$-5\pm\sqrt{22}$
* The midpoint $m=\mid{r+s}=\mid{b}=\mid{10}=-5$. The product $rs=3$.
* Our answer then becomes $\quad{-5}{3}$
    * $-5\pm\sqrt{25-3}=-5\pm\sqrt{22}$
* With practice, this is something you can almost read off of the expression itself.

---
<!--_backgroundColor: var(--que)-->
## Level 2: Reduction

* Now, let's add on the step of reducing.
7. Find the roots of $f(x)=3x^2-4x+5$.

* $\frac{2}{3}\pm\sqrt{\frac{11}{9}}$
* $\frac{2}{3}\pm\sqrt{-\frac{11}{9}}$
* $2\pm\sqrt{-1}$
* $2\pm1$

---
<!--_backgroundColor: var(--ans)-->
# Answer

$\frac{2}{3}\pm\sqrt{-\frac{11}{9}}$
* After reducing the expression by 3 to get a leading coefficient of 1, we get: $f(x)=x^2-\frac{4}{3}x+\frac{5}{3}$.
* The midpoint $m=\frac{2}{3}$, and product $c=\frac{5}{3}$.
* Following the formula, we get: $\quad{(\frac{2}{3})}{\frac{5}{3}}$.
    * $r,s=\frac{2}{3}\pm\sqrt{\frac{4}{9}-\frac{15}{9}}=\frac{2}{3}\pm\sqrt{-\frac{11}{9}}$.

---
<!--_backgroundColor: var(--que)-->
## Challenge

8. Find the roots of $f(x)=2x^2-12x+20$.

* $6\pm2$
* $3\pm i$
* $6\pm2i$
* $3\pm1$

---
<!--_backgroundColor: var(--ans)-->
# Answer

$3\pm i$
* After reducing the expression by $2$ to make the leading coefficient $1$, we are looking for the roots of $f(x)=x^2-6x+10$.
* The roots $r,s=\quad{3}{10}=3\pm\sqrt{9-10}=3\pm i$

---
<!--_backgroundColor: var(--que)-->
## Deriving the Formula

9. For a quadratic $f(x)=ax^2+bx+c$, which of the following describes the roots of $f(x)$?

* $\quad{(-\frac{b}{2a})}{\frac{c}{a}}$
* $\quad{(-\frac{b}{2a})}{4ac}$
* $-\frac{b}{2}\pm\sqrt{\frac{(-\frac{b}{2a})^2-4ac}{2a}}$
* $-\frac{b}{2}\pm\sqrt{\frac{(-\frac{b}{2a})^2-c}{2a}}$

---
<!--_backgroundColor: var(--ans)-->
# Answer

$\quad{(-\frac{b}{2a})}{\frac{c}{a}}$
* Dividing by the leading coefficient, the roots of $f(x)$ are the same as the roots of $x^2+b_rx+c_r$, where $n_r=\frac{n}{a}$
* The midpoint $m=-\frac{1}{2}\frac{b}{a}=-\frac{b}{2a}$ and product $p=\frac{c}{a}$
* This expands as $\quad{(-\frac{b}{2a})}{\frac{c}{a}}$.

---
<!--backgroundColor: var(--que)-->
## Break Questions (not scored)

---

## Closing Question:

10. How often do you expect to use the Quadratic Formula (traditional or simplified) in "real life", outside of school?

* Never
* Rarely
* Sometimes
* Always

