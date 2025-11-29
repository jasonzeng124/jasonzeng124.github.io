---
layout:     post
title:      "Afterthoughts on Pinely Round and Teamscode"
subtitle:   "waymo orzorzorzorzorzorzorzorzorzorzorzorzorzorzorzorzorzorzorzorzorzorz"
date:       2024-07-29
author:     "jasonzeng124"
header-img: "img/bg_images/bg-teamscode.jpg"
catalog: true
mathjax: true
alter: 0
tags:
    - Competitive Programming
    - Codeforces
    - Problemsetting
---

Did a lot of competitive programming yesterday :D.

[Pinely Round 4 (Division 1+2)](https://codeforces.com/contest/1991) was yesterday (spoiler: I did bad). As usual, ABC were easy problems. Then came D.

![Clarification answer: least stupid constructive](/img/content_images/2024_7_29_constructive.png)

The statement:

> You are given a graph of $n$ nodes labeled $1\dots n$. Two nodes $u, v$ are connected if and only if $u \oplus v$ is a prime number. Output any optimal coloring of the graph.

:kms:

Well, it was a funny problem, even if I really dislike it. D tanked my performance, as I worked on it from 00:27 to 01:56 D:. First off, the samples are made for guessing (they had a very obvious pattern), but of course it was not right. Since I was getting suspicious, I did not submit the answer given in the samples. After writing a brute force, I noticed that the answer was 4 for $n\ge 6$. Then, I tried guessing the answer based on the output of the brute force (did not go well).

After like 1.5 hours of struggling, I tried taking all nodes $\bmod 8$, which did not go well either, but motivated me to take it $\bmod 4$. At this point, I noticed that (1) they formed a clique, so of course they had to be different, and (2) any edges going from one group of 4 to another group of 4 did not affect the coloring.

Then, the answer is either the sample output, or $1, 2, 3, 4, 1, 2, 3, 4, 1, 2, 3, 4, \dots$

The result: expert perf on div 1+2, and I am no longer a master D:

A short note, I guessed the solution for problem E, then couldn't prove that Bob could win... because I forgot to use the main condition of bipartiteness - that it could be split into two groups with no edges in between them...

And also, I was pretty close to getting F, but I wasted time implementing a obviously wrong solution (using mo's noooooo).

OK, that's how I'm back to being CM on cf... Hopefully not for long.

---

Shortly after the CF round, Teamscode started. Nothing went terribly wrong, except that the test data for P!=NP was wrong, and also Thomas had an untested model solution for Flappy Deer.

My problem, Waymo orzorzorz, was actually easier than Rinbot and Stage 4, even though I was sure that it was harder. Well, it was hard enough to be an AK killer for the novice division :). It's also funny how cerealcodes had set the exact same problem (well, their fault that they were procrastinating their contest...).

Anyway, the model solution to Waymo orzorzorz (not the original model, because Yam orz found a better model):

First observe that you always type $x$ single orz's, and then copy-paste to multiply $x$ by $y$ such that $xy \ge N$. Consider fixing the number of Copy and Paste events: Clearly, a copy should be accompanied by a paste, so there should be at most $log_2 N$ copies. Then, given that you have $c$ copies, you have at most $c N^{1/c}$ pastes (you do a series of a copy, then $N^{1/c}$ pastes, then repeat).

Then, the solution is as follows: Fix $c$. If $c\ge 2$, you simply run iterate over the # of pastes. If $c=1$, then $x=\left\lceil{\frac{N}{y}}\right\rceil$, and it is well known that there are $\mathcal{O}(\sqrt N)$ distinct $x$'s, so you can brute force. And the $c=0$ case is trivial.

The complexity is dominated by the small $c$ terms, and the larger $c$ terms run in $\mathcal{O}(\log N)$, so the solution runs in $\mathcal{O}(\sqrt N + \log^2 N)$.

Well, now that the 2024 season of Teamscode contests is over, it was really fun to actually set problems. This contest actually reminds me of my first teamscode contest (the first problem was P=NP!). It's been a long journey since then. Also, Waymo and a few other problemsetters are graduating this year. We will certainly miss them (and their problems). It was fun...

