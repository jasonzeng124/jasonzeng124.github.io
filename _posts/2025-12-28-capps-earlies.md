---
layout:     post
title:      "how my college predictions went"
subtitle:   "tl;dr not very informative?"
date:       2025-12-28 23:00:00
author:     "jasonzeng124"
header-img: "img/post-bg-2015.jpg"
catalog: true
mathjax: true
alter: 1
tags:
    - College
---

I tried predicting the odds of my classmates' chances at college. Well, the earlies are over, and honestly looking at the earlies is enough to draw some conclusions, and I don't think I'll continue this (its not that interesting).

My average surprise (or cross-entropy loss, basically $-\log p$ where $p$ denotes the probability that I assigned to the outcome) was 1.11. This is higher than a bit, so its basically useless. I would've done better assigning all my classmates 50%s and just watching coins flip.

The base rate in my data was like 43%, so a flat predictor wouldn't do better than me. And acceptance rate would do worse than me too.

I do think I did not predict as well as I could have, some mistakes being:

1. I'm used to CS rates. if everyone here applied CS I might be more accurate, but, well, not everyone is CS.
2. My anchor in general was base acceptance rate. Perhaps I should've used data from our school, then adjusted it instead. In general if you take the expected value by sum of my probabilities, it'd be a bit low, I should've adjusted for this too.
3. I don't know that much about my classmates. Or I did but didn't really take it into consideration.
4. I thought I could do much better than 1 bit, maybe like 0.7 or something. Turns out I'm really wrong here. It's more RNG than I thought.

well, further proof that college apps is just rng. who would've thought?

psa. rng = random number generator. for those (nonempty set) who didn't know