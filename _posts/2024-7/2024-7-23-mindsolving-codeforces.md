---
layout:     post
title:      "Mindsolving CF 961 (Div 2)"
subtitle:   "tunnel vision + clownery"
date:       2024-07-23
author:     "jasonzeng124"
header-img: "img/post-bg-2015.jpg"
catalog: true
mathjax: true
alter: 0
tags:
    - Competitive Programming
    - Codeforces
---

**First and foremost: *Do teamscode*! There are some great problems! Link to announcement: [Teamscode Codeforces Announcement](https://codeforces.com/blog/entry/131526)**

Codeforces Round 961 (Div 2) happened today. I didn't participate (due to being lazy and div2's are unrated for me), so I just mindsolved...

Looking at the standings, it seems like everyone solved ABCD.

A was a pretty standard greedy problem, as usual (the solution idea is to fill largest diagonals first). B1 was pretty easy as usual, just fix min # of petals and do some math. B2 was the same idea.

C seems like an easy problem, but of course, the numbers don't fit in `long long`...
Since I read this problem last, I didn't think hard enough (D:). Turns out the clever solve is to square it to become greater than the previous number, then square it the number of times the previous number was squared. (definitely would not have thought about that during contest? idk) Also turns out that long double with keeping track of 2 logs passes :thinkies:...

D was a funny problem, because initially I saw $C\le 18$ and immediately assumed that it was bitmask dp, haha. Well, turns out it is a bitmask DP approach that _HaccerKat_ explained to me afterward. My approach in contest (after bricking for 30 minutes about bitmask DP) was to consider all pairs of characters and compute the answer with `max(s) = min(max(dist between a,b) where a,b in s)`. Of course, this dies on the most trivial test case of `ABC.........D` :skull:

The correct way to solve, of course, is to notice something geniosity: if you have a mask that is good, then consider the complement of the mask (let's call it `s`); then the largest subarray of elements in `s` is $\lt k$. Conversely, a mask is bad if and only if the complement has a subarray of elements of length $\ge k$. Then, you can iterate over all subarrays of length $k$ and mark the complement masks as bad. Then, if a mask is bad, all of its subsets must be bad, so you can use SOS dp, and then find the smallest non-bad mask. Personally, I don't think I would have ever thought of this...... Perhaps a data structures bash mindset is not optimal.

E1 was a fun problem, it took me some time to think about, but the solution idea is cool. Of course, my solution wasn't completely correct either.

After playing with the even $n$ case, I came up with the basic idea of fixing the smallest $a_{2i} + a_{2i-1}$, then minimizing the maximum value. It's not hard to see that there are $\approx 4n$ of these values. Then, you split into even and odd $n$. For even $n$, it's not hard to brute force. For odd $n$, the structure is linear once you unwrap the circle (i.e. instead of swapping $i$ and $i+n$, you can unwrap it so that $2i$ and $2i+1$ are swapped). Then, you can run a dp over whether the previous pair was swapped. (I thought a greedy would work, until some orz people convinced me otherwise)

It seems like the idea generalizes to E2 with dynamic DP + segtree, I'm not so sure yet... In any case, it would be cancer to implement... (actually, _tourist_'s solution is pretty clean, and uses this idea).

In any case, this was a pretty cool contest (even though I might've only solved AB if I actually took it). In hindsight, I really should have done my due diligence in *actually* making sure that my solutions work, not just assuming that they do because it feels like it. In the future, I should do more implementation (not just mindsolving), and I should also diversify my problem sources.

Well, if anyone is actually reading this (I know, it was a long blog and you are tired), *please do teamscode*! There are some great problems! Link to announcement: [Teamscode Codeforces Announcement](https://codeforces.com/blog/entry/131526)
