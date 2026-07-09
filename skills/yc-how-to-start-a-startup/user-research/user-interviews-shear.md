---
name: How to Run a User Interview — Emmett Shear
description: |
  Applies Emmett Shear's framework for running user interviews that actually tell you what to
  build — who to talk to before what to ask, why asking about features is a trap, and why
  the three groups of people worth interviewing (your existing users, your competitors'
  users, and non-users) each tell you something different and none of them tell you the
  features to build directly. Grounded in Shear's own experience building Kiko, Justin.tv,
  and Twitch — including his own early failure to talk to users at all — not generic user
  research advice. Load this when a founder is deciding who to interview, has been burned by
  building a requested feature nobody used, is choosing where to focus limited research time,
  or is trying to get their team to actually believe what user research turned up. Drives a
  diagnostic conversation, but states a direct, opinionated take once there's enough context
  to support one — not purely Socratic.
tags: user-interviews, user-research, customer-discovery, feature-validation, non-users, competitor-users, horseless-carriage-effect, interview-technique, product-validation, buy-in, qualitative-research
source: "How to Run a User Interview," Emmett Shear, CS183B How to Start a Startup, Stanford 2014, Lecture 16, https://www.youtube.com/watch?v=qAws7eXItMk
---

## Overview

This skill is relevant when a founder is deciding who to talk to before building something,
has built a requested feature that nobody actually used, is trying to prioritize research time
across different groups of people, or needs to convince a skeptical team of what user research
found. Shear's central move is refusing to ask about features at all — interviews are for
understanding a person's actual problem and context, not for validating a solution the founder
already has in mind.

**Example situations where this skill is relevant:**
- "I don't know who to talk to before I start building this"
- "I asked users if they'd want feature X, they said yes, I built it, and nobody used it"
- "I have limited time — should I talk to my users, my competitors' users, or people who aren't using anything like this yet?"
- "I did a bunch of interviews but my cofounder/team doesn't believe the conclusions"
- "Should I run interviews over email to save time?"
- "We had early success talking to users, but growth is slowing and I'm not sure why"

This is not the right skill for deciding whether the underlying idea is worth pursuing at all
(`ideas/idea-and-product-altman.md`) or for the ongoing customer-support relationship once a
product has real usage (`product/building-for-love-hale.md`) — though the "don't ask about
features" principle connects directly to Hale's "stay away from asking if a feature is good."

## Assumptions

1. **The founder is trying to figure out what to build or why something isn't working**, not
   running usability testing on something already built. Shear draws this distinction
   directly — on-site feedback tools and usability tests are a different, later kind of
   research that irons out an existing design, not this kind.
2. **There's at least a rough idea or product direction to investigate.** The framework is
   about who to talk to and how, not about generating ideas from nothing.
3. **The person wants a direct opinion, not just questions.** Shear names specific mistakes
   plainly (asking about features, talking to whoever's convenient, interviewing over email)
   from his own repeated experience getting this wrong before getting it right.

## Insights

> "We built it, but we sold it on eBay — so that's not necessarily the end you want for your
> startup. We didn't know anything about calendars, neither of us used calendars, nor did we
> think during that period we've got to talk to anyone who actually did. We got the build-
> stuff part down. We did not get the talk-to-users part."
— Emmett Shear, CS183B Lecture 16, 2014, on his first startup, Kiko Calendar

Context: Shear opens with his own failure, not a success story — establishing that this isn't
abstract theory, it's a lesson he learned by building something nobody wanted first.

> "Who you talk to is as important as what questions you ask. If we'd gone and talked to
> viewers only, we'd have gotten a completely different set of feedback than talking to the
> broadcasters. People just follow the content — the broadcaster comes with it."
— Emmett Shear, CS183B Lecture 16, 2014, on identifying broadcasters as Twitch's key user

Context: The organizing claim of the entire talk. Shear is explicit there's no formula for
identifying the right person to talk to — it takes real judgment about who a product is
actually being built for, which is itself the first hard problem to solve.

> "One of the problems with selling things to college students is they don't actually spend
> very much money... the people most likely to actually buy a note-taking app would be
> college IT [administrators]... you might also talk to parents, who spend money on their
> kids' education."
— Emmett Shear, CS183B Lecture 16, 2014, from the live interview exercise

Context: A direct illustration that the "obvious" user (the person who'd use the product) and
the person whose interview actually matters (who pays, who decides) are often different people
— broadening who to consider talking to beyond the first obvious answer.

> "You want to stay as far away from features as possible, because the things people tell you
> wind up feeling overwhelmingly real. When a real user asks you for a feature, it's very hard
> to say no to them... but you get the horseless carriage effect — you're getting asked for a
> faster horse instead of the actual solution."
— Emmett Shear, CS183B Lecture 16, 2014

Context: Shear's core methodological warning. Feature requests from real, sympathetic people
carry emotional weight that makes them feel more valid than they are — the interview's job is
to find the underlying problem, not collect a feature backlog.

> "The one thing you really don't want to do is ask them: I've got this great idea for a
> feature, are you excited about it? The feedback you get is often 'oh yeah, that's great' —
> but when you actually build it, you find out that while they thought it was clever, no one
> actually cares enough to switch to get it."
— Emmett Shear, CS183B Lecture 16, 2014

Context: The specific trap this lecture is most focused on avoiding — asking "is this feature
good" produces false-positive enthusiasm that doesn't survive contact with an actual product.

> "The money test is amazing — it really does clarify whether they're really excited, because
> if you're not five-dollars-excited about it, you're probably not very excited about it."
— Emmett Shear, CS183B Lecture 16, 2014

Context: Offered as the strongest available validation signal, stronger than any stated
opinion — getting someone to commit money (even a small amount) tests real conviction in a way
enthusiasm in conversation doesn't.

> "People who are using your service already and are willing to put up with all these issues
> — kind of means these are probably not actually the biggest problems. If you're willing to
> ignore that you can't edit the ban list, and you're using the service anyway, maybe that
> isn't a huge problem."
— Emmett Shear, CS183B Lecture 16, 2014, on interviewing existing Twitch/Justin.tv broadcasters

Context: A genuinely counterintuitive read on existing-user feedback — the fact that someone
tolerates a limitation while continuing to use the product is itself evidence the limitation
isn't what's actually holding the product back.

> "The majority of people you're competing with are non-users — people who've never used your
> service or a competitor's. What they say is what blocks you from expanding the size of the
> market. If you only talk to yourself and your competitors' users, you can never expand it."
— Emmett Shear, CS183B Lecture 16, 2014

Context: The third and, per Shear, most overlooked interview group. Non-users reveal
structural blockers (a Korean esports player refusing to broadcast practice sessions for
competitive reasons; "my computer isn't fast enough") that existing users, by definition,
don't have.

> "We dumped almost all of our resources into things no one ever mentioned in an interview —
> but those addressed the underlying goals: people wanted money, stability, and universal
> access. We built a subscription program, invested in video stability, and got broadcasting
> built into the Xbox and PlayStation 4."
— Emmett Shear, CS183B Lecture 16, 2014

Context: The payoff of not building the literal features requested — Shear's team translated
requests (polls, chat features, child accounts) into the underlying goals behind them, and
built toward the goals instead.

> "Recording interviews is like magic. It stops you from taking notes mid-conversation, and
> you can play it back for the rest of the company. It's astonishing the influence it has on
> what people believe the right thing to build is."
— Emmett Shear, CS183B Lecture 16, 2014

Context: Shear's answer to "how do you get company buy-in for what you learned" — asserting a
conclusion is easy to disbelieve; playing the actual recording is not.

> "Email interviews are basically useless. The most interesting things come from 'huh, that's
> interesting, tell me more' — the instant someone says something you didn't expect, you drop
> into detective mode. People don't like silence, so they keep talking to fill the void."
— Emmett Shear, CS183B Lecture 16, 2014

Context: A specific mechanical claim about interview medium — live back-and-forth (Skype or in
person) enables the follow-up-on-surprise technique that written, asynchronous exchanges don't.

## Principles

1. **Decide who to talk to before deciding what to ask.** This is the first, hardest question
   for almost any startup — who the user actually is, and where to find them.
2. **The obvious user and the person whose feedback matters most are often different people.**
   Check who pays, who decides, and who's affected, not just who would use the product.
3. **Never ask if a feature is good, or whether someone would use it.** Sympathetic agreement
   in conversation doesn't predict switching behavior — it produces the horseless-carriage
   effect, not real signal.
4. **The strongest validation available is getting someone to commit money.** "Five-dollars-
   excited" is a real, higher bar than any stated opinion.
5. **Existing users who tolerate your product's flaws are giving you a signal about what
   doesn't actually matter, not a roadmap.** If they're using it anyway, the flaw likely isn't
   the real blocker.
6. **Competitors' users are often the fastest path to short-term wins** — they already have
   the target behavior; you only need to convince them to switch, which is easier than
   creating new behavior from nothing.
7. **Non-users are the group that reveals how to expand the market, not just win share.**
   They tell you the structural blockers that existing users, by definition, have already
   overcome or don't have.
8. **Translate requested features into underlying goals, then build toward the goals.**
   Nobody asked Twitch for "video stability" as a feature — they asked for reliability
   problems to go away, which is a goal, not a spec.
9. **Talking to whoever's convenient (existing forum members, etc.) produces weaker data than
   talking to who you actually need to reach.** Worth real effort (Shear's team spent weeks
   tracking down identities) to reach the right people, not just the reachable ones.
10. **Recorded interviews, played back, are dramatically more persuasive internally than
    summarized conclusions.** If a team doesn't believe research findings, the fix is often
    playback, not better argument.
11. **Interview medium matters — live conversation (Skype/in-person) enables following
    surprises; email doesn't.** The most valuable moments come from unscripted follow-up on
    something unexpected.
12. **Who you need to talk to shifts over time — stop doing this and your next features get
    worse.** Early-stage critical users are rarely the same people who matter years later.

## Where This Can Mislead You

- **"Never ask about features" can be over-applied to shut down any product-specific
  conversation.** Shear does eventually dig into specific behaviors (which tools someone uses
  and why, whether they review notes) — the rule is specifically about not pitching your own
  feature idea and asking for a verdict on it, not about avoiding all product-adjacent detail.
- **The "existing users tolerate flaws so they're not the real problem" read is a genuinely
  sharp insight, but it's not universal.** Some tolerated flaws are tolerated because users
  have no better option yet, not because the flaw is unimportant — worth checking whether
  there's a real alternative they're comparing against before concluding the flaw doesn't matter.
- **Focusing resource-constrained research on competitor users first (Shear's own choice at
  Twitch) was explicitly a short-term-growth-pressure decision** ("my project would've been
  killed without 25% month-over-month growth"), not a claim that competitor users are always
  the right first priority. Under different pressures, non-user research for market expansion
  might be more valuable earlier.
- **"Don't compensate people" worked for Shear's specific case** (people motivated by genuine
  interest in an emerging hobby/behavior). It doesn't generalize to every context — some
  populations worth reaching (busy professionals, hard-to-access experts) may require
  compensation to get real access, and refusing to pay may just mean talking to whoever's
  cheapest to reach rather than who's most important.
- **The international/language barrier point is presented as "just a hard problem," which is
  accurate — but the described workarounds (translators, bilingual proxies) are explicitly
  named as producing a non-representative sample.** Don't treat those workarounds as solving
  the problem; they're a partial mitigation Shear himself flags as imperfect.
- **6-8 people per segment "usually being enough" is a rule of thumb from Shear's specific
  categories (broadcasters, competitor users, non-users), not a universal sample-size law.**
  More heterogeneous or higher-stakes decisions may need more before patterns stabilize.

## Thinking Framework

**Deciding who to interview first**
Ask: "Who would actually use this — and separately, who pays for it, or decides whether it
gets adopted?" If those are different people (a note-taking app used by students but paid for
by IT or parents), name that split directly and recommend covering both, not just the obvious
user. Push for a broad first pass across several groups before narrowing — "you want to get
familiar with the space" before committing to one segment.

---

**Feature seems validated because a user asked for it, or agreed it was a good idea**
Ask: "Did they ask for this unprompted, or did you describe it and ask if they'd want it?" If
the latter: name the trap directly. "That's the exact pattern Shear warns against — agreement
in conversation doesn't predict switching. What's the smallest version you could actually put
in front of them, or the smallest commitment (even money) you could ask for instead?"

---

**Limited time, deciding which group to prioritize (existing users, competitor users,
non-users)**
Ask what the immediate pressure is — is it short-term growth, or understanding why the market
isn't bigger? If short-term growth: competitor users are the faster win, per Shear's own
Twitch decision — they already have the behavior, they just need convincing. If the question is
why growth has a ceiling: non-users are the group with the answer, and existing/competitor
users won't have it, almost by definition.

---

**Feedback from existing power users feels important but nothing's changing**
Ask: "Are they still using the product despite these complaints?" If yes: reframe directly —
"That's actually evidence these aren't the real blockers. What have people who tried it and
stopped said instead?" Redirect toward churned users or non-users rather than doubling down on
vocal current users.

---

**Team doesn't believe the research conclusions**
Ask: "Did you play them the actual interviews, or summarize what you heard?" If summarized:
recommend recording (with consent) and playing back the specific moments that drove the
conclusion — Shear's own fix for exactly this problem.

## Action Prompts

**Step 0: Get the specific situation**
If the founder hasn't said what they're deciding, ask: "What's the specific research question
right now — who to talk to, how to validate a specific feature idea, or getting buy-in on
what you found?"

**Step 1: Match to the right thread above** and go there directly.

**Step 2: State a plain view once you have enough context.** If a founder describes pitching
a feature idea and getting enthusiastic verbal agreement, say so directly: "That's the trap —
verbal enthusiasm for a pitched feature doesn't predict use. The next step is a real
commitment test, not another round of the same question."

## What Not To Do

- **Don't ask users whether a specific feature idea sounds good.** Ask about their current
  behavior and problems instead, and infer from there.
- **Don't treat existing users' feature requests as the roadmap.** Read between the lines for
  the underlying goal, and check whether the request is something they tolerate rather than
  something that's actually blocking them.
- **Don't default to interviewing whoever's easiest to reach.** If the right people take real
  effort to find, that effort is usually worth it.
- **Don't run interviews over email if a live conversation is possible.** The follow-up-on-
  surprise technique that produces the best insight requires real-time back and forth.
- **Don't rely only on your own or your competitors' existing users when trying to understand
  why a market isn't bigger.** That question's answer lives with non-users specifically.
- **Don't assume six interviews from one group generalizes to a different group.** Different
  segments (students vs. IT admins vs. parents; broadcasters vs. non-broadcasters) produce
  meaningfully different answers — deliberately sample across extremes, not just within one.

## Related Skills

Deciding what to build once a signal is found connects directly to
`ideas/idea-and-product-altman.md` (especially the love-vs-like framing) and
`product/building-for-love-hale.md` (especially "don't ask if a feature is good," which
Hale's Q&A makes the same point about). Cofounder and early-team decisions that shape who's
available to run this kind of research are `hiring/team-and-cofounders-altman.md`.
