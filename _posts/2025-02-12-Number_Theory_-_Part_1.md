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
Hey there, welcome to this post. This post is inspired by my math discrete math/number theory class in university. I am by no means a math/number theory expert and this course is just an intro to it. This series is meant to help those who don't have any basics in number theory to gain some foundational knowledge. If you want to know more, feel free to google or ask an expert. This course will be split into 3-4 parts and this part is all about modulo. Lets start!

### Division theorem
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

### Divisibility
if $d|a$ , then `d` is a factor of `a` and `a` is a multiple of `d` 


Here are some theorems for divisibility:

- if a|b and a|c then a|(b+c)
- if a|b then a|bc for all integer c
- if a|b and b|c then a|c

