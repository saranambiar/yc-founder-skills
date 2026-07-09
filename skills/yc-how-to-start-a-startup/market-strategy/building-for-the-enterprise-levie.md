---
name: Building for the Enterprise — Aaron Levie
description: |
  Applies Aaron Levie's framework for building an enterprise software company — why the
  enterprise/consumer choice isn't the tradeoff founders assume, the structural shifts (cloud,
  standardized platforms, user-led IT adoption) that changed what's possible in enterprise
  software, and concrete tactical patterns: starting with an intentionally small wedge,
  finding asymmetries incumbents can't or won't copy, seeking out bleeding-edge customers, and
  translating customer requests into the right solution instead of building exactly what's
  asked. Grounded in Box's own founding story — including the specific value-mismatch that
  forced Levie's team to choose a direction — not generic enterprise-sales advice. Load this
  when a founder is deciding between consumer and enterprise, has a product that's simultaneously
  too much for consumers and too little for enterprises, looking for a wedge into an
  enterprise market dominated by incumbents, or trying to figure out how much to build exactly
  what enterprise customers ask for. Drives a diagnostic conversation, but states a direct,
  opinionated take once there's enough context to support one — not purely Socratic.
tags: enterprise-software, b2b, wedge-strategy, incumbent-asymmetry, user-led-adoption, cloud-shift, consumer-vs-enterprise, feature-requests, platform-vs-custom, enterprise-sales, bleeding-edge-customers
source: "Building for the Enterprise," Aaron Levie, CS183B How to Start a Startup, Stanford 2014, Lecture 12, https://www.youtube.com/watch?v=tFVDjrvQJdw
---

## Overview

This skill is relevant when a founder is deciding between consumer and enterprise, stuck with
a product that's simultaneously overbuilt for consumers and underbuilt for enterprises,
looking for a wedge into a market with entrenched incumbents, or unsure how literally to build
what enterprise customers ask for. Levie's account is grounded in Box's own founding crisis —
they didn't set out to build enterprise software, and were forced to choose a direction when
their product turned out wrong for both markets at once.

**Example situations where this skill is relevant:**
- "Should we go after consumers or enterprises with this?"
- "We have paying users, but our product feels like it's for nobody in particular"
- "There's a huge incumbent in this space — how could we possibly compete?"
- "An enterprise customer is asking for a very specific feature — should we build exactly that?"
- "We're a two-person company — can we realistically sell to large enterprises at all?"
- "Should our product be self-serve, or do we need a sales team?"

This is not the right skill for evaluating market structure and monopoly characteristics in
general (`market-strategy/competition-monopoly-thiel.md`, which this skill's wedge/asymmetry
thinking directly complements) or for translating user feedback into product decisions outside
an enterprise context (`user-research/user-interviews-shear.md`, `product/mvp-and-users-cheung.md`).

## Assumptions

1. **The founder is considering, or already building, a product with enterprise customers**,
   not purely consumer. Some of this framework (platform vs. custom, sales alongside
   self-serve) is specific to the enterprise buying and adoption motion.
2. **The company is early enough that market positioning is still a live decision.** Levie's
   own story is about a genuine fork in the road, not a retrospective justification of an
   unchangeable choice.
3. **The person wants a direct opinion, not just questions.** Levie states specific,
   sometimes counterintuitive claims (start intentionally small even though incumbents will
   dismiss you; don't build exactly what customers ask for) from Box's own founding decisions.

## Insights

> "For consumers, we had built a very comprehensive product — more functionality than a
> consumer wanted. For enterprises, we had built too insignificant a product — not enough
> security, not enough of what enterprises wanted from their data. We found ourselves at this
> juncture where we had to choose."
— Aaron Levie, CS183B Lecture 12, 2014

Context: The actual crisis that forced Box to pick a direction — not an abstract strategic
choice, but the discovery that trying to serve both markets with one product satisfied
neither.

> "In the consumer world, there's about $170 billion combined in app purchases and digital
> advertising. In enterprise, there's $3.7 trillion spent on IT every single year. Consumers
> are trying to conserve a limited amount of money. Enterprises are trying to increase
> productivity and get higher performance — the value equation is completely different."
— Aaron Levie, CS183B Lecture 12, 2014

Context: Levie's case for why enterprise's total spend and value logic — buyers optimizing for
what technology gets them, not minimizing what they spend — makes it a fundamentally different
opportunity than consumer, not simply a harder, less fun version of the same game.

> "There are only two moments of opportunity for a technology revolution in the enterprise:
> the raw materials change — cost of computing drops, so it becomes better to centralize and
> deliver on demand — or customers' own expectations change. If you're in shipping or
> logistics, Uber represents a massive change to your industry whether you like it or not."
— Aaron Levie, CS183B Lecture 12, 2014

Context: A framework for spotting enterprise opportunity broadly — either the underlying
technology economics shift (enabling new categories) or end-customer behavior shifts elsewhere
force every business in an industry to need new capability, whether or not they wanted to change.

> "It used to be that you could only sell to the top five or ten thousand companies in the
> world — only they had the budget and infrastructure to deploy your technology. Today, a
> two-person company can sign up for Box, and General Electric, with 300,000 employees, can
> too. The IT model has become user-led rather than IT-led — and in an IT-led world,
> incumbents generally win, because they already have the relationship with the CIO."
— Aaron Levie, CS183B Lecture 12, 2014

Context: The structural shift Levie identifies as most important — cloud and mobile made it
possible for a small startup to get adopted by individual users first, and expand into a real
enterprise sale later, bypassing the incumbent relationship advantage that used to be decisive.

> "Spot technology disruptions: look for a wide gap between how things have been done and how
> they now can be done. PlanGrid noticed that $4 billion a year was spent printing and
> updating construction blueprints — and realized the iPad was the perfect vector to make that
> obsolete. That's the pattern: something impossible or impractical years ago becomes very
> practical once an enabling technology shows up."
— Aaron Levie, CS183B Lecture 12, 2014

Context: The first of Levie's tactical patterns — look specifically for the widest gap between
current practice and current technical possibility, since that gap is where the opportunity is
largest.

> "Start intentionally small. You can't compete with an incumbent on the full solution — find
> the wedge that slips into the gaps of existing products. ZenPayroll took just the one slice —
> payroll for small businesses — that was most painful, and only later expanded up-market.
> Incumbents look at something that small and dismiss it. That's exactly the point."
— Aaron Levie, CS183B Lecture 12, 2014

Context: A direct argument for deliberately narrow initial scope in enterprise specifically —
being dismissed by incumbents as too small is a feature of a good wedge, not a warning sign.

> "Find asymmetries — do things incumbents can't or won't do, because the economics don't work
> for them or because they're technically locked in. If you're competing with a suite vendor
> who wants everything vertically integrated, build platform-agnostic technology instead.
> Zenefits doesn't charge the small business for their HR software at all — they get paid by
> commission from the insurance companies, a business model no traditional software company
> could copy without abandoning their own."
— Aaron Levie, CS183B Lecture 12, 2014

Context: Two distinct kinds of asymmetry — technical (architecture an incumbent's own product
line prevents them from copying) and economic (a business model an incumbent can't adopt
without cannibalizing their existing revenue).

> "Find customers at the bleeding edge of their industry and work with them as early adopters —
> what Paul Graham calls living in the future. Skycatch builds enterprise drones for
> construction, farming, and oil and gas — industries not known for high tech — by finding the
> specific organizations at the edge of their industry and discovering what's missing from how
> they already operate."
— Aaron Levie, CS183B Lecture 12, 2014

Context: A sourcing strategy for early enterprise adopters — instead of guessing what an
industry needs abstractly, find the specific organizations already pushing the edge of what's
normal in that industry and learn directly from what's still missing for them.

> "Listen to your customers, but don't always build exactly what they're telling you. Your job
> is to distill their requests into the best and simplest solution — not to build exactly what
> they ask for. Palantir does this with very complex problems: they translate them into simple
> solutions the customer wouldn't have known how to ask for."
— Aaron Levie, CS183B Lecture 12, 2014

Context: A direct warning against literal feature-request fulfillment in enterprise contexts
specifically — echoing a pattern that shows up across multiple lectures in this repo: the
stated request is rarely the best solution to the real underlying problem.

> "Keep consumer DNA at the center of the product — it makes adoption easier and gives you a
> real chance at going viral inside an organization. But your product selling itself doesn't
> mean you don't need salespeople. You'll still want consultative, domain-oriented sales to
> help customers navigate your product and the competitive landscape — just don't let sales
> become a substitute for building a great product."
— Aaron Levie, CS183B Lecture 12, 2014

Context: A direct rejection of the false choice between product-led and sales-led motion —
Levie's own example, Mixpanel, enters through individual developers self-serving, then expands
the account through inside sales, using both simultaneously rather than picking one.

## Principles

1. **The enterprise/consumer choice isn't "fun vs. hard" — it's a fundamentally different
   value equation.** Enterprises optimize for what technology gets them, not for minimizing
   spend, which changes what pricing and positioning actually work.
2. **A product that's simultaneously too much for consumers and too little for enterprise is a
   forcing function, not a temporary inconvenience.** It usually means a real choice about
   direction can't be deferred any longer.
3. **Structural shifts (cloud economics, standardized/open platforms, user-led IT adoption)
   determine when entering enterprise software is actually viable for a startup** — not just
   whether the idea itself is good.
4. **User-led adoption is the mechanism that lets startups bypass the incumbent relationship
   advantage.** In an IT-led world, existing vendor relationships decide; in a user-led world, a
   good product can get adopted from the bottom up before the enterprise sale even happens.
5. **Look for the widest gap between current practice and current technical possibility** —
   that gap is where the largest opportunities concentrate, and it recurs across industries as
   enabling technology changes.
6. **Start intentionally small and expect to be dismissed by incumbents for it.** You can't
   compete with an incumbent's full solution — the wedge has to be narrow enough to slip
   between existing products, with room to expand later.
7. **Look for asymmetries incumbents can't copy — technical lock-in or a business model that
   would cannibalize their existing revenue** — not just a better version of what they already do.
8. **Source early enterprise adopters from the bleeding edge of an industry**, not from
   guessing abstractly what an industry needs — the organizations already pushing boundaries
   reveal what's actually missing.
9. **Translate customer requests into the underlying problem and the simplest real solution —
   don't build literally what's asked.** This pattern shows up across multiple lectures in this
   repo (Cheung's Frankenstein warning, Shear's feature-request trap) and is especially acute
   in enterprise, where requests often come wrapped in organizational complexity.
10. **Modularize with open platforms and APIs rather than building every custom vertical need
    directly into the core product.** This scales better than bespoke customization per customer.
11. **Product-led and sales-led motion aren't mutually exclusive.** Keep consumer-grade product
    quality for adoption and virality, but still invest in consultative sales — sales
    complements a great product; it doesn't substitute for one.

## Where This Can Mislead You

- **"Start intentionally small" and "incumbents will dismiss you" can be misread as
  reassurance that any small, dismissed idea will eventually expand.** Levie's examples
  (ZenPayroll, Box itself) succeeded because the narrow wedge solved a real, sharply painful
  problem with a clear expansion path — smallness and being underestimated are not
  themselves the source of value; they're just what a real wedge often looks like from outside.
- **The "find asymmetries" framework can be used to justify almost any unconventional
  business model as "an asymmetry incumbents can't copy."** Zenefits' insurance-commission
  model worked because it was a genuinely sustainable, structurally different revenue
  source — not because being different from the incumbent's model is inherently valuable on
  its own. Check that the asymmetry is actually durable, not just currently uncopied.
- **"Don't build exactly what customers ask for" is not license to ignore customer requests or
  substitute the founder's own preferences for their stated problems.** The point, as with
  Cheung's and Shear's versions of this same idea, is to dig into the underlying problem behind
  the request — not to override it with something the founder simply prefers to build.
- **The specific structural shifts Levie names (cloud, mobile, user-led IT) were the enabling
  conditions of 2014.** The underlying method — look for what's newly possible that wasn't
  before — is durable; the specific list of enabling technologies will be different in any
  other period, and should be re-derived rather than assumed to still be the live opportunity.
- **"Keep consumer DNA, but you'll still need sales" is Levie's own resolved position after
  initially fearing sales entirely (the "Chuck with a briefcase" anxiety) — it's not a claim
  that every enterprise company needs the same mix of product-led and sales-led motion.** The
  right balance depends on deal size, buyer complexity, and how self-explanatory the product
  actually is; Box's specific mix isn't a universal ratio.

## Thinking Framework

**Deciding between consumer and enterprise**
Ask: "What's the actual value equation for your specific users — are they trying to minimize
spend, or trying to maximize what they get out of technology?" If it's genuinely ambiguous:
that's worth resolving before building further, using Levie's own value-equation framing
directly. If the founder is choosing based on which sounds more fun or exciting: name that
directly as a weak basis for the decision.

---

**Product feels overbuilt for consumers, underbuilt for enterprise**
Ask: "If you had to fully commit to one side within the next month, which would it be — and
what would you strip out or add?" Don't let this sit unresolved; Levie's own experience is that
trying to serve both produces a product that satisfies neither. Push for an actual decision,
not further feature accumulation on both sides.

---

**Facing an entrenched incumbent**
Ask: "What's the narrowest wedge you could own completely that the incumbent would dismiss as
too small to bother with?" Then: "What can you do that they structurally can't — either
technically, or without cannibalizing their own business model?" Push for a specific, concrete
answer to both, not a general sense of being "more nimble" or "more modern."

---

**Enterprise customer asks for a specific feature**
Ask: "What's the underlying problem behind that specific request?" Don't let the founder jump
straight to a build decision. Reference the Palantir example directly if useful — the goal is
the simplest real solution to the underlying problem, which is often not the literal feature
requested.

---

**Deciding on product-led vs. sales-led motion**
Ask: "Is your product self-explanatory enough that a user could get real value without any
human help, and does the deal size justify consultative sales on top of that?" If both are
true: recommend combining both, as Levie describes with Mixpanel, rather than treating this as
an either/or choice.

## Action Prompts

**Step 0: Get the specific situation**
If the founder hasn't said what they're deciding, ask: "What's the specific enterprise
question right now — consumer vs. enterprise, competing with an incumbent, a feature request,
or your sales motion?"

**Step 1: Match to the right thread above** and go there directly.

**Step 2: State a plain view once you have enough context.** If a founder describes building
a feature exactly as an enterprise customer specified without asking why, say so directly:
"That's the trap Levie warns about — worth digging into the underlying problem before
committing to that specific build."

## What Not To Do

- **Don't let "enterprise sounds hard, consumer sounds fun" drive the market choice.** Push
  for the actual value-equation comparison instead.
- **Don't validate a product trying to serve both consumer and enterprise needs
  simultaneously without forcing a real decision.** Name the value-equation mismatch directly.
- **Don't treat being dismissed by an incumbent as evidence the idea is too small to matter.**
  That's often exactly the signal a real wedge produces.
- **Don't build a literal feature request without asking what problem is actually behind it.**
  This applies with extra force in enterprise, where requests often carry organizational
  complexity that obscures the real need.
- **Don't recommend abandoning sales just because the product is well-designed and self-serve
  friendly.** The two aren't a substitute for each other in most enterprise contexts.
- **Don't treat any unconventional business model as a durable "asymmetry" without checking
  whether it's actually structurally hard for an incumbent to copy**, versus just currently
  uncommon.

## Related Skills

Market structure and monopoly characteristics generally, which this skill's wedge and
asymmetry thinking directly extends into an enterprise-specific context, is
`market-strategy/competition-monopoly-thiel.md`. The pattern of translating customer requests
into underlying problems appears also in `product/mvp-and-users-cheung.md` (the Frankenstein
warning) and `user-research/user-interviews-shear.md` (never ask if a feature is good).
