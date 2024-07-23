---
layout:     post
title:      "reflections on 8 years of robotics - part ii"
subtitle:   "...high school"
date:       2025-11-27 23:00:00
author:     "jasonzeng124"
header-img: "img/post-bg-2015.jpg"
catalog: true
mathjax: true
alter: 1
tags:
    - Life
    - Robotics
---


\dots......


Note: I might personally be a bit salty, it definitely leaked into here, so perhaps don't take *everything* at face value.


Well, the next year (2022) I started high school, and FRC robotics. I joined programming team, and soon enough I became literally the only member of programming team (ok, this is a bit of an exaggeration. But it wouldn't be inaccurate to say that I led the programming team since freshman year).

It also happens that our programming team collectively scared away all the freshman between 2022 through 2024. I'll elaborate on this later, and other problems related to recruiting, later.

<p style="text-align:center;">* * *</p>

Some background on the 2021 team. It consisted of three of the most experienced (IMO) people, originally from LH robotics, plus another very experienced mechanical member. They were able to design their robot over kickoff weekend, get their robot to programming a while before the competition, and had an entire *two weeks* of testing. No wonder they got to worlds.

Then they graduated (along with some advisors). This presented a problem for our team, which will become apparent very quickly.


<p style="text-align:center;">* * *</p>

**2023: cubes and cones; Captain: IH (co23), Programming Cap: TB (co24)**

When the 2023 season (the cubes and cones one) started, I was actually quite inexperienced with FRC, and proposed a bunch of designs that (in retrospect) would probably fail, or at least fail somewhat. But I did have somewhat of an idea of what I was doing.

One of the things I did tell our team, literally at the outset, was not to care about tilted cones on the ground. This idea was met with quite a lot of opposition, especially from a certain safety captain. We ended up doing as I told them to, at least for this aspect, but it took them a lot longer to realize it.

Actually, at this point I already had some influence over the design process. But our design team (well actually just LXM, a sophomore) went through many flawed ideas, and by week 3 we were really desperate just to build anything.

The design was a tilted elevator with a two-segment arm and a normal end effector. I wasn't really sure about the design (retrospectively, I actually like it). One other thing it had was an H-drive. One thing about H-drives (that I know from experience from 2018) is that it's hard for the center wheel to touch the ground, so they went with a robonauts-2018 type suspension (it's quite quirky). I told them to go with a normal suspension, they said no. I didn't believe it would work, and I told everyone so, but they thought, you know, 118 did it, they won, you know, why can't we do it? Well, I had no choice but to approve it, I guess (hint: it didn't work).

(I wonder why 118 could do it? I'll get to that later).

The robot ended up being finished(*) literally 3 days (ok maybe more I don't exactly remember) before our first competition. We can all guess how that turned out..................

(*) not as finished as I would have liked...

Oh and sometime in the middle of the season we were asked to deposit some money to pay for plane tickets. haha.

Oh, and one more thing. We put LED strips on the robot. And programmed them. To flash in rainbow.

To be honest, this is everything you really need to know about 41.

Ok, with minimal personal saltiness, here is what actually made us fail:
 * code issues (really, not enough testing time)
 * the autos were not very reliable (also, we had localization issues)
 * electrical issues (somehow no other team has as many electrical issues as we do)
 * mechanical issues with the elevator
 * the h-drive mechanism didn't work

<p style="text-align:center;">* * *</p>

**2024: throwing rings; Captain: TB, OG (co24), Programming Cap: BP (co25)**

Sophomore year came. This year, we got swerve drives, and we (during robotics class) programmed most of the swerves before the season (we didn't get to path planning, and localization was still spotty. well both of these are still spotty). It turned out to be very reliable.

Build season came, luckily for our team it was a shooter game with only one game object. Our design was a ground intake, that flipped around to meet a shooter that rotated on a pivot. Again, I liked this design. My only concern was the handoff, I told design to make sure it would work (hint: it didn't work that well).

Everything appeared to be going well, albeit a bit slowly. And then, we had a bunch of technical issues with the intake (i.e. a bunch of chains that are the wrong length etc, mounting issues). Well this resulted in the intake being an absolute nightmare for programming to control. And the handoff became infinitely harder to pull off.

Also we couldn't really nail down localization, but that's really our fault...

Anyway, programming got the robot 1.5 weeks, ish, before the competition? We definitely didn't get autos working, but we coded most of the functionality. somehow we coded shoot-on-the-fly?????

Anyway, the competition didn't go well. The next competition two weeks later actually went pretty well, because ~~the robot code actually worked~~ no, i wish. we just played defense. yes.

Sidenote, a bit toward competition season I was less invested in robotics, because of USACO.

So another somewhat-objective analysis:
 * the intake was badly-designed, so it was horrible to actually use and/or code
 * the handoff was somewhat cooked because of the intake
 * there were localization issues so we couldn't shoot reliably
 * no autos, and when we added autos, they weren't really reliable either
 * would've been nice to get more testing time

<p style="text-align:center;">* * *</p>

**2025: pipes and balls; Captain: TA (co25), Programming Cap: BP (co25)**

Junior year. wow, this year, really.

The game was about putting pipes on poles, and putting balls in places. Our design (my proposal, this time), was a telescoping arm with a wrist, that would pick up pipes and put them on the poles. My main concern this time was geometry, and making sure the arm could actually reach all the poles (hint: we were a few inches short).

Everything went as usual, that is to say, slowly. There were excuses made for not having the full shop. Well, these are really just excuses. Anyway, programming got the robot around 1.5 weeks before the competition.

One stupid thing we did was that we wired all the wires inside of the box tube. Well, guess what happens when we have to troubleshoot electrical issues? :D (answer: you have to take literally everything apart. iirc this happened once or twice).

Well a lot went wrong the first competition. For one, the kids had to stay until like 2 am because the main weld broke. And you know what happens when you try to weld something, on a robot? (hint: welding involves melting things by putting a massive amount of current through metal, so a motor died). Also, we had issues with the intake being bad so that it would miss a lot of pipes.

Again, toward the end of the season I became more interested in USAPhO than trying to make the robot work, so yea. It's a shame that BP codes before he thinks sometimes, because programming team without me wasn't very pretty...

Anyway:
 * weld broke
 * intake was kinda bad
 * fixing stuff on the telescopes was a pain
 * we were a few inches short from consistent L4 scoring
 * autos
 * autos, again
 * oh, and i forgot, driver practice. this applies to past years too

<p style="text-align:center;">* * *</p>

I think the biggest obstacle we faced these years, is as Dr. Stiles (one of our mentors put it), resistance to change. He complained that nobody *really* listened to him, or Mr. Hadzic, when they gave ideas. Nobody listened to me, either, really, especially the first year.

After the 2021 cohort went to worlds, everyone else thinks that they are better, that if the previous year went to worlds, they could too. And then they overengineer and well, this happens. To an extent, our team still thinks like this. Once, I thought that once the entire cohort of 2021 members graduated, we might become better again. Well, this is the year. And it appears that this may not be the case.

I once thought like this too. I still think like this sometimes. But failing several times is surprising effective at stopping this type of thinking.


<p style="text-align:center;">* * *</p>

I sometimes say that I personally approved all three of the robots. This is pretty accurate, but not entirely true. All three of the robot designs, conceptually, could have done very well, if properly executed. But something keeps on preventing us from executing well.

Design wise, I feel like we have complex designs, and yet they aren't reviewed properly, resulting in pretty costly mistakes. And because of the way everything is designed, it's really hard to fix these mistakes.

For mechanical, we just take too long. Maybe the parts are too complex, maybe we are just slow, I don't know. It just shouldn't take this long. Other teams just cut stock (with pre-cut evenly spaced holes) to size (like approximately to size, not 1/1000 in to size) and drill it in, and we somehow just can't do this.

Electrical, somehow no other team ever has as many electrical issues.

When the other subteams do something wrong, programming suffers. It's always programming. That said, there are things programming could do better. Like pre-coding every subsystem, properly having code review, and in general coding better. And prioritizing autos more.

<p style="text-align:center;">* * *</p>

There are teams that have half of our size, half of our budget, and half of our machinery. Many of them beat us. And yet, a lot of the time when we lose, we say that X team has Y money, Z mentors, and W team members.

And if we doubled our size, budget, and machinery, so what? would we really be *that* much better?


-----

Now that I'm actually thinking about it, let's just accept it. 41 won't make worlds this year. That doesn't mean we shouldn't try to, but more so that we shouldn't think in an all-or-nothing manner.

more to come...


P.S. some golden, quotes (well paraphrased, but the idea is there)

> "This isn't how 41 works, Jason. We [perfectly] engineer all of our parts"

> "We have a CNC for a reason, we shouldn't need to drill mounting holes ourselves"

haha, i know exactly how 41 worked. it didn't.