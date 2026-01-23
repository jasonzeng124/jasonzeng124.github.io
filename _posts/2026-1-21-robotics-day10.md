---
layout:     post
title:      "robotics, day 10"
subtitle:   "slowly might be an understatement"
date:       2026-1-21 21:00:00
author:     "jasonzeng124"
header-img: "img/post-bg-2015.jpg"
catalog: true
mathjax: true
alter: 1
tags:
    - Robotics
---

Intake prototype is built. Works as expected. More-or-less approved to go on robot. Actually I do need to make sure that RM puts a hard stop on this thing.

Electrical spent like 2 days fixing a problem. Well anyway the motor was dead :P or something. Only took them like 2 days.

Remind me to get electrical to find the cameras for me. And a USB thumb drive.

-----

Spindexer prototype works. Works very well actually. I told them to prototype a feeder to the shooter, hasn't been done yet, I'll make sure it gets done tomorrow.

Shooter has not been cut. Today we were still making design decisions and CADing. Hopefully ready to cut by the end of tomorrowTM. Although to be honest progress on this has been too slow, we need to do this much faster.

Well, we're still quite behind. Steadily at a slower rate than my schedule.

-----

Programming wise, I got programming team to come in today.

The robot code that I wrote for the drivetrain compiles :P Although everyone is too crowded for me to actually run it. I'll get them to do that tomorrow... Or something. I really want to get reliable PIDs and test odom and stuff, before we get the new robot and it's all tuning.

Also vision. I wanted to make an automated vision tuner, did not get that opportunity yet. Although I don't really trust anyone else to do this (do I even trust myself?).

I also told VS and another guy (idk his name, fully ngl), to make some CV stuff to track the ball (to make shot tracking easier). They vibe coded it quite quickly (like by 4 it was done?), although it doesn't really meet my standards for what I want it to do yet. 

Mr. H came in today. Nothing too notable as of right now. He did tell us how we did the shot testing in 2022 (holy inefficiency: fix a distance and brute force shooter v/theta, and track that. let's say 10x speed, 10x theta, 10x distance, easily 1k shots.......). I proposed tracking with CV, he rejects it. (im fully ngl I'll do it anyway.). Other than that, not much. Also he still doesn't know that we want a turret (not that at this point we (I) have really a means to change it... AG still sticking to it and almost everyone agrees. I think we can do well both ways although im like neutral-slightly-turret-biased).

He also told me to get a programming todo list. So here it is:

1.  test shooter control w/ prototype
2.  do drivetrain sysid + test (onboard) PID + test odom
3.  (depends on: vision) test / tune apriltag localization + check instantaneous relative-pose accuracy (my prediction: not great for bad angles)
4.  vision thingy for automated ball shot tracking
5.  (depends? on: 4) ball shooting model
6.  (depends on: 1) full shooter subsystem
7.  full intake subsystem
8.  full indexer subsystem
9.  controls
10. (depends on: 5) shoot-on-the-fly
11. stupid stuff like update software

12. Remind me to get electrical to find the cameras for me. And a USB thumb drive.

Wow that's surprisingly not that much. And besides the shooter stuff, the rest is pretty much no-brain. Like run motor at 1434% speed. But damn this shooter is gonna be hard.

Ok this is all doable by freshmen. So yea....

redacted version:

1.  test shooter control w/ prototype
2.  do drivetrain sysid + test (onboard) PID + test odom
3.  (depends on: vision) test / tune apriltag localization + check instantaneous relative-pose accuracy (my prediction: not great for bad angles)
4.  (depends? on: 4) ball shooting model
5.  (depends on: 1) full shooter subsystem
6.  full intake subsystem
7.  full indexer subsystem
8.  controls

-----

One other thing. I've been spending so much time at robotics that I haven't had time to do anything else........ I have to figure out a way to allocate time better...