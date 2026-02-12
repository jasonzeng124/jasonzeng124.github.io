---
layout:     post
title:      "reflections on robotics, part 4"
subtitle:   "how did this come to be?"
date:       2026-2-10 22:00:00
author:     "jasonzeng124"
header-img: "img/post-bg-2015.jpg"
catalog: true
mathjax: true
alter: 1
tags:
    - Robotics
---

> "do we really need five weeks to build our backup robot? if we're just going to copy some robot online?"

<p style="text-align:right;">&mdash;&mdash;&mdash; CET</p>

<p style="text-align:center;">* * *</p>

Is this not enough said? (it's not just CET with this mentality, I'm just quoting CET because it has been said just too perfectly)

-----

*blog written with some discussion with LXM incorporated*

We are well into week 5. And there is no sign of significant progress. Why?

Of course you can be somewhat simple-minded and blame it all on design. or mechanical. or whatever.

But there are deeper underlying issues at play here.

In this blog I want to take a look at some of the more fundamental cultural issues that are causing us to fail. consistently.

-----

I want to take a look at the team, as a single entity first.

What does the team want? Well, for one, to win.

But not just to win.

The team wants to win *in style*.

<p style="text-align:center;">* * *</p>

What does *winning in style* mean? For different people, it means different things. But for 41, my feel is that *style* looks like the following:

- The robot looks pretty.
- The design is ""original""
- We build most of it ourselves
- We have full CAD which the team fully follows
- We can score fancy stuff, like high climbs or L4 coral
- Robot is made out of metal. Not something wimpy like wood.
- etc etc etc.

-----

But sometimes we are too focused on the style part, that we forget that we have to win first.

So let's take a closer look at what individuals in the team want:

**Design:** Design team is here to design the robot. So it's natural that they want to design as much robot as they can. In particular, design will like robots with a lot of different functions, and they like to custom-build fancy stuff. What they don't really like is flat-out copying robot designs like everybot, or buying entire COTS subsystems, or free-building stuff, or simple strategies that don't really need a lot of designing.

**Mechanical**: Mechanical is really a "CAD-in, metal-out" machine, in my view. But even they want to do stuff. In particular, they want to build stuff, and they want to build fancy pretty parts with their fancy machines. The robot should Look Good TM. What they don't like is drilling holes (with hand drills), materials like wood, punch tube, buying subsystems, or other stuff like that.

**Electrical**: Electrical just wants electrical stuff to work. Electrical team's goals are very simple, just wire the robot. Which might be why we don't really have an electrical team, and it's just mechies who wire the robot occasionally. Which is Not Good because when something goes wrong nobody knows how to fix it.

**Programming**: Programming wants to write fancy features and fancy autos. The prerequisite, of course, is that the robot works. In general programming wants stuff that has a lot to program (more DOFS = more fun), and more time to program cool things and better autos. But on 41, the one thing we really want is time. No time = no time to program all your DOFS or write autos or even to get the robot tuned nicely.

Notice how very few people have "robot works" as a strong prerequisite for their robot to be stylistic.

In theory, there are supposed to be people who have a *big picture* in mind and keep that big picture in mind while doing things. In particular, a team captain who can override the individual biases about style and just worry about winning. In our team, there are like three such people. Me, AG, and KC. And probably, I'm more on the side of "win" and AG more on the side of feature creeping, and KC in the middle kind of.

And there's no real captain with authority to make big decisions which is kinda pain.

Anyway speaking of captaining i'm gonna go on a mini tangent. I think one of the most important things as captain is to dedicate time to captaining. Which means your captain really shouldn't be doing stuff like machining or designing or writing robot code, they really need a big picture of things. This applies to other roles like design/prog leads too. In particular LXM has complained about having to run CNC or do electrical stuff instead of designing. Or me having to write robot code instead of making sure that design is doing the right thing.

-----

Well, I've addressed one part of CET's golden quote. The robot part.

Now, I'll address the "5 weeks" part.

Our team likes to one-shot the 120 lb robot.

-----

Supposing that overall team strategy and workflow form a $n$-dimensional space, surely one-shotting the 120 lb robot is one of the more stupid things to do.

There are many things in this space. There are dimensions such as CAD fidelity, precision of build, how many prototypes / intermediate stage robots, how much time is left, etc. Some examples:

- free build the entire robot
- full cad the robot and build it
- free build prototypes and full cad robot
- free build prototype robot and full cad robot
- free build entire robot and iterate on robot
- sketch a 2d sketch and build robot
- etc etc etc.

And different teams use different strategies in this space. But 41's current strategy has been proven not to work for 3 years. And we haven't changed anything that could possibly make it work.

In particular I don't think our team understands the point of a) prototyping, making rough robots, and b) post-full-robot iteration. Both of these are really useful and can reduce your time by a lot. Oh and c) driver practice, of course.

Prototyping is something that gives you measurements you can just throw on CAD. Post-robot iteration means you can just CAD stuff and build it, and if it doesn't work, you just CAD something else. Instead of making a perfect-fidelity CAD the first time.

I don't think our team recognizes the fact that we can change our robot after we build it. Perhaps it is sort of a "we make no mistakes" type of thing, but I don't think that's the full story. It is a bit stylistic, of a "we cadded the full robot and built it and it just works", perhaps. There's not really room allocated to "oh no this doesn't work let's make a new version" and so we either bandaid it in some janky way, or we do it in between comps and it's too late.

We don't have to one-shot the 120 lb robot. And we shouldn't.

-----

One thing that we need a capable captain for is to know the ability of our team, and to choose a strategy based on the team's ability. We really don't have a captain, for one, and for another, I did a lot of overestimating our team's ability. Even after factoring in what I've seen from previous years. It's really hard to estimate the team's ability until build season comes, and by then it's way too late.

I also did propose trying to make an early protobot. In retrospect it would've been a good idea, definitely, but the other captains didn't like it.

-----

Some other things that should be talked about.

Our team really falls for sunk-cost fallacy a lot. Even very blatant instances of sunk-cost fallacy. When I was talking about bailout CET did mention "but we'd waste AG's work". I did tell him that it was sunk-cost fallacy but I don't think he understood. Our team definitely does not understand. This does do a good bit of impeding good decision-making, especially at critical points where a decision should be late. Even now I think sunk-cost fallacy is going to be the reason we don't go with an objectively-better backup robot (if it is indeed better).

There's also a sort of lack of responsiblity in the team. Most of the people on the team treat stuff as work, and don't take full responsiblity. As such some stuff just never gets done. Examples would include organizing the shop, or prototyping stuff, or designing something and making sure it fits.

But anyway I digress. This stuff is not as fundamental to our decision making.

What is fundamental is that our decision making. And for the past few years it's been too focused on style rather than winning. Together with resistance to change (already mentioned) and skill issues (also mentioned in part 3), this is what is holding our team back.