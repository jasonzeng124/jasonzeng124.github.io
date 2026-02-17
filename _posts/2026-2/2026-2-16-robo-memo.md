---
layout:     post
title:      "technical memo on robotics strategy"
subtitle:   "\"how many of you would want a 120 ball box on your alliance\", seriously"
date:       2026-2-16 21:01:00
author:     "jasonzeng124"
header-img: "img/post-bg-2015.jpg"
catalog: true
mathjax: true
alter: 0
tags:
    - Robotics
---

> It seems pretty hard for our team to get any sort of advantage here. Maybe the best thing to do is to stick to the meta, and to execute well? But I don't trust that to happen, at all. But the alternatives aren't much better...
>
> -- me, after kickoff

LYT has been pushing me to do a little thinking on what the frc game actually entails.

I hate thinking but I guess I should do some thinking sometimes.

-----

So let's lay out some Pareto-optimal strategies, and take a look.

Before that, however, some assumptions:

- You can get around 2 balls / second with 4 well-trained human players. This is not a joke, seriously. In particular, raw BPS is like 2.5 per second and accounting for accuracy it is 2/s
- On average, you will intake maybe 1-5 balls per second, depending on how efficient your driving and intake are. Let's just say 2
- Shooting will be around 6-10 balls per second, and robots can store around 50-80 balls
- Cycling during the active period will be hard due to defense
- Cycling during the inactive period will be easy and you'll be able to defend (ie take balls away)
- Traditional hit-while-shooting defense won't be effective enough versus just cycling

And let's look at some strategies:
- turret
- multiple shooters, note that the shooting speed is only like 50% faster at max
- big box, you can store around maybe 100 balls? Maybe like 120 if you go over bump?

LYT claims that big box is at least break-even with the previous two strategies.

-----

The cycle goes around like:

- AUTO 20s
- free shoot 10s
- alternating shift periods x4 25s
- endgame 30s

So 160s total. 110s with legal shooting.

-----

Lets look at a multiple-shooter robot first. Say it is higher end of speed, so 10 balls per second, and lower end of storage, so 50 balls.

During auto and free shoot you'd be pretty good with 50 balls.

During the active periods it will be able to shoot its entire hopper in like 5 seconds. Then you have like 15s to get balls. With heavy defense during the active period the average ball intake rate might be like 2/s? So you get like 80 balls total.

During the inactive period it would probably be possible to load a full hopper at like 3 bps.

-----

Turret is mostly similar, perhaps. Probably a bit slower, and similar storage (although a well-built turret will have a bit more). So like 8 bps and 50 balls.

Roughly the advantage of turret is intaking while shooting. Assuming you can do this without many losses, you might get like 50 + 25 * 2 = 100 or so balls in the active period?

-----

Now for the big box.

During auto, the idea is to load up 100 balls and feed it into the humans. If there's no other shooter bot on your team that's all you do.

During the active periods you unload into a fast shooter. Roughly the calculations go:

150 balls total, 10bps means 15 seconds to empty, and you get like 150 points with 10s to go. The 10s can be taken to gather more balls. And this almost matches the efficiency of two shooter bots.

Endgame really depends on climb type, so this might be significantly less efficient in endgame though. But it definitely is very doable.

-----

I hate to admit this, but it's definitely a very viable strategy (hey i thought of it like day 1). And if storage sizes on shooter bots are less, this strategy becomes increasingly viable. And this gives you more time to spend optimizing driving, and also intake and hopper size.

Some funny ideas: make your hopper out of metal plate, and have like 4-in-diameter holes in them so the balls can protrude out of the walls. Maybe on the ceiling too...

41 probably won't do this, because it looks absurd. And they won't like it. But it's definitely doable.

