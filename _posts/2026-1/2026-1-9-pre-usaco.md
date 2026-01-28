---
layout:     post
title:      "USACO is tomorrow"
subtitle:   "it might be over"
date:       2026-1-9 19:00:00
author:     "jasonzeng124"
header-img: "img/post-bg-2015.jpg"
catalog: true
mathjax: true
alter: 0
tags:
    - Competitive Programming
---

USACO is tomorrow. I am not prepared at all. I'm like, really washed. Probably worse than I was last year, which was already pretty bad.

My goal is camp. Surely, that is possible with a bit of luck...

-----

I haven't really grinded CP seriously for like almost a year now. So I'm expecting to be really washed. Especially with implementation speed (I haven't implemented anything in a long while...).

USACO adopted a new-ish format this year. 3 regular online monthlies, 1 proctored open (presumably in-person). All non-finalist plats demoted to gold. But none of this really affects me.

Cheating might be really bad. Like, really really bad. But what can I do, but to try my hardest, anyway? So no point in thinking about all of this.

As aqxa once said to me (i don't really remember... but the meaning is roughly there iirc):

> before the contest, you study as much as you can. but during the contest, all you can do is to try your best, and don't think or care about what result you get. and whatever you get is just the result of how much you practiced

If I don't camp it's just a skill issue i guess.

-----

So, I'm not implementing anything today. But I will write editorials for some of my mindsolves. Or really I read the edi, but I should understand it.

**IOI 2025, day 1, problem 2. Triple Peaks. Part 1.**

So you basically count $i$, $j$, $k$ such that $h_i=k-j$, $h_j=k-i$, and $h_k=j-i$.

After some rearranging you get:

$ h_i-i=h_j-j $

$ h_j+j=h_k+k $

$ h_k-k=h_i+i $

From this, you can create a graph of $(h_i-i, h_i+i)$, and you count the number of triangles in the graph. This is easy on $O(n\sqrt n)$.

Alternatively, fix a value of $h_i-i$. Lets say $m$ indices have $h_x-x=h_i-i$, then solving in $O(m^2)$ is trivial. Otherwise, suppose there is a triangle $i$, $j$, $k$. Fix $k$, then we have $h_j+j=h_k+k$ so we know $h_j+j$ and $h_j-j$ and we can find $j$. And similarly $i$. So we can fix $k$ from $0$ to $n-1$ to solve in $O(n)$. We can do the $O(n)$ for $m>\sqrt n$ and $O(m^2)$ otherwise, for a total of $O(n \sqrt n)$ again.

-----

**IOI 2025, day 1, problem 3. World Map.**

First, solve tree case. $2n-1$ is easy for tree case, just euler tour.

```
AAAAAAAAA
ABBBBBAEA
ABCBDBAEA
```

Notice that node width is like subtree size * 2 + 1, so its propto subtree size.

We need to add back edges somehow. (during virtual i was quite stupid and put them in the wrong direction :skull: honestly i should've actually written out the width/height but wtv).

For each node add two rows above, and put like `XAXBXCX` where X is node and ABC are the down-edges. This works for ratio $R=3$ as you have like $2n-1$ row and $3n$ columns.

```
AAAAAAAAA
A A A A A
AAAAAAAAA
ABBBBBAEA
AB B BAEA
ABBBBBAEA
ABCBDBAEA
ABCBDBAEA
ABCBDBAEA
```

For $R=2$ you try to squeeze stuff up. The trick is to do stuff on diagonals. A diagram makes this clear.

```
AAAAAAAAA
AA A A AA
ABABABAEA
ABB BBAEA
ABCBDBAEA
```

There are many details (like implementation) that I can't get right here. But, honestly, I don't care that much. The construction is enough to satisfy me.

Plus this is too geniousity for me anyway.

**CSP-S 2025, problem 4 Employ**

I was going to write edi for this.

But I don't understand solution, like at all.

skull emoji.

I'll write what I think is the solve for a subtask, hopefully it is right....

Consider fixing the sequence of AC / NO. Then, we can try to count... but that's really hard, because we have constraint $x_i\ge a$ if AC and $x_i < a$ if NO. Or something like that.

Consider removing the NOs, changing to X (don't care). Then we only have one type of constraint. And it's monotonically increasing or decreasing or something (ok its decreasing), so it's pretty easy to count.

For each bitmask we can calculate this value in like $O(n 2^n)$. And we can reverse SOS to get the final answer in $O(n 2^n)$.

At least I think this is right...

-----

Tomorrow I aim for 500+. Or maybe LB.

Idea is that I should perform like, around 1 solve in 1 hour, then spend like next 2 hours for second solve or nontrivial partial. Then spend last hour grabbing anything I can.

Perhaps I can do it, I don't know. I'll just have to hope for luck I guess.

Good luck to everyone else taking USACO!

I should go to sleep soon, I'll have a long day tomorrow.