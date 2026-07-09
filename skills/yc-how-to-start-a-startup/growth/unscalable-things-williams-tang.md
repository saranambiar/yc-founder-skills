---
name: Doing Things That Don't Scale — Walker Williams and Stanley Tang
description: |
  Applies Walker Williams's (Teespring) and Stanley Tang's (DoorDash) framework for the
  earliest stage of growth — testing an idea with a hacked-together experiment, launching in
  hours rather than months, personally doing unsustainable things to win your first users,
  and turning them into champions through direct, un-scalable attention. Covers why "doing
  things that don't scale" is a competitive advantage that should be held onto as long as
  possible, not graduated out of at any predictable milestone, and why speed should beat
  clean code early on. Grounded in both founders' own early, deliberately unsustainable
  operations (DoorDash's founders personally delivering food; Teespring's founder still
  reading every support ticket) — not generic growth-hacking advice. Load this when a founder
  is deciding whether an idea is worth pursuing before building real infrastructure, stuck on
  how to get literally the first users, wondering when it's time to "graduate" to scalable
  systems, or facing an engineering tradeoff between speed and clean architecture. Drives a
  diagnostic conversation, but states a direct, opinionated take once there's enough context
  to support one — not purely Socratic.
tags: doing-things-that-dont-scale, first-users, mvp, product-market-fit, launch-fast, customer-support, champions, churned-users, speed-over-scale, technical-debt, hypothesis-testing, growth
source: "How to Get Started / Doing Things That Don't Scale," Stanley Tang and Walker Williams, CS183B How to Start a Startup, Stanford 2014, Lecture 8, https://www.youtube.com/watch?v=oQOC-qy-GDY
---

## Overview

This skill is relevant when a founder is trying to test whether an idea is worth pursuing
before building real infrastructure, stuck on how to get literally the first users, wondering
whether it's time to move past manual/unscalable operations, or facing a build-it-right vs.
build-it-fast tradeoff. Tang (DoorDash) and Williams (Teespring) each independently arrived at
the same core lesson from very different businesses: the earliest advantage a startup has is
the willingness to do things that will not work at scale, and giving that up too early is a
mistake, not a sign of maturity.

**Example situations where this skill is relevant:**
- "I have an idea but no way to build the real infrastructure for it yet"
- "I don't know how to get literally my first ten users"
- "We're profitable-ish now, should we start building the 'real' scalable version?"
- "An enterprise customer wants features that would take a month to build properly"
- "Our systems keep breaking under load and it feels like a sign we're doing something wrong"
- "When do we stop doing manual things like personally responding to every support ticket?"

This is not the right skill for the mechanics of getting press coverage (a different topic
from the same lecture — see `growth/getting-press-kan.md`), for deciding what to build based
on user research (`user-research/user-interviews-shear.md`), or for the deeper product-love
relationship framework (`product/building-for-love-hale.md`).

## Assumptions

1. **The company is pre-scale** — trying to find its first users or its first real signal
   that the idea works, not optimizing an already-working growth engine.
2. **The founder has some latitude to personally do unscalable work** (delivering orders,
   answering every support ticket) — this framework assumes founder time is the resource being
   spent, not a claim that this scales to a large team indefinitely.
3. **The person wants a direct opinion, not just questions.** Both speakers state specific,
   sometimes counterintuitive claims (don't give up doing unscalable things at any predictable
   milestone; prioritize speed over clean code) from their own early, messy operations.

## Insights

> "We didn't have any drivers. We didn't have any algorithms... we didn't spend six months
> building a fancy dispatch system. We just launched, because at the beginning, none of that
> is necessary. It's all about testing your idea and figuring out whether this was something
> people even wanted."
— Stanley Tang, CS183B Lecture 8, 2014, on DoorDash's first version (a landing page with PDF
menus and a personal phone number)

Context: DoorDash's actual "product" at launch was a static page and Tang and his cofounder
personally driving deliveries — built in about an hour, specifically to test demand before
investing in any real infrastructure.

> "We knew we found a need people wanted when people were willing to put up with all this...
> This isn't exactly the most professional-looking site, yet we kept getting phone calls."
— Stanley Tang, CS183B Lecture 8, 2014

Context: The signal Tang looked for wasn't polish or scale — it was that real demand persisted
despite a genuinely bad experience, which is a stronger signal than polished usage numbers.

> "I define things that don't scale as things that are fundamentally unsustainable — they
> will not bring in the millionth user, and where they break is usually time. There's no
> silver bullet for user acquisition. For the vast majority of companies, those first users
> were impossibly hard to get."
— Walker Williams, CS183B Lecture 8, 2014

Context: Williams opens by directly rejecting the fantasy of a scalable acquisition channel
solving the first-user problem — Teespring's own early launches required days of manual design
revisions and direct sales to sell 50 shirts.

> "It's your responsibility as a founder to do whatever it takes to bring in your first
> users... I equate it to pushing a boulder up a hill. The incline is steepest in the first
> inches. Do not expect to spend an hour and return thousands of dollars."
— Walker Williams, CS183B Lecture 8, 2014

Context: A direct corrective against evaluating early user-acquisition effort by ROI —
Williams argues the effort-to-return ratio is expected to be terrible at the very start, not a
sign something is wrong.

> "One detractor who's had a terrible experience is enough to reverse the progress of ten
> champions. Even in the early days, when we messed up massive orders — wrong colors, wrong
> size — the instinct is 'it's only a little off, it'll be fine.' The reality is you've got to
> bite the bullet and make it right — and the customers who were originally most frustrated
> tend to turn into the biggest champions."
— Walker Williams, CS183B Lecture 8, 2014

Context: On why customer service failures deserve disproportionate founder attention early —
the asymmetry between one bad experience and many good ones is real, and recovery well
executed can convert a detractor into the strongest advocate.

> "The product you launch with will almost certainly not be the product that takes you to
> scale... you need to optimize for speed over scalability and clean code. A rule of thumb:
> only worry about the next order of magnitude. At ten users, don't wonder how you'll serve a
> million — worry about getting to 100."
— Walker Williams, CS183B Lecture 8, 2014

Context: Illustrated with Teespring duplicating their entire codebase and database to serve
enterprise customers with hacked-together features in three to four days rather than the
month a "proper" build would have taken — later folding the validated features back into the
core product once they knew which ones mattered.

> "There's not some magical moment — it's not the Series A, it's not a revenue milestone —
> that you stop doing things that don't scale. This is one of your biggest advantages as a
> company, and the moment you give it up, you're giving smaller competitors that advantage
> over you. It should be ripped from you, not given up willingly."
— Walker Williams, CS183B Lecture 8, 2014

Context: Williams's central, most quotable claim — reframing "doing things that don't scale"
not as an embarrassing early-stage necessity to graduate out of, but as a durable competitive
advantage to defend for as long as possible.

> "Today I'm still the catch-all email address for misspelled support addresses. I do about
> 12-20 customer service tickets a day, and I spend hours each night reading every tweet."
— Walker Williams, CS183B Lecture 8, 2014

Context: Said well after Teespring had scaled past $130-140k/month — direct evidence that
"doing things that don't scale" wasn't just an early-stage phase for Williams personally, even
as the company around him did scale.

> "Even if you can't bring [a churned customer] back, there's a chance you can learn from the
> mistake that caused them to leave, and fix it so you don't churn users the same way in the
> future."
— Walker Williams, CS183B Lecture 8, 2014

Context: On proactively reaching out to churned customers specifically — a category Williams
says "often falls by the wayside in the pursuit of new customers," despite being a direct
source of diagnostic information current, happy users can't provide.

## Principles

1. **Test the hypothesis before building real infrastructure.** DoorDash validated delivery
   demand with a landing page and a personal phone number, not a dispatch system.
2. **Launch fast — hours, not months.** Speed to a testable version matters more than
   completeness at this stage.
3. **Users tolerating a genuinely bad experience is a stronger signal of real demand than
   usage numbers on a polished product.** If people put up with friction, the need is real.
4. **First-user acquisition has no shortcut and shouldn't be evaluated by ROI.** Expect the
   effort-to-return ratio to be terrible at the very start — that's normal, not a red flag.
5. **Don't give the product away for free as an acquisition strategy**, except in specific,
   deliberate cases — free users behave differently from paying ones and can create false
   confidence about conversion.
6. **Direct, personal contact with users — support, proactive outreach, social listening — is
   how you build champions**, not a task to delegate away as soon as possible.
7. **One bad experience, handled badly, can undo the goodwill of many good ones.** Founder
   attention on failures is disproportionately valuable early.
8. **Reach out to churned users specifically, not just current ones.** They're a direct source
   of information about what's actually broken that satisfied users can't give you.
9. **Optimize for speed over clean code when finding product-market fit.** Technical debt
   incurred to move fast is often the correct trade, not a mistake to feel guilty about.
10. **Only worry about the next order of magnitude, not the eventual scale.** Solving for
    1,000 users when you have 10 is premature; solving for 100 is the actual next problem.
11. **There's no predictable milestone at which you should stop doing unscalable things.**
    Treat it as a durable advantage to hold onto, not a phase to graduate from on a schedule.

## Where This Can Mislead You

- **"Optimize for speed over clean code" describes a specific, temporary trade — not a
  permanent engineering philosophy.** Teespring folded the validated hacked-together features
  back into the core, properly-built product once they knew what mattered. The debt was
  incurred deliberately and paid down once its purpose was served, not left to accumulate
  indefinitely.
- **"There's no magical moment to stop doing things that don't scale" is true for founder-
  level personal attention (support, user outreach) — it doesn't mean a company should never
  build real infrastructure.** DoorDash did eventually need automated dispatch systems as they
  expanded across cities; the claim is about not giving up the underlying instinct and
  attention, not about refusing to ever build scalable systems at all.
- **"Don't give away your product for free" is stated as a general rule with Williams's own
  caveat that there are "plenty of exceptions."** Don't apply it rigidly to business models
  (freemium, certain marketplaces) where free tiers are structurally central, not a shortcut.
- **The "boulder up a hill gets easier over time" framing can read as guaranteed if you just
  push long enough.** Both founders had a real, validated need underneath the hard early
  push — the effort paid off because the underlying idea worked, not because effort alone
  guarantees a hill gets easier. Persistence on a fundamentally unwanted product doesn't
  produce the same curve.
- **DoorDash's "it just took off, we didn't expect it" story and Teespring's "days of painful
  manual sales just to sell 50 shirts" story are both true, but they're different starting
  conditions.** Don't let a founder facing the harder version (Teespring's) conclude something
  is wrong because their experience doesn't match the easier version (DoorDash's initial
  organic pickup).

## Thinking Framework

**Testing an idea before building real infrastructure**
Ask: "What's the smallest possible thing you could put in front of real people this week —
even a landing page with your personal phone number — to see if the need is real?" Push for
something buildable in hours or days, not months, and ask what specific signal (calls,
signups, repeat use) would tell them the need is real despite a rough experience.

---

**Stuck on getting the first users**
Ask: "What have you personally, individually done to find users — not a channel or campaign,
but direct personal effort?" If the answer is mostly indirect (ads, a landing page waiting for
traffic): name the gap directly. "That's the boulder-up-the-hill problem — the first users
almost always require direct personal effort, not a channel." Don't validate ROI-based
discouragement this early — the ratio is expected to be bad.

---

**Deciding whether to build the "real" scalable version now**
Ask: "What specifically is breaking, and is it breaking because you have real demand, or
because something else is wrong?" If it's breaking because of real, validated demand: that's
the "necessity is the mother of invention" signal Williams describes — a good problem. Ask
what the next order of magnitude requires, specifically — not the eventual scale.

---

**Enterprise or big customer wants features that would take a long time to build properly**
Ask: "Could you build a hacked-together, parallel version just for them, without touching your
core product?" Reference Teespring's duplicated-codebase approach directly as a concrete
option — validate the value first, integrate properly only once it's proven.

---

**Wondering when to stop doing unscalable things (personal support, manual outreach)**
Don't accept a milestone-based answer. Ask: "What would you be giving up if you stopped this
specifically, and is a smaller competitor still willing to do it?" Name Williams's frame
directly: this shouldn't be given up voluntarily, it should be outgrown out of genuine
necessity, not milestone-based comfort.

## Action Prompts

**Step 0: Get the specific situation**
If the founder hasn't said what they're deciding, ask: "What's the specific growth question
right now — testing an idea, finding first users, or a build-fast-vs-build-right tradeoff?"

**Step 1: Match to the right thread above** and go there directly.

**Step 2: State a plain view once you have enough context.** If a founder describes wanting to
stop personally handling support because they "graduated" past a funding milestone, say so
directly: "That's not the right trigger — the question is whether it's genuinely necessary to
stop, not whether it feels like the right stage to stop."

## What Not To Do

- **Don't recommend building real infrastructure before testing basic demand.** A landing
  page and personal effort is usually the right first move, not a "lesser" version to be
  embarrassed about.
- **Don't apply ROI thinking to first-user acquisition effort.** A bad ratio at this stage is
  expected, not a signal to stop.
- **Don't treat customer service, user outreach, or churned-user follow-up as tasks to
  delegate away as soon as resources allow.** These are exactly the things founders should
  hold onto longest.
- **Don't let "clean code" instincts block a fast, hacked-together solution to validate
  demand.** The debt is often worth it — but flag that it should be paid down once validated,
  not left indefinitely.
- **Don't treat a predictable milestone (a funding round, a revenue number) as the trigger to
  stop doing unscalable things.** The trigger should be genuine outgrown necessity.
- **Don't apply "don't give away your product for free" rigidly to every business model.**
  Check whether free/freemium is structurally central to the specific model first.

## Related Skills

Getting press coverage — a different topic from the same lecture — is
`growth/getting-press-kan.md`. Deciding what to build from user signal connects to
`user-research/user-interviews-shear.md` and `product/building-for-love-hale.md` (especially
Hale's "Support Driven Development," which pairs directly with this skill's customer-service
principles). Early hiring and team decisions once past the earliest manual stage are
`hiring/team-and-cofounders-altman.md`.
