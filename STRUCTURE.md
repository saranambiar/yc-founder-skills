# founder-skills — Repo Structure & Conventions

Always read this before creating, moving, or renaming any skill file. Read `NORTH_STAR.md`
first — every convention here is in service of that standard.

---

## Folder structure

```
founder-skills/
├── CLAUDE.md                          ← project instructions, always read first
├── STRUCTURE.md                       ← this file
├── README.md                          ← user-facing intro and usage guide
├── llms.txt                           ← agent discovery index (one line per skill)
├── NORTH_STAR.md                       ← the standard every skill file is judged against
├── EXTRACTION_RUBRIC.md               ← how to turn a transcript into a skill file
├── skill-rubrics.md                   ← quality standards for evaluating skill output
├── plans/
│   └── product-skill-pipeline.md     ← execution plan for building skills
├── scripts/
│   └── install.py                    ← pip CLI stub (Phase 2)
├── .github/
│   └── CONTRIBUTING.md               ← contribution guide (Phase 2)
└── skills/
    └── yc-how-to-start-a-startup/
        ├── market-strategy/
        │   ├── competition-monopoly-thiel.md        ← BUILT (Lecture 5, Thiel)
        │   └── enterprise-disruption-levie.md       ← TODO (Lecture 12, Levie)
        ├── ideas/
        │   ├── idea-and-product-altman.md           ← BUILT (Lecture 1, Altman — idea/product half)
        │   ├── why-start-a-startup-moskovitz.md      ← BUILT (Lecture 1, Moskovitz — motivation half)
        │   └── counterintuitive-startups-graham.md  ← TODO (Lecture 3, Graham)
        ├── product/
        │   ├── mvp-and-users-cheung.md              ← TODO (Lecture 4, Cheung)
        │   └── building-for-love-hale.md            ← TODO (Lecture 7, Hale)
        ├── growth/
        │   ├── growth-mechanics-schultz.md          ← TODO (Lecture 6, Schultz)
        │   └── unscalable-things-williams-kan-tang.md ← TODO (Lecture 8, Williams/Kan/Tang)
        ├── hiring/
        │   ├── team-and-cofounders-altman.md        ← BUILT (Lecture 2, Altman — team/hiring half)
        │   ├── culture-chesky-lin.md                ← TODO (Lecture 10, Chesky/Lin)
        │   ├── scaling-teams-collison-silbermann.md ← TODO (Lecture 11, Collison/Silbermann)
        │   └── great-founder-hoffman.md             ← TODO (Lecture 13, Hoffman)
        ├── fundraising/
        │   ├── what-investors-want-andreessen-conway.md ← BUILT (Lecture 9, Andreessen/Conway/Conrad)
        │   └── pitching-seibel-bosmeny-caldwell.md  ← TODO (Lecture 19, Seibel/Bosmeny/Caldwell)
        ├── sales/
        │   └── early-sales-bosmeny.md               ← TODO (Lecture 19, Bosmeny — sales portion)
        ├── operations/
        │   ├── execution-altman.md                  ← BUILT (Lecture 2, Altman — execution half)
        │   ├── how-to-operate-rabois.md             ← TODO (Lecture 14, Rabois)
        │   ├── how-to-manage-horowitz.md            ← TODO (Lecture 15, Horowitz)
        │   ├── legal-finance-hr-levy-nathoo.md      ← TODO (Lecture 18, Levy/Nathoo)
        │   └── later-stage-altman.md                ← TODO (Lecture 20, Altman)
        └── user-research/
            ├── talking-to-users-cheung.md           ← TODO (Lecture 4 — user research portion)
            └── user-interviews-shear.md             ← TODO (Lecture 16, Shear)
```

---

## Naming conventions

**Folders** — named by topic, lowercase, hyphenated. Describes the founder decision or situation, not the lecture.
```
market-strategy/   hiring/   fundraising/   product/   growth/   operations/
```

**Files** — named as `[topic]-[speaker-last-name].md`. Lowercase, hyphenated. If multiple speakers on same topic, list up to two surnames.
```
competition-monopoly-thiel.md
culture-chesky-lin.md
what-investors-want-andreessen-conway.md
```

**Never** name files by lecture number. `lecture-5-thiel.md` tells a founder nothing.

---

## One file = one lecture = one speaker (or one panel)

Each file covers one lecture's worth of thinking on a topic. No merging insights from different lectures into a single file. If two lectures cover the same topic (e.g. hiring appears in Lectures 2, 10, 11, 13), each gets its own file under the same folder.

Why: attribution stays clean, contradictions between speakers stay visible, the Karpathy extraction loop processes one lecture at a time anyway.

Exception: panel lectures with 2-3 speakers on the same topic (e.g. Lecture 10: Chesky + Lin on culture) can be one file since they appeared together. Attribute every insight to the specific speaker.

---

## Lecture → file mapping

Verified against actual lecture titles and speakers on 2026-07-09 (see `lessons/` for what
was wrong before and why). Lecture 2 was previously mislabeled "early hiring" — its real
title is "Team and Execution." Lecture 1's file name previously said "execution," which is
actually Lecture 2's topic — Lecture 1 is idea evaluation/early product (Altman) plus why to
start a startup at all (Moskovitz). Both split into two files because each covers two
distinct topics, the same way Lecture 4 and Lecture 19 do.

| Lecture | Speaker(s) | Topic folder | File name | Status |
|---------|-----------|--------------|-----------|--------|
| 1 | Sam Altman | ideas/ | idea-and-product-altman.md | BUILT |
| 1 | Dustin Moskovitz | ideas/ | why-start-a-startup-moskovitz.md | BUILT |
| 2 | Sam Altman | hiring/ | team-and-cofounders-altman.md | BUILT |
| 2 | Sam Altman | operations/ | execution-altman.md | BUILT |
| 3 | Paul Graham | ideas/ | counterintuitive-startups-graham.md | TODO |
| 4 | Adora Cheung | product/ | mvp-and-users-cheung.md | TODO |
| 4 | Adora Cheung | user-research/ | talking-to-users-cheung.md | TODO |
| 5 | Peter Thiel | market-strategy/ | competition-monopoly-thiel.md | BUILT |
| 6 | Alex Schultz | growth/ | growth-mechanics-schultz.md | TODO |
| 7 | Kevin Hale | product/ | building-for-love-hale.md | TODO |
| 8 | Williams/Kan/Tang | growth/ | unscalable-things-williams-kan-tang.md | TODO |
| 9 | Andreessen/Conway/Conrad | fundraising/ | what-investors-want-andreessen-conway.md | BUILT |
| 10 | Alfred Lin, Brian Chesky | hiring/ | culture-chesky-lin.md | TODO |
| 11 | Collison/Silbermann | hiring/ | scaling-teams-collison-silbermann.md | TODO |
| 12 | Aaron Levie | market-strategy/ | enterprise-disruption-levie.md | TODO |
| 13 | Reid Hoffman | hiring/ | great-founder-hoffman.md | TODO |
| 14 | Keith Rabois | operations/ | how-to-operate-rabois.md | TODO |
| 15 | Ben Horowitz | operations/ | how-to-manage-horowitz.md | TODO |
| 16 | Emmett Shear | user-research/ | user-interviews-shear.md | TODO |
| 17 | Hosain Rahman | — | SKIP for v1 (hardware-specific) | SKIP |
| 18 | Levy/Nathoo | operations/ | legal-finance-hr-levy-nathoo.md | TODO |
| 19 | Seibel/Bosmeny/Caldwell | fundraising/ | pitching-seibel-bosmeny-caldwell.md | TODO |
| 19 | Tyler Bosmeny | sales/ | early-sales-bosmeny.md | TODO |
| 20 | Sam Altman | operations/ | later-stage-altman.md | TODO |

Note: Lecture 1 (Altman/Moskovitz), Lecture 2 (Altman), Lecture 4 (Cheung), and Lecture 19
(Bosmeny) each produce two files because they cover two distinct topics.

---

## Build priority

Build in this order — most live for an early-stage founder first:

1. `market-strategy/competition-monopoly-thiel.md` — **DONE**
2. `hiring/team-and-cofounders-altman.md` + `operations/execution-altman.md` — **DONE**
3. `ideas/idea-and-product-altman.md` + `ideas/why-start-a-startup-moskovitz.md` — **DONE**
4. `fundraising/what-investors-want-andreessen-conway.md` — **DONE**
5. `product/building-for-love-hale.md` — feeds directly into what you're building
6. `user-research/user-interviews-shear.md` — most tactical, immediately usable
7. `hiring/culture-chesky-lin.md` — relevant once you're hiring beyond 5 people
8. `growth/unscalable-things-williams-kan-tang.md` — early traction phase
9. Everything else in order

**Before pulling a transcript for the next lecture:** verify its actual title, speakers, and
content against a real source (YouTube, startupclass.samaltman.com) — don't trust this table
blindly. It was wrong once already for Lecture 2. See `lessons/verify-lecture-mapping-before-building.md`.

**Full step-by-step process, including the now-mandatory HTML companion:** see
`EXTRACTION_RUBRIC.md`. Every skill file ships as a pair — `[name].md` (the AI-facing skill)
and `[name].html` (human-readable lecture notes, cloned from the shared template) — built in
the same pass so they can't drift out of sync.

---

## SKILL.md format

Every skill file must follow the format defined in CLAUDE.md exactly:

```
---
name:
description:
tags:
source:
---

## Overview
## Assumptions
## Insights
## Principles
## Where This Can Mislead You
## Thinking Framework
## Action Prompts
## What Not To Do
## Related Skills
```

`Where This Can Mislead You` is mandatory (added after the Thiel/skill-rubrics rebalance —
see `NORTH_STAR.md` and `EXTRACTION_RUBRIC.md` Step 3). It's easy to drop since it isn't in
the original CLAUDE.md template; check for it explicitly on every new file.

**Source field format:**
`"[Lecture title]," [Speaker], CS183B How to Start a Startup, Stanford 2014, [YouTube URL]`

**Related Skills:** only link to files that actually exist. Remove placeholder links.

---

## Creation pipeline (C → B → A)

**Phase C (first file in a new topic area):** conversation-first with Claude
1. Extract transcript: `python3 -c "from youtube_transcript_api import YouTubeTranscriptApi; api = YouTubeTranscriptApi(); t = api.fetch('VIDEO_ID'); [print(e.text) for e in t]" > speaker-lectureN-raw.txt`
2. Check transcript quality before starting — 2014 auto-captions are often low quality
3. Conversation session: feed in chunks, ask "if I was making a [topic] decision right now, what from this changes how I think?"
4. Convert conversation to SKILL.md: "Based on our discussion, write a SKILL.md following CLAUDE.md format. Include only what actually shifted how you'd think about a [topic] decision."
5. Use the file in one real decision before publishing

**Phase B (after first file):** extract rubric
- Document what worked as `EXTRACTION_RUBRIC.md`
- What made an insight actionable vs. interesting
- What question format surfaced the good stuff
- What got cut and why

**Phase C → A (at scale):** single-pass extraction
- Replace multi-turn conversation with one structured prompt encoding the rubric
- Extract transcript → prompt → SKILL.md draft → rubric check → edit pass → publish

---

## What goes in llms.txt

One line per skill file, format:
```
/skills/yc-how-to-start-a-startup/[folder]/[file] — [one sentence: when to load this]
```

Example:
```
/skills/yc-how-to-start-a-startup/market-strategy/competition-monopoly-thiel.md — load when a founder is deciding whether to enter a market, evaluating defensibility, or asking why a competitor can't just copy them
```

Update llms.txt every time a new file is added.

---

## Transcript files

Raw transcripts live at repo root during active work: `speaker-lectureN-raw.txt`
Delete or move to `/transcripts/` after the skill file is written.
Don't commit raw transcripts to the repo — they're working files, not published artifacts.

---

## Pending work

See `tasks/todo.md` for the current execution plan.
See `skill-rubrics.md` for quality standards.
See `lessons/` for what's been learned from building and testing skills so far.
