---
type: publication
kind: practice
status: published
created: 2026-11-06
question: How do I scale engineering without funding?
description: Grow what each engineer delivers before you grow how many there are. What to fix first, how to grow your own leaders, where AI fits, and when to make the next hire.
image:
image_alt:
image_caption:
destination: reyor.co.uk
drafted-by: claude
from: "/desk brief, 2026-11-06 (reyor-website #420): the second practice piece"
tags:
  - published
---
# How do I scale engineering without funding?

Grow what each engineer can deliver before you grow how many engineers you have. Find out where work gets stuck and fix that first, make delivery predictable, grow your leaders from the people you already have, and keep the people who know your system. Then hire when there's a real capacity constraint or a skills gap the team can't close, and pay for it with what the last improvement earned.

If you've found this, you're probably running a bootstrapped business that wants to grow without borrowing capital or destroying your margins. You're in good company: most UK businesses grow without ever selling equity, which I set out in [Do I need to raise to hire more engineers?](https://www.reyor.co.uk/desk/do-i-need-to-raise-to-hire-more-engineers/). That piece is about whether to raise. This one is about how to grow without it.

## What does "scaling engineering" actually mean?

It means engineering delivers more of what matters, more reliably, and can change course with less effort. Adding people is one way to try for that. It's the most expensive way, and the slowest to pay back.

Four measures tell you whether engineering is scaling:

- how long a change takes to go from an idea to a customer using it;
- how often what was promised arrives when it was promised;
- how often a release breaks something, and how quickly it's put right;
- how long your engineers stay.

They tend to move together. Google's DORA research has repeatedly found that "speed and stability are not tradeoffs", and that for most teams the measures are correlated ([DORA's software delivery performance metrics](https://dora.dev/guides/dora-metrics/)). A team that ships small changes often is usually the more stable one too.

## What should I fix first?

The way work flows. Before I change anything, I measure it.

I map every step a piece of work takes, from an idea to a customer using it, and how long it spends at each step: how much of that is being worked on, and how much is waiting. It's called a value stream map. The bottlenecks show themselves. A review queue, a release that only happens once a month, a decision that waits for one person to be free.

Then fix the biggest one, and measure again.

Seventy engineers in six teams were shipping on a three-month cycle, in a company that had spent a long time trying to fix it with pressure. What was slowing them down was confusion. The six teams moved from waterfall to scrum, and they got clarity about their roles, about what mattered to the business and to customers, and the autonomy to decide. [Three months became two weeks or less](https://www.reyor.co.uk/work/), and in the same year the function returned the only positive eNPS score in the department.

In the teams I've led, small, frequent releases have been the biggest single lever. A small change is quicker to check, easier to undo if it's wrong, and gets a customer's reaction sooner.

## How do I make delivery predictable?

Make it reliable before you make it fast. You can plan around a team that delivers what it says it will, even slowly. You can't plan around one that's fast but unpredictable.

A post-merger engineering team of a little over 30 people was working in silos and shipping reliably less than half the time. The technology wasn't the problem. The people had stopped trusting each other, and stopped believing in why they were there. Six months of building the foundations (structures, a shared language, and clarity about what the work was for) took [delivery reliability from below 50% to above 90%, and a $300K account that was leaving, stayed](https://www.reyor.co.uk/work/).

Most problems are people problems, and most people problems are communication problems. Predictable delivery starts with everyone knowing what's been promised, to whom, and by when … and feeling safe to say early when it won't happen.

Then when things feel stable, I have an entire technique and framework for taking that predictability to new levels, really refining that delivery engine. It's based on [the Hill equation](https://en.wikipedia.org/wiki/Hill_equation_(biochemistry)) (not mine), data-driven probabilistic forecasting, and a simple work classification system. It helps you plan and predict delivery more accurately, then gives you a way to measure it, so you can change how you work, refine your approach, and see the impact on both speed and reliability. It sounds really complicated (and it was to create) but it's not to use.

## How do I grow leaders instead of hiring them?

Look for the people already doing the work of leading: the ones others go to, who explain why, and who care about the customer as much as the code. Then give them the role, the support, and the room to grow into it.

When I moved those six teams to scrum, the delivery managers who'd been running them became scrum masters or engineering managers, depending on their skills and what they wanted to do. They weren't replaced. The people who know where the work is buried are the best placed to dig it out.

Some years ago I coached, unpaid, a lead engineer moving into their first management role. They'd be managing people who had been their peers, and that shift in the relationship is the part I've seen new managers struggle with most. We worked on setting boundaries that were fair to everyone, and on how to have impact through other people, at a scale their own code never could.

At my current client, I'm helping an engineering manager learn to run a whole research and development function, which is part sales, part marketing, part product management, and part engineering. They were already a solid manager. They were also full of ideas, a real people person, still keen to build, and frustrated at how little impact they could have as a pure engineering manager. Together we've worked on how they present themselves, how they reach out, how to lead customer conversations, how to run research, and how to make decisions quickly. It's early, and the results aren't in yet. But in their words, they're "really excited, and full of energy, and haven't enjoyed work so much in years".

Growing someone into a role costs their time and yours. Hiring into it costs months of searching, a salary set by the market, and a new person who has to learn your system and your people from scratch.

## How do I keep the engineers I have?

Give them clarity about what their job is, and a visible way up. Every engineer who leaves takes knowledge of your system that no document holds.

A 70-person function had no shared answer to what any of its jobs actually were. There was no clarity on what a role meant, no honest way to have a performance conversation, and no visible way up. So people left, and the leavers were rarely the ones anyone expected.

I built a careers framework: a shared language for what the work is, so that a manager and an engineer could have the same conversation twice. It was built for that function of 70, then adopted across the whole software organisation, 300 engineers in all. [Churn fell by around 30%](https://www.reyor.co.uk/work/). Retention improved because people finally knew what was expected of them.

## Doesn't AI change all of this?

It changes how much each engineer can produce. What decides whether that output is useful stays the same: clear priorities, good judgement, and someone who knows what good software looks like.

AI coding tools are now genuinely capable, even in old codebases, and in languages they were barely trained on. Guided by someone who knows how to build good software, and who'll challenge its decisions, AI multiplies what a small team can deliver. That makes everything above more important. A team that's unclear on what matters will now build the wrong thing faster.

In my own work with AI, what made the difference was the boring part. How we test, written down. How we build, written down. Every decision logged with its reason. It's what made human engineers better long before AI, and it turns out to do the same for the machine.

So AI is a reason to scale this way, and sooner. A well-guided engineer with AI can now do what used to take several. The guiding is the part you can't skip.

## When should I make the next hire?

When there's a true capacity constraint: the team is working on the right things, the work flows, and there's still more that matters than they can do. Or when there's a skills gap different enough that the team can't close it, or one that would create a capacity constraint if they tried.

I don't have a default for who that hire should be. Every company, every team, every skill, and every objective is different. What I'd look at is the map. If it shows the bottleneck is people doing the work, hire. If it shows waiting, decisions, or hand-offs, a new person adds to the queue.

Pay for it with what the last improvement earned. When you've shipped faster, kept a customer, or freed capacity, the margin that creates is what funds the next person. That keeps your growth in step with your revenue. If you'd rather borrow for it, the first piece has [what debt changes, and what it doesn't](https://www.reyor.co.uk/desk/do-i-need-to-raise-to-hire-more-engineers/).

## What does it cost to do it this way?

Patience, mostly. The hard part is measuring change whose results arrive late.

Most of what matters here lags: reliability, retention, how quickly a team can change course. It's easy to measure a quarter or two, not see the change you wanted, and stop … just as you were on the edge of a real shift. It's like starting to post and write with no presence at all, and stopping at month six because there are no new leads yet, when you've gone from nothing to steady engagement and a name in the places that matter.

So decide up front what you'll measure, which early signs you'll accept on the way (fewer items waiting, shorter reviews, a release that went out when it was promised), and how long you'll give it before you judge it.

It cost me, too. Moving the 70 engineers to a new way of working cost me my standing with some of the senior leadership, in a company that expected leaders to know every detail. Leaving room for teams to decide meant walking into meetings without the answers they expected, and being honest about the ambiguity instead.

If you'd like help with it, this is what I do. In two weeks, find out whether your next stage needs capital, or whether the capacity is already in the building. It's called the Growth Without Dilution Plan: three or four days of my time inside your company, looking at the delivery itself (how long work waits, where it waits, and why), then a written plan showing where your capacity is trapped, what unlocking it takes, and what the alternative raise would cost you in equity, side by side. You keep the plan whatever you decide.

**[Let's find another way](https://www.reyor.co.uk/another-way/)**

## Who this is for

Founders and CEOs of companies up to £20m in revenue that have grown on their own money, exist to do something rather than only to reach an exit, and want engineering to deliver more without raising. That's whether you're building to sell one day, to hand on, or to run for decades. And founders who've decided, from the start, to build this way.

It isn't for VC-backed companies that have already chosen capital and hypergrowth, for private equity portfolio operations, or for anyone looking for a CTO to run sprints.

**[Let's find another way](https://www.reyor.co.uk/another-way/)**
