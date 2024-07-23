---
layout:     post
title:      "Solution notes for codechef round"
subtitle:   "mindsolving again, i guess"
date:       2024-07-31
author:     "jasonzeng124"
header-img: "img/post-bg-2015.jpg"
catalog: true
mathjax: true
alter: 0
tags:
    - Competitive Programming
    - Codechef
---

Mindsolved Starters 145 (was going to implement but I got lazy after mindsolving...)

Only got ABC, kinda disappointing ngl

A: notice that a 2 1's on boundary makes Bob win (looked at patterns too late :[), can be proved with induction (probably).

B: iterate over # of initial 0's, then you can do some math with genfuncs (at least acc to oeis lol).
(editorial uses some clever contribution solution that I didn't think of ... idea is to fix the difference then count)

C: Look at the highest 1 bit in X, try to make that bit in the AND be 1. If you can, great, see if any other bits match that bit, otherwise, go to the next bit and try again.

Wow, looks like it took me like 1.5 hours to mindsolve 3 problems :skull:

Oh I guess I also solved D (totally not writing this blog in the middle of the contest):

D: ~~template small to large~~ for each value, add its divisors, and do small-to-large. At each node, after merging, just query divisors. Probably best to segtree merge.

Maybe I should have gotten E, didn't think hard enough (edi solution is not that bad). And F is more like a MO problem...

Well, solving 4 theoretically places me between 19th and 50th, which is not bad (for codechef).

