---
layout:     post
title:      "interlude - thoughts about 41's design process"
subtitle:   "reflections at week 3"
date:       2026-1-29 12:00:00
author:     "jasonzeng124"
header-img: "img/post-bg-2015.jpg"
catalog: true
mathjax: true
alter: 1
tags:
    - Robotics
---

So I've been thinking a bit about the design recently.

Yes, I did approve it. And I do think it will work.

But it certainly wasn't my intention to go with something like this at the start, and honestly I would probably prefer something else.

-----

I should preface the discussion by saying, that we did a lot more prototyping this year than in all of 2023-2025, combined. Which honestly is pretty good. Of course, there are problems with our prototyping process (which do need to be addressed), but it is better than no prototyping at all.

In week 1 really was the time for the most rough prototypes. Like the stuff with drills spinning it. Here I was the one who really took charge and got our rough roller intake and our shooter prototype up.

In weeks 2 and 3 the attention was turned more-or-less to our indexer prototypes. Actually the shooter prototype has not changed largely since I built it in the first place. And the intake prototype we've just been refining some of the details, but no major changes either.

Here I was more involved in trying to get the CAD jump-started. Although it appears that my efforts here have failed (it appears to be largely because we didn't have a concrete robot design, especially with a decision on the indexer.). But I stopped doing hands-on work with the prototypes, and KL wasn't here either for week 2. So the prototyping efforts did stall out.

In fact in weeks 2 and 3 the summation of our prototypes is just a spindexer, and a failed hopper intake (so 118-style) prototype. In particular, the failure was due more so to the skill issue of the prototypers rather than the indexer being hard. Although it probably was indicative of the 118-belt-indexer being somewhat harder, than, say a spindexer, they also had like a week to do it.

Anyway by the time we were pressed for time to make a decision the only indexer we really prototyped was a spindexer.

-----

On day 1, AG had already had a strategy and a design in mind. The idea was a standard, high-volume hopper with an adjustable-hood turret shooter.

It should be noted that here right at this point there is already a ton of powercreep. And even though this is like a Ri3d design, it is quite nontrivial to build already.

In any case most of the team was settled on a turreted shooter from the outset. At the very least, AG AP and KC (+ alumni TB OG and mentors P, S) were definitely for it. I was like neutral, leaning for it. Against it was RM, LYT, and Mr. H.

Perhaps in retrospect it was less definitive than I thought it was. Perhaps it was possible for 41 not to do turret. But back then I did perhaps think that fighting against turret would be fighting against the flow of the water. And part of me wanted to do it too.

I also did not realize how much design complexity turret would add. Everyone I consulted with told me that turret was rather simple. And indeed it was a simple mechanism, at least the turret part of it is. But the complexity is involved with having to design a good portion of the robot and especially the shooter around the turret. And the shooter is critical-path here.

In any case I believed AG that the turret was "easy" to add on and that it'd just be minimal additional time. And I let him work on a turreted shooter, although I was not entirely sure about turret. I don't think it was until perhaps middle-end of week 2 that I realized how much more complex turret makes everything.

By that time AG was promising me every day that the shooter would be done tomorrow. For like until now. And to be honest, I think the shooter has been a few hours away from done on CAD for the entire week now, or at least that is my impression. So I believed him. Well now it is actually done (well being assembled right now), so it's a bit late to switch away from turret...

-----

For intake, it appears that RM has been working on it more-or-less the entire time (well also the hopper). Intake has primarily been slower here, I think, because there really isn't an idea of what the rest of the robot will look like. So it doesn't make sense to mount the intake anywhere at all. And it's not clear how high the intake needs to bring the balls or how much guidance the balls need or where they need to go.

For indexer RS did CAD something that looks like a spindexer, but on the crayola to technical pen scale, it was like marker. Not that it could have been significantly better without a shooter CAD. The hard part is not the spindexer, but really its interaction with the elevator.

In any case we did not really have a real decision on the indexer for a while. At the beginning we wanted to just do rollers that converge (with mecanums) to a single shooter in the center. Later we started alternate designs such as the spindexer and the 118 belt roller. But neither were cadded to any significant degree and so the only progress we had on any of these was the prototyping. And the easiest one to prototype was spindexer, which was the only prototype that our team got to work.

Around Monday on week 3 it became clear that we needed to set on a design. And thus the natural outcome happened.

-----

Aside from more / better prototyping, what else should we have done? We definitely could have done better...

I think deferring the final decision on the indexer was the correct decision. At the very least a serious prototype attempt at each idea should have been attempted, which would more-or-less have taken the first two weeks.

I think one thing we could have done, at the minimum, was to do more rough crayola cadding, just to get an idea of how everything will fit on the robot. This can be done for each idea reasonably fast, and it'll give a good idea of what it'll look like. We did do this, but only after we decided on our robot design. It should have been done sooner.

Also in general we need to do more crayola cadding, and slowly increase the level of detail (LoD) on our CAD. This will make stuff like CADing mounts easier, especially in places where mechanisms will interact or be mounted together. This might be a bit harder in Inventor than other CAD software, perhaps switching softwares is worth thinking about.

-----

Next year will likely be pick-and-place rather than a shooter game. Which does demand some different considerations, and I'll briefly discuss this too.

Pick and place games are different, in that generally they:

- require more DOF
- are harder to drive
- are harder to control
- are harder to build
- need more programming time
- are much harder to prototype
- geometry of mechanisms matters more
- etc.

One way to avoid this is to design simpler. For example, 1923's cube shooter in 2023, or the fast cycling kitbot clones in 2025. And this is probably the easiest and best way to avoid these issues.

But if you must face a pick-and-place game head-on with a full robot design, it is a bit more challenging. More things are going to be only in CAD, and you just have to trust that they work when you build it. The only real thing to prototype is the intake (and this better be prototyped *very well* or there will be issues). A full design should be decided on much earlier, and more time needs to be allocated to CAD and building as well. And you really only get one shot (you really can't rebuild everything).

Although maybe making things modular and using more stuff like punch tubing will help. This restricts your robot to be simple (which is probably a good thing). But they also tend to be more jank and don't work entirely as well. You can prototype with this, although it won't be 1:1 like prototyping this year has been.

-----

Compared to, say, VEX or FTC, FRC has always seemed fast-paced. I used to be on a VIQC team back in middle school so I do have some perspective on this. But now that I think about it, FRC is a lot of time. 

Say, if you compute the time, it comes out to be around 300 hours for all of them. And on FRC you have a team that is almost 2x the size, sometimes. If you're efficient you can get plenty of prototyping and iteration. And although the time between competitions is shorter, it forces you to design for repairability and modularity.

It's definitely a bit more fast-paced, but if you use time and resources efficiently, it's very managable. And even if you don't, you'll still find that you have a lot of time. Especially if you're like our team and meet for 6 hours every day.