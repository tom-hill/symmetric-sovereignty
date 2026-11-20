---
type: publication
kind: practice
status: published
created: 2026-11-20
question: Why is my engineering team slow?
description: Usually not because anyone is working slowly. Where the time actually goes, the three things it waits on, and what to check before you hire another developer.
image:
image_alt:
image_caption:
destination: reyor.co.uk
drafted-by: claude
from: ~/Documents/Desk/briefs/why-is-my-engineering-team-slow.md
tags:
  - published
---
# Why are my developers slow to ship?

Usually not because anyone is working slowly. Most of the time a piece of work spends between an idea and a customer is spent waiting, not being worked on. What it waits on is almost always a lack of clarity about what to build and why, a lack of trust to raise problems and ship, or a lack of purpose. Find where your work waits before you hire anyone to speed it up.

If you've found this, you probably feel your developers ship too slowly. Customers are waiting for things you promised, competitors seem to move faster, and you've started to wonder whether the answer is more people, and if you should raise money to pay for them. You also may not be technical, which makes it hard to tell whether the team is slow, the work is hard, or something else is going on.

But as I say a lot, most problems are people problems, and most people problems are communication problems. A slow team is usually one of them.

## Slow compared with what?

Start here, because "slow" means different things to different people. To you it might mean a feature arrived a month late. To your developers it might mean the release process takes a week. Until you agree what you're measuring, you'll argue about the answer.

Two measures do most of the work:

- how long a small change takes to go from an idea to a customer using it;
- how often what was promised arrives when it was promised.

Measure them before you change anything, so you can tell later whether what you changed helped. And don't trade one for the other. Google's DORA research has found that "speed and stability are not tradeoffs" ([DORA's software delivery performance metrics](https://dora.dev/guides/dora-metrics/)). The teams that ship most often tend to break things least.

## Where does the time actually go?

Mostly into waiting. A piece of work waits for someone to decide what it should be, for a developer to be free, for a review, for a test environment, for a release that only happens once a month, or for an answer from the one person who knows.

You can see it by following a few pieces of work from the moment someone asked for them to the moment a customer had them, and writing down how long each spent at each step. It's called a value stream map, and I describe how I do it in [how to scale engineering without funding](https://www.reyor.co.uk/desk/how-do-i-scale-engineering-without-funding/). The first time most founders see one, the surprise isn't how long the work takes. It's how little of that time anyone was actually working on it.

When you ask why the work was waiting, the answers usually come back to one of three things.

## Is it clear what they're building, and why?

When it isn't, work starts before it's understood, gets changed halfway through, and waits while someone finds out what was meant. Priorities shift each week, so nothing gets finished. Developers build exactly what they were asked for, and it's still wrong.

Seventy engineers in six teams were shipping on a three-month cycle, in a company that had spent a long time trying to fix it with pressure. Everyone had agreed the problem was speed. Nobody had asked what was actually slowing it down. It was confusion, not effort. The teams got clarity about their roles, about what mattered to the business and to customers, and the room to decide for themselves. [Three months became two weeks or less](https://www.reyor.co.uk/work/). The pressure had been the thing slowing them down.

Every case study says what it cost me, and that one cost me my standing with some of the senior leadership. The company expected leaders to know every detail. Leaving room for the teams to decide meant walking into meetings without the answers people expected, and being honest about the ambiguity instead. I was called a rebel, and incapable. I'd do it the same way again.

## Do they trust each other enough to ship?

When they don't, everything gets checked twice, problems are hidden until they can't be, and nobody wants to be the one who releases something that breaks. Releases get bigger and rarer, because each one feels risky, and bigger releases are riskier still.

The most expensive thing in a slow team is bad news that travels slowly. A developer who knows on Tuesday that a date won't be met, and doesn't feel safe saying so until the Friday before, has cost you weeks you could have planned around. Feeling safe to speak up isn't a nice-to-have you fix after the next hire. It's how fast the truth reaches you, and that shows up in your profit and loss.

A post-merger engineering team of a little over 30 people, across three continents, was working in silos and shipping reliably less than half the time. The technology wasn't the problem. The people had stopped trusting each other. Six months of building the foundations that should have been there from the start (structures, a shared language, and genuine clarity about what the work was for) took [delivery reliability from below 50% to above 90%, and a $300K account that was leaving, stayed](https://www.reyor.co.uk/work/).

## Do they know why it matters?

The same team had also stopped believing in why they were there. That's the third thing, and the one founders find hardest to see from outside, because a team without purpose still turns up and still works hard. It just stops caring whether the work lands.

You see it in small ways. Nobody asks how a customer reacted to a release. Nobody pushes back on a request that makes no sense. Good people leave, and the leavers are rarely the ones you expected.

The number in that team's story was the consequence, not the point. The point was that 30 people came to work on a Monday with a reason to be there.

## Isn't it just the code?

Sometimes. Old code nobody dares change, builds that take twenty minutes, and no automated checks to catch a broken change before a customer does are all real, and they do slow a team down.

But in my experience they're usually what a lack of clarity or trust leaves behind, not the cause. Code gets tangled when nobody has the time or the permission to tidy it, and checks go unwritten when the pressure is always on the next feature. A team that's clear on what matters, and safe to say so, makes the case for fixing them, and gets it fixed. A rewrite without that just builds the same tangle again, but newer.

## Will hiring more developers fix it?

Usually not, and it often makes it slower. Every new person adds conversations, handovers, and decisions that need agreeing, and they need the team's time to get up to speed. If the work is waiting rather than being worked on, a new developer adds to the queue. I set out the maths in [do I need to raise to hire more engineers?](https://www.reyor.co.uk/desk/do-i-need-to-raise-to-hire-more-engineers/).

The same goes for a new senior hire. If the work waits between deciding what to build and building it, the gap I describe in [do I need a CTO or a CPO?](https://www.reyor.co.uk/desk/do-i-need-a-cto-or-a-cpo/), a second leader gives it two owners rather than closing it.

Hire when the map shows the team is working on the right things, the work flows, and there's still more that matters than they can do.

## What should I do first?

Measure before you buy. Follow a handful of pieces of work through, find where they wait, and ask why. You'll usually find the answer is already in the building, and costs far less than another salary.

If you'd like help with it, this is what I do. In two weeks, find out whether your next stage needs capital, or whether the team you already have can get you there. It's called the Growth Without Dilution Plan: three or four days of my time inside your company, looking at where work waits and why, then a written plan showing where your capacity is trapped and what unlocking it takes. You keep it whatever you decide.

**[Let's find another way](https://www.reyor.co.uk/another-way/)**

## Who this is for

Founders and CEOs of software companies up to £20m in revenue that have grown on their own money, exist to do something rather than only to reach an exit, and feel their team should be shipping faster than it is.

It isn't for companies that have already chosen capital and hypergrowth, or for anyone looking for someone to push their team harder.

**[Let's find another way](https://www.reyor.co.uk/another-way/)**
