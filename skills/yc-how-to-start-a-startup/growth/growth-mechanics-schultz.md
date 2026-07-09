---
name: Growth — Alex Schultz
description: |
  Applies Alex Schultz's framework for growth — retention as the single metric that
  determines whether growth tactics are even worth attempting, the retention-curve test for
  real product-market fit, why startups shouldn't have a dedicated growth team (the whole
  company should be), setting a company-wide "north star" metric, designing toward the
  product's specific "magic moment," and concrete tactics (virality's payload/frequency/
  conversion model, K-factor, SEO, and email/SMS/push deliverability). Grounded in Schultz's
  own experience building growth at eBay and Facebook, including his own early SEO and
  keyword-research mistakes — not generic growth-hacking advice. Load this when a founder is
  wondering whether they're ready for growth tactics at all, deciding whether to hire a growth
  team, choosing a north star metric, trying to identify their product's magic moment,
  evaluating whether a viral mechanic will actually work, or debugging weak SEO/email
  performance. Drives a diagnostic conversation, but states a direct, opinionated take once
  there's enough context to support one — not purely Socratic.
tags: retention, product-market-fit, north-star-metric, growth-team, magic-moment, virality, k-factor, seo, email-deliverability, marginal-user, cohort-analysis, growth-tactics
source: "Growth," Alex Schultz, CS183B How to Start a Startup, Stanford 2014, Lecture 6, https://www.youtube.com/watch?v=vJqlG5ytLDs
---

## Overview

This skill is relevant when a founder is wondering whether they're ready for growth tactics at
all, deciding whether to hire a growth team, choosing a company-wide north star metric, trying
to identify their product's "magic moment," evaluating a viral mechanic, or debugging weak
SEO or email/notification performance. Schultz's central, load-bearing claim is that almost
everything people call "growth hacking" is irrelevant if retention isn't already real — and
that most founders who think they have product-market fit don't yet.

**Example situations where this skill is relevant:**
- "We're not growing fast enough — should we hire a growth hacker or a growth team?"
- "I don't know if our retention is actually good or if I'm fooling myself"
- "What metric should our whole company be rallying around?"
- "I built a referral/viral mechanic but I'm not sure if it'll actually work"
- "Our SEO traffic is flat despite a lot of effort"
- "Our email open rates are terrible" / "should we send more marketing emails?"

This is not the right skill for validating the initial idea or building the MVP
(`product/mvp-and-users-cheung.md`), or for the earliest pre-product-market-fit hustle of
finding first users (`growth/unscalable-things-williams-tang.md`). A related but distinct
growth framework from a different speaker is `growth/growth-mechanics-cheung.md`.

## Assumptions

1. **The question is about scaling growth on top of a real product**, not about whether the
   idea itself is any good. Schultz is explicit that growth tactics applied to a product
   without real retention are close to worthless.
2. **The founder has, or can get, real usage data** — day-N retention by cohort, at minimum.
   Some of this framework (the retention curve test specifically) requires actual numbers, not
   just intuition.
3. **The person wants a direct opinion, not just questions.** Schultz states blunt, sometimes
   provocative claims (startups shouldn't have growth teams; newsletters are "stupid") backed
   by specific numbers from his own time at eBay and Facebook.

## Insights

> "What matters most for growth? ...Retention. Retention is the single most important thing
> for growth. We have a fantastic product [at Facebook] — if we can get people on and ramped
> up, they stick."
— Alex Schultz, CS183B Lecture 6, 2014

Context: Schultz elicits this from the room rather than stating it first — deliberately, since
the answer (retention, not virality or paid acquisition) is the one thing every other growth
tactic depends on.

> "If you look at percent monthly active versus number of days from acquisition, and your
> retention curve asymptotes to a line parallel to the x-axis, you have a viable business and
> product-market fit for some subset of market. But most companies that fly up and talk about
> growth hacking and virality — their retention curve slopes down and eventually intercepts
> the x-axis."
— Alex Schultz, CS183B Lecture 6, 2014

Context: The single diagnostic Schultz returns to throughout the talk — plot day-N retention
by cohort (works with as few as ~10,000 users) and check whether the curve flattens or decays
to zero. He used this exact methodology to predict Facebook's B2B advertiser lifetime value to
97% accuracy using only 90 days of a brand-new product's data.

> "If it doesn't flatten out, don't go and do growth tactics. Don't do virality. Don't hire a
> growth hacker. Focus on getting product-market fit. The number one problem I've seen inside
> Facebook for new products, and the number one problem I've seen for startups I've advised,
> has been they don't actually have product-market fit when they think they do."
— Alex Schultz, CS183B Lecture 6, 2014

Context: A direct, blunt diagnosis of the most common mistake he sees — reaching for growth
tactics as a fix for a retention problem that only a better product can actually solve.

> "Different verticals need different terminal retention rates. If you're in e-commerce and
> retaining 20-30% of users monthly, you're probably doing pretty well. If you're in social
> media and your first batch isn't like 80% retained, you're not going to have a massive
> social media site."
— Alex Schultz, CS183B Lecture 6, 2014

Context: Directly answers "what counts as good retention" — there's no universal number; the
bar is set by what comparable, successful companies in the same vertical actually achieve, not
by an absolute standard.

> "Startups should not have growth teams. The whole company should be the growth team. The
> CEO should be the head of growth. You need someone to set a north star — Mark published
> monthly active users, both internally and externally, as the number he held the whole company
> to. WhatsApp published sends. Airbnb talks about nights booked. eBay optimized for gross
> merchandise volume, not revenue, even though outsiders judged them on revenue."
— Alex Schultz, CS183B Lecture 6, 2014

Context: Schultz's argument for why a single, leadership-defined metric matters: the moment a
company has more than one person, the founder can't control what everyone does — only what
they collectively believe matters. Most plausible north star metrics correlate with each other
anyway, so the specific choice matters less than everyone actually rallying around one.

> "Registrations don't matter unless they become long-term active users. At eBay, we changed
> affiliate payment from confirmed registered users to activated confirmed registered users.
> We lost 20% of registered users overnight — but active users only dropped 5%, and active-user
> growth massively accelerated."
— Alex Schultz, CS183B Lecture 6, 2014

Context: The mechanism: paying for mere registration lands people on a signup page before
they've seen anything worth wanting; paying for activation lands them on the actual product
(search results for what they wanted), which produces real engagement instead of empty signups.

> "The magic moment for Facebook is that first time you see a friend's face — that's why we
> focused on getting people to 10 friends in 14 days. Look at LinkedIn's, Twitter's, or
> WhatsApp's registration flow — the number one thing they all try to do is get you connected
> to the people you want as fast as possible, because in this vertical, that's what matters."
— Alex Schultz, CS183B Lecture 6, 2014

Context: The "magic moment" is the specific experience that converts a new signup into someone
who understands, viscerally, why the product matters — Schultz argues every registration flow
should be redesigned around reaching it as fast as possible, not around collecting more signup
information first.

> "Everyone in the Valley gets this wrong: we optimize for ourselves. My favorite example is
> notifications — every company says 'I'm getting too many notifications, that's what we need
> to fix.' Are your power users leaving because of too many notifications? No. What you need
> to focus on is the marginal user — the one who doesn't get a notification and forgets you
> exist."
— Alex Schultz, CS183B Lecture 6, 2014

Context: A direct corrective against designing growth decisions around the founder's or team's
own experience of the product — the people making the decisions are almost never the marginal
users whose behavior the decision is actually meant to move.

> "Virality has three parts: payload (how many people you can hit with one blast), frequency
> (how many times you can hit them), and conversion rate. Hotmail was low payload, high
> frequency, high conversion. PayPal was low payload, low frequency, but extremely high
> conversion — you were literally offering to send someone money. Facebook was not viral via
> sharing mechanics at all — it grew through word of mouth, because there was no native way to
> contact people who weren't already on the service."
— Alex Schultz, CS183B Lecture 6, 2014

Context: A framework for diagnosing why a specific viral mechanic does or doesn't work,
illustrated with three real examples that succeeded through different combinations of the
three variables — plus a direct correction of the common misconception that Facebook itself
grew "virally" in the mechanical sense.

> "I spent a year optimizing my cocktail site to rank for 'cocktail making.' Turns out in the
> UK, about 500 people a month search that. Everyone searches 'cocktail recipes' — and in the
> US, the biggest market, everyone searches 'drink recipes.' I dominated the wrong search term.
> When we fixed one thing at Facebook — adding a directory so Google could reach every public
> profile page — we 100x'd SEO traffic overnight."
— Alex Schultz, CS183B Lecture 6, 2014

Context: Two SEO lessons from direct, costly personal experience — keyword research has to
precede optimization effort (supply, demand, and value, not intuition about what people search
for), and internal link structure can matter more than any single content decision.

## Principles

1. **Retention is the prerequisite for every other growth tactic, not one tactic among many.**
   Plot day-N retention by cohort; if the curve doesn't flatten, fix the product before
   attempting virality, paid acquisition, or hiring a growth specialist.
2. **"Good retention" is vertical-specific, not a universal number.** Benchmark against
   comparable successful companies in your specific category, not an absolute standard.
3. **Startups shouldn't have a growth team — the whole company should function as one**, led
   directly by the CEO, because growth is fundamentally a coordination problem that only
   leadership-level authority can solve once more than one person is involved.
4. **Pick one company-wide north star metric and hold everyone to it.** The specific choice
   matters less than the fact that it's singular and everyone actually believes it's the thing
   that matters — most plausible candidates correlate with each other anyway.
5. **Registrations are worthless without activation.** Optimize acquisition spend and
   affiliate/referral payment for the behavior that actually predicts long-term value, not the
   easiest-to-measure proxy.
6. **Every product has a specific "magic moment" — the experience that makes a new user
   understand why it matters.** Redesign onboarding to reach it as fast as possible, ahead of
   anything else.
7. **Optimize growth decisions for the marginal user, not for yourself or your power users.**
   The people making product decisions are systematically unrepresentative of the users whose
   behavior those decisions are meant to change.
8. **Virality breaks down into payload, frequency, and conversion rate — diagnose which one is
   actually driving (or missing) in a specific mechanic**, rather than treating "virality" as
   one undifferentiated property a product either has or doesn't.
9. **A viral mechanic with a K-factor over 1 is worthless without retention behind it.**
   Getting the viral loop working is a wasted effort if users don't stick around once acquired.
10. **SEO keyword research has to be based on actual search data, not intuition about what
    people search for.** Confusing your own vocabulary for your users' is an easy, costly
    mistake even for someone technically skilled at SEO mechanics.
11. **Email, SMS, and push all live or die on deliverability first, relevance second.** Being
    flagged as spam or abusing opt-outs destroys the channel permanently; beyond that,
    triggered/notification-based messaging beats generic newsletters because different users
    at different stages need different messages.
12. **Hard work and fast execution are a real, underrated growth advantage.** Schultz
    attributes Facebook's growth-team era success significantly to intensity and iteration
    speed, not superior tactics or intelligence.

## Where This Can Mislead You

- **"Don't do growth tactics if retention isn't there" can be misapplied as "never experiment
  with growth until retention is perfect."** Schultz's own example (the eBay affiliate payment
  change) is itself a growth tactic applied while retention was already real but improvable —
  the rule is about sequencing relative to genuine product-market fit, not a ban on any growth
  work before perfection.
- **The retention-curve asymptote test needs real cohort data to run — it can be attempted
  with rough numbers on a small user base (Schultz says ~10,000 is enough to get a usable
  signal), but a founder with only a handful of users doesn't yet have enough data for this
  specific diagnostic to be reliable.** Don't apply it to too small a sample and treat the
  result as conclusive.
- **"Startups shouldn't have growth teams, the whole company should be the growth team" is
  Schultz's view from Facebook's own specific history** (a growth team was in fact created
  there once they hit a real, painful growth plateau around 50-100 million users). The claim
  is about not treating growth as a siloed specialist function *instead of* company-wide
  focus — not a claim that dedicated growth roles or teams never make sense once a company
  has genuinely outgrown ad hoc coordination.
- **Picking "almost any" north star metric because they're correlated is true directionally,
  but not a license to pick a metric carelessly.** eBay's specific choice (gross merchandise
  volume over revenue) mattered because it prevented a specific wrong optimization (favoring
  categories with better margins over overall marketplace health) — the correlation claim
  doesn't mean the choice is inconsequential in every case.
- **The virality payload/frequency/conversion framework explains why past viral mechanics
  worked — it's a diagnostic lens, not a guarantee a new mechanic modeled on Hotmail or PayPal
  will work the same way today.** Distribution environments (email norms, platform policies)
  have changed substantially since those examples.
- **"Email is dead for people under 25" is Schultz's 2014 read on a specific demographic and
  is explicitly time- and audience-bound** — he says directly it's different for an older
  audience. Don't apply it as a blanket rule regardless of target demographic or how
  communication norms may have shifted since.

## Thinking Framework

**Deciding if you're ready for growth tactics**
Ask: "Have you plotted day-N retention by cohort — does the curve flatten, or does it decay
toward zero?" If they haven't measured this: that's the actual next step, not premature
optimization. If it decays toward zero: say so directly — "That's the signal Schultz says
means focus on product-market fit, not growth tactics, no matter how tempting virality or paid
acquisition looks right now."

---

**Choosing whether to build a growth team**
Ask: "Is the whole company already oriented around one specific metric everyone believes
matters?" If not: that's the more urgent gap — recommend defining and communicating a single
north star before considering a dedicated team. If yes, and the company has genuinely outgrown
ad hoc coordination on growth specifically: a dedicated team may be the right next step, but
name that this is closer to Facebook's own later-stage decision than the advice for an early
startup.

---

**Picking a north star metric**
Ask: "What's the one thing that, if everyone optimized toward it, would mean the company is
genuinely healthy — not just busy?" Push past registration/signup counts specifically — ask
what the activated, sustained version of that number would be. Reference the eBay GMV-vs-
revenue and WhatsApp-sends examples as illustrations of picking the metric that resists the
wrong optimization, not just the most visible one.

---

**Identifying the product's magic moment**
Ask: "What's the first specific moment when a brand-new user actually understands why this
matters — not what they see, what they feel?" Push for something concrete and specific (like
"seeing a friend's photo," not "using the core feature"). Then ask how many steps of the
current onboarding happen before that moment, and whether any of them could move after it.

---

**Evaluating a viral mechanic**
Ask about all three variables directly: "How many people does one action reach, how often can
you repeat it, and what's the actual conversion rate at each step?" If they've only estimated
payload (e.g., "everyone imports their whole contact list"): push for the realistic
conversion-rate chain (import → invite → click → signup → import again) to get an actual
K-factor estimate. Then ask the more important question: "Is there real retention behind this
yet?" A K-factor over 1 without retention is not a reason to proceed.

---

**Debugging weak SEO or email performance**
For SEO: ask "What specific keyword data did you use to choose what to optimize for?" If the
answer is intuition rather than actual search volume research: name the cocktail-site mistake
directly. For email: ask "Is this a newsletter sent to everyone, or a notification/trigger
based on where someone is in their specific journey?" If it's a blanket newsletter: recommend
segmenting by engagement/lifecycle stage instead.

## Action Prompts

**Step 0: Get the specific situation**
If the founder hasn't said what they're deciding, ask: "What's the specific growth question
right now — whether you're ready for growth tactics, choosing a north star, a viral mechanic,
or SEO/email performance?"

**Step 1: Match to the right thread above** and go there directly.

**Step 2: State a plain view once you have enough context.** If a founder describes wanting
to hire a growth hacker while their retention curve is still decaying to zero, say so directly:
"That's exactly the pattern Schultz calls the number one problem he's seen — the fix is product-
market fit, not a growth hire."

## What Not To Do

- **Don't let a founder pursue virality or paid acquisition before checking whether retention
  is real.** Redirect to the retention-curve test first, every time.
- **Don't accept a single, universal "good retention" number.** Push for the specific
  vertical's comparable benchmark instead.
- **Don't recommend a siloed growth team as the default fix for slow growth at an early-stage
  company.** Push for company-wide north-star alignment first.
- **Don't let registration/signup counts stand in as the success metric without checking
  activation.** Ask what the activated version of that number actually looks like.
- **Don't accept a founder's own experience of the product as representative of the marginal
  user's experience.** Redirect decisions toward the low-engagement user specifically.
- **Don't treat a high K-factor as sufficient justification to invest further in a viral
  mechanic.** Check for real retention underneath it first.

## Related Skills

Validating the idea and building the MVP, prior to any of this, is
`product/mvp-and-users-cheung.md`. A related but distinct growth framework — sticky/viral/paid
growth types, CLV/CAC, and the pivot decision — is `growth/growth-mechanics-cheung.md`. The
earliest pre-retention hustle for first users is `growth/unscalable-things-williams-tang.md`.
Recovering momentum once growth has stalled, from a different angle, is
`operations/execution-altman.md`.
