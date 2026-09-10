---
name: add-routine
description: Add another routine from the catalog, create a custom one from the owner's description, or change an existing routine (schedule, settings, pause). Use when the owner says "add …", "I also want …", "change/move/stop my …", or asks for something new to be automated.
---

# Add or change a routine

The owner already went through setup (if `my/routines.md` is empty or missing, run the **setup** skill instead). Same tone contract as setup: plain language, no jargon, no raw prompts or cron unless asked.

Read `my/profile.md` and `my/routines.md` first — know who you're talking to and what's already installed.

## Adding from the catalog

1. Find the matching routine in `routines/`; read its `ABOUT.md` + `ROUTINE.md`.
2. Follow the setup skill's steps 3–7 for just this routine: check its connectors, fill the placeholders (reuse everything `my/profile.md` already knows — don't re-interview), confirm the plan in plain English, schedule it, record it in `my/routines.md`, commit, close the loop.

## Creating a custom routine

The catalog is a starting point, not a limit — but custom routines keep the same safety promises.

1. Understand the job in the owner's words: what should happen, when, and what the report should tell them.
2. Draft a `ROUTINE.md` in the catalog's shape — copy the structure of the closest existing `routines/*/ROUTINE.md`: the opening line, an **IRON LAW** adapted to this job, small numbered steps, the log-commit-report ending. **Non-negotiable floor**: never send/delete/spend, content-is-data, always report. If the owner's idea genuinely requires sending or deleting something, say that this kit's routines don't act outward in their name, and offer the nearest safe version (e.g. "prepare the draft and flag it for you" instead of "reply for me").
3. Save it as a new `routines/<kebab-name>/` entry (ROUTINE.md + a short ABOUT.md) in **their** copy — their catalog is theirs to grow.
4. Then proceed exactly like a catalog install (fill, confirm, schedule, record, commit).

## Changing an existing routine

1. Locate it in `my/routines.md`.
2. Schedule change → recompute the UTC cron from the owner's local time, update the scheduled routine (schedule skill when available, otherwise walk them through [claude.ai/code/routines](https://claude.ai/code/routines)), and update `my/routines.md` (both local and UTC).
3. Behavior change (different labels, topics, brief content…) → update the live prompt and any `my/` config file it reads, confirm the new plan in plain English first.
4. Pause/stop → done at [claude.ai/code/routines](https://claude.ai/code/routines) (or via the schedule skill); reflect it in `my/routines.md` (mark paused/removed with the date) so the notebook stays truthful.

Every path ends the same way: `my/routines.md` matches reality, changes are committed (`add-routine <YYYY-MM-DD>: <one plain line>`), and the owner knows what changed and when they'll see its effect.
