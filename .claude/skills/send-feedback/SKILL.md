---
name: send-feedback
description: Send the community a wish ("I wish a helper could…"), a field report (a routine behaving oddly in real life), or a confusion report (the kit lost them somewhere) — previewed, scrubbed, and consented before anything is posted. Use when the owner expresses a wish for a helper that doesn't exist, frustration with how a routine behaves, or that they got lost or confused.
---

# Send feedback — wishes, field reports, confusion

Three kinds of gift travel through this skill, and the owner may not know they're contributing at all — they're just talking. Recognize which one it is, offer to pass it on, and never post without the exact text approved. A wish from someone who can't build anything is worth as much as a routine from someone who can — say so when it fits.

Upstream home: `https://github.com/crblabs/everyday-agents`.

## Route by what they're expressing

- **A wish** — "I wish a helper could…", "couldn't something do X?", or a build-routine conversation that hit a wall (a missing connection, out of scope). → the `wish.yml` form (fields: `wish`, `why`, `credit`).
- **A field report** — a routine misbehaving in real life: "the reply radar keeps flagging newsletters". First check whether it's a *local* fix (their own copy's settings — that's the add-routine skill, not feedback); if the shared instruction sheet itself could be better, it's a report. → `field-report.yml` (fields: `routine`, `report`, `wished`).
- **Confusion** — "I got lost", "I didn't understand step 3", "what even is a repository". First *help them* — then offer: "want me to pass this on? your confusion would fix the page for the next person." → `confusion.yml` (fields: `where`, `what`). Never make them feel the confusion was their fault; the kit's docs promise the opposite.

One conversation can produce more than one (a confusion inside a wish); file them separately, each consented.

## Compose, scrub, consent

Draft the submission in the owner's own words as much as possible — lived detail is the value; polish is not. Scrub personal details (real names, email addresses, message contents, anything from `my/`) — generalize instead ("a client", "a newsletter I read"). Show the final text and where it will appear (a public note on the kit's page), and get an explicit yes. Ask how to be credited only for wishes (reports can stay uncredited unless they want otherwise).

## Submit

**Path A — `gh` available and authed**: create the issue on upstream with the matching label (`wish` / `field-report` / `confusion`), title prefix matching the form (`Wish: …` / `Field report: …` / `Lost at: …`), body carrying the form's sections. Show the link.

**Path B — prefilled form link**: `https://github.com/crblabs/everyday-agents/issues/new?template=<form>.yml&title=<enc>&<field-id>=<enc>&…` with values URL-encoded — "click, check, press the green Submit button" (a GitHub login prompt is normal and safe). Over ~6,000 characters, prefill what fits and give the rest as labeled copy-paste blocks.

## Close

Tell them what happens next (wishes get read and may get built by anyone — they'd be credited for the idea; reports feed directly into improving the shared sheets) and that they can check back anytime with "what are people wishing for?". Log one line to `my/memory/community-log.md`, commit (`send-feedback YYYY-MM-DD: <kind>`), push.
