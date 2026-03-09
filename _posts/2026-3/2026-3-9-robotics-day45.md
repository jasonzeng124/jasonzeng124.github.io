---
layout:     post
title:      "robotics, days 37 to 45"
subtitle:   "frequency of yelling curse words increased 20x"
date:       2026-3-9 20:00:00
author:     "jasonzeng124"
header-img: "img/post-bg-2015.jpg"
catalog: true
mathjax: true
alter: 1
tags:
    - Robotics
---

I just typed 4141 into my personal laptop today :fall:

I also have hit like >300 hours on robotics, probably.

Anyway, now that comp is over, a day-by-day summary of what happened each day:

note, AG was unfortunately (fortunately?!?!) out from day 36 to day 39. i wish i was, too.

**day 37, 3/1**

like 2-6 in Mentor M's garage. got turret more-or-less working (*actually not really, the tuning sucked although at the time I was too tired to notice, kP=200 go brrr.) hood working. intake had bearing issues, didn't get to do that. did flywheel tuning. anyway EOD it was shooting, kinda.

from dms with AG:

> hood brok
> 
> intake needs fixes
> 
> i still need to fix vision
>
> spindexer clogs are fine, most of them don't seem to be issue

**day 38, 3/2**

> "i can finally rest now cuz nothing works mechanically" --me, circa 8:20 mar 2 2026

i think they fixed bearing, then did more of something IDR. intake bearing issue fixed. while tuning intake, the intake joint gears kill themselves because of a somewhat bent axle, the gears grind out. RIP gears. Anyway Mentor H comes in, asks to spin the intake (with joint down). We do, one of the pulleys grinds itself out too, becomes a bearing instead of a hex bore (this is what happens when you 3dp pulleys). Anyway he advises us to forgo intake and focus on only climbing and defense. And to make an 8-ball shot auto.

*he turns out to be right, but unfortunately nobody took him seriously back then*

> i might not have robot all of tomorrow
>
> there is serious talk of skipping wednesday
>
> only now i can lowk understand the teams that are assembling a drivetrain at comp

**day 39, 3/3**

Tried to replace gears on intake. Another set of gears with no teeth, now. Changed to chain and sproket, worked fine. finally. only took us until like 9 pm.

climber has some issues. at least for L3 it does. will take like 3 days to fix

at this point i think it might be feasible to have a working robot by comp. at least thats what I tell AG.

**day 40, 3/4**

i think on this day we like had everything working for a while, ish. actually we demo'd it to Mr. G's class and it made like 8/10 balls in.

Anyway ponz advises us to move breaker and not use solder. it takes CET like 4 entire hours to do this and he ends up soldering in the end anyway. (more to this...)

There is something to shooter (i lowk forget) but KL fixes it.

Some time today i crash out and threaten to quit if they don't get it done by 7. They do get it done by 7, barely. I should've quite anyway, ngl, sometimes I wish I did.

after that i stay until like 10:30 doing stuff. by myself. :wilted_rose:

Turret has backlash issue so it doesn't aim right within \pm 10 degrees. Also other issues with it being inaccurate.

**day 41. 3/5**

funny how day 41 is the most like team 41.

KL redoing turret. Mentor M mounting climber. Problems with elevator due to turret screws hitting. Playing with elevator. \dots.

entire time, i'm literally sitting on the bump (that they took time away from prototyping to build, and we never used it, and the only thing that happened with it is it fell on the floor a few times). I give up and leave early because there's no way that I'm getting it in time.

Got fortune cookie: "vacation awaits you. plan the trip today". perhaps fortune cookies are right sometimes.

**day 42. 3/6**

load in day. except the robot isn't done.

> me staring at robot
>
> Mentor S: "are you surprised?"

6:30, it's not done, but we have to go. we go there and inspect etc.

so KL applies a fix during load-in and we finally like kinda have a finished robot.

**day 43. comp, day 1**

Me and LYT and Claude Code vibe tune a shooter tuning on the bus. it unironically works perfectly.

practice match is ok but we kinda suck. we lose power in middle i think.

first match, i do some code deploy that has some type error and it fails. LMAO.

second match, we lose power? i don't remember really. anyway they think its a power connection and they think they figure it out and fix.

third match, we still lose power or something.

Mentor L and CET take a look at power. apparently some loose power solder joint. who told them not to solder?

fourth match, no show.

fifth match, we still lose power. something to do with ring clamps on breaker. they fix it i think after borrowing a breaker.

at some point they fix everything but there are still brownouts. at this point garrett takes a look and he tells us we're drawing too much power. Apparently 300 amps is too much LMAO i should've done some thinking.

I add current limits to everything. starts working.

at this point its like 2nd last match of day, and they are still fixing stuff between every comp. something is also limiting our shooting or intaking capacity severely and idk what. also random shooter issues.

at some point i also decide to just try l1 climb unconditionally even though it isn't tested. it works, but the hooks bend too much for l2/l3. so much for the climber.

**day 44. comp, day 2**

before EOD yesterday I deleted intake and whatever from code and decided that we were going to be a defense bot. We do better in defense than scoring like 5 balls a match, anyway.

4 uneventful defense matches.

anyway alliance selection, we are chosen 2nd pick of 4th alliance.

we play defense, forgoing hang cuz it's not worth compared to defense.

one match driver station breaks. AG driving on single joystick (no turn) rotated 90 degrees :fall:

next match some drivetrain encoders break or something IDK what really. AG driving on xbox controller with like 2 swerve modules intact and just trying to wiggle to the right direction. "hit them" "how are you hitting them with this"

they try to replace encoders, anyway they run out of time and alliance calls backup robot. they can't drive defense and it is a throw rip. KC and AP say we would have won if we could defend.

so that is story of how we managed to break every subsystem on the robot.

Anyway they decide to make a new robot, basically a copy of lunatecs / WCP CC / my bathtub. :wilted_rose: what was I trying to tell them to do in february? anyway they aren't finishing it now. no way.

> "we don't need 5 weeks to build a backup robot"
>
> now you have 3, are you happy CET???? are you??????

oh and won innovation in control. scam. that thing was made like 6 years ago and hasn't changed since.

it is funny, we get 29 district poitns out of like 60 required which is a lot, considering our robot entirely didn't work.

**day 45, 3/9/2026, today**

slept until 2 today :fall:

anyway visited for a bit. tried to get them to draw a 1:1 scale diagram on whiteboard. they won't. :wilted_rose:

they aren't finishing this if they can't draw it 1:1 on a whiteboard and start assembling immediately.

I took brief look at old robot. minimum 1 weeks to get it fixed and working, I think. I'd prefer to work on a new robot but I don't think I really have a choice, I'm probably going to have to work on this one.

-----

this year might be our best chance at qualifying for lehigh (although if we qualify for lehigh I don't necessarily go). and our best chance at worlds, maybe (i would def go). simply due to rng, not even due to us being good in any way :skull:. hopefully the team does not throw...