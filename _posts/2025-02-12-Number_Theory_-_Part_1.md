---
title: Introduction to Number Theory - Part 1
date: 2025-02-12 11:05:41 +0700
math: true
categories:
  - Math
  - Course
tags:
  - "#compsci"
  - "#math"
  - "#crypto"
  - "#course"
description: This is an introductory course to number theory and its application in computer science specifically cryptography.
---

## Welcome! 
Hey there, welcome to this post. This post is inspired by my discrete math/number theory class in university. I am by no means a math/number theory expert and this course is just an intro to it. This series is meant to help those who don't have any basics in number theory to gain some foundational knowledge. If you want to know more, feel free to google or ask an expert. This course will be split into 3-4 parts and this part is all about modulo. Lets start!

## Division theorem
>let `a` be a whole number and `d` be a positive whole number, then there exists a unique whole number `q` and `r` with $0\leq r<d$ such that $a=dq+r$
{: .prompt-info}

Lets see an example:

`a` = 10

`d` = 3

find q, and r

We can easily see that $10 = 3\times3 +1$ , so q is 3 and r is 1

>Remember that $0\leq r<d$ meaning that, for the above example, `q` = 2, `r` = 4 or `q` = 4, `r` = -2, although does make 10, is not a valid answer
{: .prompt-warning}

`d` is often called the 'divisor'
`q` is often called the 'quotient'
`r` is often called the 'remainder'

Let's practice:
1. Find the quotient and remainder for `a` = 20 and `d` = 3
2. Find the quotient and remainder for `a` = -20 and `d` = 3
3. Find the quotient and remainder for `a` = 10 and `d` = 5

>`r` is not allowed to be negative but `q` is allowed
{: .prompt-tip}


For a pair of `a` and `d` where the remainder is 0, such as practice
no. 3, we can say that `d` divides `a`, or in math notations, $d|a$. In 
other words, $d|a$ means that $a=d\times q$.

## Divisibility

Here are some theorems on divisibility


>1. if $a\vert b$ and $a\vert c$ then $a\vert (b+c)$  
>2. if $a\vert b$ then $a\vert bc$ for all integer c
>3. if $a\vert b$ and $b\vert c$ then $a\vert c$ .
{: .prompt-info}

Prove of theorem 1:

By the definition of divisibility, $b = a\times q, q\in \mathbb{Z}$ and $c = a \times k, k \in \mathbb{Z}$ 

$b+c=a\times q+a\times k$

$b+c=a(q+k)$

since $q,k \in \mathbb{Z}, (q+k)\in \mathbb{Z}$. 

Meaning that we could rewrite as $b+c = a*j, j\in \mathbb{Z}$. 

Hence, $a\vert(b+c)$.

Prove of theorem 2 and 3 are left as an exercise to the reader. You could prove it with similar method.


## Modulo
Recall the division theorem, $a=dq+r$ . When we calculate a mod d, we are calculating `r`. 

For example, what is 3 mod 5? 

$3 = 0\times 5 +3$, meaning that 3 mod 5 equals 3. 

So what are the applications of modulo? A really common example used to demonstrate the applications of modulo is something i like to call the "what day is it " problem. Here is how it goes.

The first day is Monday. What day is the 123rd day?

We can solve this using modulo. We know that 1 week has 7 days, so we'll use that fact to solve the question. First we calculate $(123-1)$ mod 7. We subtract by 1 because Monday is the first day, if Monday is the, let's say 23rd day, then we subtract by 23. 

$122$ mod 7 = 3, and 3 days after Monday is Thursday, meaning that the 123rd day is in Thursday!


## Thank you
Alright that marks the end of this post. Remember, you have to practice often to get good and quick with any number theory topics. Don't get discouraged if you find it difficult and keep on practicing. See you on part 2, where I'll discuss modular exponentiation, greatest common divisor, and lowest common multiple! Stay safe and have a nice day 😊

