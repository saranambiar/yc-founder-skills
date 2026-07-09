# Extraction Rubric — how to turn a lecture into a skill file

Read `NORTH_STAR.md` and `skill-rubrics.md` before this file. This is the step-by-step
process; those are the standard the output is judged against. Written after two lectures
(Thiel via full conversation-first iteration, Altman Lecture 2 via direct single-pass
extraction) — this is Phase A of the C→B→A pipeline described in `STRUCTURE.md`, now that
Phase B (this document) exists.

---

## Step 0: Verify the lecture, before touching a transcript

`STRUCTURE.md`'s lecture → topic table was assembled from memory once and was wrong for
Lecture 2 (labeled "early hiring," actually "Team and Execution"). Before pulling a
transcript for any TODO lecture:

1. Search for the actual video title and full speaker list — don't trust a summarized
   lecture list uncritically; simplified lists often drop guest panelists (this looked like
   5+ errors in `STRUCTURE.md` on first pass; only one was real).
2. Confirm the topic folder and file name still make sense given what the lecture actually
   covers. If it covers two distinct topics, plan to split into two files now (see Step 4).
3. Fix `STRUCTURE.md`'s table in the same pass if it was wrong. Don't proceed on a table
   entry you haven't checked.

Skipping this step risks building a plausible-sounding but fabricated skill file — grounding
content in the wrong transcript is a version of the exact thing `CLAUDE.md` rules out
("do not invent insights... everything must be grounded in the transcript provided").

## Step 1: Pull and read the full transcript

```bash
python3 -c "
from youtube_transcript_api import YouTubeTranscriptApi
api = YouTubeTranscriptApi()
t = api.fetch('VIDEO_ID')
with open('transcripts/SLUG/SLUG-raw.txt', 'w') as f:
    for e in t: f.write(e.text + '\n')
"
```

- If more than one upload of the same lecture exists, fetch both and compare. Prefer the one
  with real punctuation and capitalization over raw lowercase auto-captions — it's faster to
  read and less likely to be misparsed. (Word counts should be close; if one is dramatically
  shorter, check it isn't a cut-down re-upload.)
- **If `youtube-transcript-api` returns `IpBlocked`** (this happens after roughly 10 pulls in
  one session), don't retry it repeatedly. Check whether
  `github.com/Atarity/How-To-Start-A-Startup` has the lecture and pull the raw file directly
  with `curl`/`wget` — e.g. `curl -s "https://raw.githubusercontent.com/Atarity/How-To-Start-A-Startup/master/<lecture-folder>/<file>.md"`.
  **Do not use `WebFetch` for this** — it routes content through a summarizing model and
  returns a paraphrase even when asked for verbatim text, which breaks the exact-quote
  requirement below. See `lessons/transcript-fallback-when-youtube-is-blocked.md`.
- **Read the entire transcript before writing anything** — not a skim, not just the first
  section. Both lectures built so far had their most decision-relevant material in places
  that wouldn't have survived a skim: the Q&A at the end of Thiel's lecture (Palantir example,
  lean-startup skepticism, the closing "vast gate" line) and the pre-lecture Q&A in Altman's
  (the burnout/support-network answer, which matters directly for the intensity section later
  in the same transcript).
- Raw transcripts live at `transcripts/<slug>/` and are gitignored — never commit them.

## Step 2: Decide topic scope — one file, or split?

Check whether the lecture covers one coherent topic or genuinely distinct topics that would
serve different founder situations (a founder asking about cofounder equity and a founder
asking about competitor-driven demoralization are not the same conversation). If it splits,
follow the existing precedent (Lecture 4 → product + user-research; Lecture 19 → fundraising
+ sales; Lecture 2 → hiring + operations): one `.md` and one `.html` per topic, sharing the
same `source` field and transcript.

Don't split reflexively — most lectures are one coherent topic. Split only when the two
halves would genuinely be loaded for different kinds of founder questions.

## Step 3: Write the `.md` file

Follow the SKILL.md format from `CLAUDE.md` exactly, but every behavioral instruction in it
is calibrated against `NORTH_STAR.md`, not just internally consistent. Concretely:

- **Overview**: what it's for, concrete example situations, and — critically — what it's
  *not* for, naming the adjacent skill that covers that instead (even if that skill doesn't
  exist yet — say so, don't leave the boundary implicit).
- **Assumptions**: name the stage/context the advice is calibrated for. Both lectures so far
  needed this — Thiel's frameworks assume long-term company building; Altman's hiring advice
  assumes a pre-~10-person team. Advice applied outside its calibrated stage produces wrong
  answers, and the assumptions section is what lets the AI catch that instead of applying it
  blindly.
- **Insights**: comb the *entire* transcript for quotable, decision-relevant material —
  including the Q&A, including asides, including things said before the "official" lecture
  starts. Aim for 8-12 quotes minimum. A quote earns its place if it would change a specific
  decision, not just because it's memorable. Every quote gets a one- or two-sentence Context
  note explaining what problem the speaker was addressing — a quote without context is a
  fortune cookie.
- **Principles**: 8-13 numbered, distilled directly from the Insights above — not generic
  startup advice restated. If a principle doesn't trace to a specific thing the speaker said,
  it doesn't belong here.
- **Where This Can Mislead You** — mandatory, not optional. Every framework has edges: advice
  that's time-bound (2014-specific), stage-bound (pre-scale vs. post-scale), or that a founder
  could over-apply into paralysis or false modesty. This section is where that judgment lives.
  It's easy to drop this when compressing a lecture into a template — it doesn't map to a
  named section in `CLAUDE.md`'s original spec, which is exactly why it has to be checked for
  explicitly (see `lessons/dont-lose-the-self-critique-layer.md`).
- **Thinking Framework**: situational, not a checklist. For each situation: how to introduce
  it (lead with a concrete illustration or question, not a jargon label), what to ask, and
  what a good vs. weak answer looks like. State a plain conclusion once the founder has
  answered and it's genuinely earned — don't chain questions forever to avoid concluding
  (see `lessons/socratic-vs-directive-balance.md`). Match this to real situations a founder
  would actually bring, not abstract topic headings.
- **Action Prompts**: Step 0 (get minimum context, skip if already given), Step 1 (route to
  the right thinking-framework thread), then one entry per situation with what to ask and
  what not to do in that situation specifically.
- **What Not To Do**: failure signals, not restated principles — describe what the AI
  actually tends to do wrong (open with filler, present a priority list, over-hedge into
  never concluding), not just what the framework says not to do.
- **Related Skills**: only link to files that exist. If none exist yet, say so and name what
  would extend this once built (the way both Lecture 2 files point at each other and at the
  not-yet-built culture/management lectures).

## Step 4: Build the `.html` companion — required for every skill file

Every skill file ships with a companion HTML page. Purpose: a human-readable "good notes for
the lecture" page — insights, quotes, and the actual arguments, not the AI-facing behavioral
instructions (those stay in the `.md` only; a founder reading the HTML doesn't need to see
"don't open with filler affirmations").

**Use `skills/yc-how-to-start-a-startup/market-strategy/competition-monopoly-thiel.html` as
the literal template.** Copy its `<style>` block and structural conventions rather than
inventing new ones — visual consistency across the whole repo matters more than any single
page being novel. Fixed section order:

1. **Header** — source tag (lecture #, speaker, course), title, one-line lede.
2. **Core argument** — the one thing the lecture is actually about, in a paragraph.
3. **Concept sections** (2-5, one per major framework/insight cluster) — use the card grid,
   callout stat boxes, and diagrams (inline SVG, following the concentric-circles/X-Y-diagram
   pattern) where a visual actually clarifies the idea; use quote blocks (rotate through the
   sage/rose/lavender/peach color variants already defined) for direct quotes with attribution.
4. **From the Q&A** — if the lecture had a live Q&A with material distinct from the prepared
   talk, give it its own section rather than burying it inside the concept sections.
5. **Where This Framework Can Mislead You** — mirror the `.md` section, using the
   `.antipattern` box style already defined in the CSS.
6. **Takeaways** — numbered principles list (`.principles-list`), matching the `.md`'s
   Principles section.
7. **Key Quotes** — a denser grid of all major quotes, for skimming/reference.
8. **Honest Test / Apply Now** — a short numbered list of questions a founder can run on
   their own situation right now.
9. **Closing line** — if the lecture has one, a final pull-quote before the footer.
10. **Footer** — source attribution, link to the original lecture, repo link.

After building: verify tag balance (`<section>`/`<div>`/`<blockquote>` open/close counts
match) and that every `nav` `href="#id"` has a matching section `id` — both are one-line
Python checks, do them before considering the page done. See the commit that synced Thiel's
HTML for the exact verification commands.

## Step 5: Update the repo indexes

- `STRUCTURE.md` — mark the row(s) BUILT, fix anything the Step 0 verification changed.
- `llms.txt` — one line per new `.md` file, format already specified there.
- `tasks/todo.md` — log what was built, what was skipped/deferred and why (e.g. live-
  conversation retesting is a known-open item for every skill file so far — track it there,
  don't silently drop it).

## Step 6: Definition of done (and what's still open even when "done")

A skill file being built and passing the mechanical checks above is not the same as it being
validated. The original plan (`plans/product-skill-pipeline.md`) set a "3-decision test" —
use the file in three real decisions before calling it finished. Fast-tracking through many
lectures means that test isn't happening per-file in real time. Be honest about this in
`tasks/todo.md` rather than letting "built" quietly stand in for "validated": every skill
file shipped this way carries an open item to actually test it in a live conversation against
`NORTH_STAR.md` before fully trusting it.

## What tends to go wrong (carry these forward)

- Dropping the transcript's Q&A section — it's disproportionately rich in decision-relevant,
  non-obvious material precisely because it's unscripted.
- Skipping the "Where This Can Mislead You" section because it doesn't map to a named
  section in the original template.
- Building the `.md` and treating the `.html` as optional or a later nice-to-have — it isn't;
  build both in the same pass so they can't drift out of sync (they already did once, for
  Thiel, before this rubric existed).
- Trusting `STRUCTURE.md`'s existing table without checking it against a real source.
- Letting the behavioral rules default toward pure Socratic questioning instead of stating an
  earned conclusion — check every new skill file against
  `lessons/socratic-vs-directive-balance.md` specifically, since it's an easy default to fall
  back into when writing "ask, don't tell" instructions.
