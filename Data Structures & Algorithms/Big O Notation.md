---
title: Big O Notation
created: 2024-09-10 05:15
tags:
  - programming
  - dsa
cssclasses:
  - img-rounded
  - img-centered
---
Example 1:
![[big-o-example-slower.png]]

Example 2:
![[big-o-example-faster.png]]

Both of these functions will produce the same output.  Most people will assume that good code = efficient code.  Efficiency of the code usually relies on some key points:
- Faster?
- Less Memory-Intensive?
- More Readability


Example outputs:
![[big-o-example-result.png]]
*Example 1 is on top, example 2 is on the bottom.*

While the time difference is drastic here, what happens when the algorithm we utilize is extremely fast, and maybe too fast to compare with other algorithms?

**Different** machines will record different times.  The **same** machines will **also** record different times.  While it is important to take speed into account, a more stable way to quantify its efficiency is to **count the number of simple operations** our computer has to perform to reach the algorithm's conclusion.

In example 2:  (n <b>*</b> (n **+** 1)) **/** 2
- there are 3 operations taking place:
	- <b>*</b>, **+**, **/**
	- These three operations only happen once.

In example 1:
- we have a **+** operation and an **=** assignment in a **for loop**.  We also have one assignment for **total** and **i**'s initial assignment and **<=** comparisons
- Depending on how we count, the # of operations can be as low as **2n** or as high as **5n + 2**.

Regardless of the exact number, the number of operations grows roughly proportional w/ n.

![[big-o-explanation.png]]


![[big-o-explanation2.png]]

![[big-o-explanation3.png]]

