---
layout:     post
title:      "Bomb and Penacony"
subtitle:   "arknights >>> hsr"
date:       2024-07-24
author:     "jasonzeng124"
header-img: "img/post-bg-2015.jpg"
catalog: true
mathjax: true
alter: 0
tags:
    - Competitive Programming
    - Codeforces
---

Today I did some knzhou E1 (also yesterday) (and played more arknights than I should). I also had time to mindsolve some codeforces problems from the best problemsetter _envy_ (also _sum_).

I mind solved FG:


The [statement](https://codeforces.com/contest/1996/problem/F) of F:

> Sparkle gives you two arrays $a$ and $b$, each of length $n$. Initially, your score is $0$. In one operation, you can choose an integer $i$ and add $a_i$ to your score. Then, you must update $a_i$ as follows: $a_i \leftarrow \max(0, a_i - b_i)$
>
> You have time to perform at most $k$ operations before Sparkle sets off a nuclear bomb! What is the maximum score you can acquire after $k$ operations?

The obvious greedy is to always take the largest element. Of course, this is optimal (doing an operation only gives you smaller array elements to do operations with, more on this later). Then, you will notice you do operations until $\max(a) \le x$, and you can binary search on this $x$.

To prove optimality, note that each element's operation sequence will yield a reward function that is convex, and more specifically linear. Then, the optimal rewards of the array will be the minkowski sum of these functions, which is also convex. This leads to an interpretation of the binary search as an application of Aliens' trick or wqs binary search. (Now I can say that aliens trick has appeared on div3 :D thx _gmbl_ for the tip)


The [statement](https://codeforces.com/contest/1996/problem/G) of G:
> You are given a cyclic undirected graph ($1 \rightarrow 2 \rightarrow 3 \rightarrow 4 \dots \rightarrow n \rightarrow 1$). You are given pairs of vertices $(a, b)$ such that they must remain connected. How many vertices can you remove?

As a data structures main, the first solution I thought of was as follows:

Observe that you can always remove an edge. If you remove an edge, it will force the configuration of the houses. By iterating the edge you remove from left to right, you can use a (range add, count min) segtree to sweep.

Of course, there is a more elegant solution (_4dalols_ orzorzorzorzorzorzorzorz):

Consider a n-gon, the constraints are of the form: you choose one side of the diagonal and paint all the edges. The answer is the # of unpainted edges.

![diagram](/img/content_images/2024_7_26_div3G_diagram.svg)

Arbitrarily choose a side, and paint the edges, each diagonal with its own color. Then, for each set of colors that are painted, there exists a (possibly empty) set of edges that correspond to a possible set of edges that you can remove. Of course, you can remove them, just flip the direction of the diagonals corresponding to the color set.

Then, it suffices to xor-hash with 64-bit numbers, and find the maximum count.

It's kinda funny how math mains always word their solutions with really mathy jargon (all my friends hate geometry too). This one is really clean once you understand it, however :D.

Also maybe it's time to learn xor hashing :P (I never know when to use it).

p.s. Speaking of problemsetting, you can expect the next blog to be about teamscode! Also do teamscode if you aren't already.
