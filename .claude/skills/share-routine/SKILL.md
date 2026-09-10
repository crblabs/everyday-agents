---
name: share-routine
description: Offer one of the owner's routines to the kit's community — scrub it of personal details, get explicit approval on the exact text, and submit it upstream (directly or via a prefilled one-click form). Use when the owner says "share my … routine", "give this to the community", or wants others to have something they built.
---

# Share a routine — a gift, scrubbed and consented

The owner wants to give a routine to the community. Your job: make the gift safe (nothing personal leaves), honest (they see exactly what goes), and warm (credit, and a clear picture of what happens next). `CLAUDE.md`'s rule applies with full force here: **nothing leaves this copy without the owner seeing the exact text and saying yes.**

Upstream home: `https://github.com/crblabs/everyday-agents`.

## Step 1 — Which routine, and is it shareable?

Confirm which routine (from `routines/` or `my/routines.md`). Sanity-check it against the kit's floor (`CONTRIBUTING.md`'s rubric): if their custom routine drifted from the contract (missing IRON LAW, missing always-report), fix that *with them* first — the review would bounce it anyway, and fixing beats rejection.

A routine that's already in the shared catalog (core or community) isn't shareable again — but a meaningful *improvement* to one is: submit it the same way, framed as a variation.

## Step 2 — Scrub

Produce the shareable version:

- Every personal value → `{{placeholder}}`: their name, timezone, label names, times, topics, people, places, anything from `my/`.
- Anything personal in prose (the ABOUT's examples, the IRON LAW's specifics) → generalized.
- Then **show the owner the removals as a list** ("I replaced: your name, your three label names, your 7am time, the two websites you watch") followed by the **full scrubbed text** of both files (ABOUT + ROUTINE). If any doubt remains about whether something is personal, scrub it and say so.

## Step 3 — Credit and the story

Ask two light questions: how they'd like to be credited (full name, first name, or anonymous — their choice, no default pushed) and, optionally, one sentence of the story ("what made you build it?") — it often becomes the best line of the ABOUT page.

## Step 4 — Explicit OK, then submit

Get an unambiguous yes on the final text — then submit, first path that works:

**Path A — `gh` is available and authed** (`gh auth status`): create the issue directly on upstream using the share form's shape — title `Routine: <name>`, label `routine-submission`, body containing the four sections (what it does / the instruction sheet / credit / story). Show the resulting link.

**Path B — prefilled form link** (the universal path): build the URL
`https://github.com/crblabs/everyday-agents/issues/new?template=share-routine.yml&title=<enc>&about=<enc>&sheet=<enc>&credit=<enc>&story=<enc>`
with each value URL-encoded. Tell the owner: "click this, the form is already filled — check it looks right, then press the green Submit button" (they may need to log into GitHub first; that's fine and safe — it's the real GitHub). **If the full URL exceeds ~6,000 characters**, prefill only template+title+credit and give the two long sections as clearly-labeled copy-paste blocks with "paste each into its box".

## Step 5 — Set expectations, and log

Tell them what happens next, honestly: a human reads every line against the public checklist before it can appear on the community shelf; they'll get a warm reply either way (visible on the same page as their submission); if accepted, it appears credited to them and other people's Claudes can install it. Nothing personal left this copy — the scrubbed text is all that traveled.

Append one line to `my/memory/community-log.md` (`YYYY-MM-DD: shared <name>`), commit (`share-routine YYYY-MM-DD: shared <name>`), push.
