---
name: add-routine
description: Install another routine from the catalog, or change an existing routine (schedule, settings, pause). Use when the owner says "add the morning brief", "change/move/stop my …", or names a catalog routine. For a wish the catalog doesn't cover, use build-routine instead.
---

# Add or change a routine

The owner already went through setup (if `my/routines.md` is empty or missing, run the **setup** skill instead). Same tone contract as setup: plain language, no jargon, no raw prompts or cron unless asked.

Read `my/profile.md` and `my/routines.md` first — know who you're talking to and what's already installed.

## Adding from the catalog

1. Find the matching routine in `routines/`; read its `ABOUT.md` + `ROUTINE.md`.
2. Follow the setup skill's steps 3–7 for just this routine: check its connectors, fill the placeholders (reuse everything `my/profile.md` already knows — don't re-interview), confirm the plan in plain English, schedule it, record it in `my/routines.md`, commit, close the loop.

## Creating a custom routine

That's the **build-routine** skill's whole job — shaping the wish, connecting what's missing, a live rehearsal, then writing and scheduling it. Hand over to it whenever the owner's request goes beyond installing or adjusting what exists.

## Changing an existing routine

1. Locate it in `my/routines.md`.
2. Schedule change → recompute the UTC cron from the owner's local time, update the scheduled routine (schedule skill when available, otherwise walk them through [claude.ai/code/routines](https://claude.ai/code/routines)), and update `my/routines.md` (both local and UTC).
3. Behavior change (different labels, topics, brief content…) → update the live prompt and any `my/` config file it reads, confirm the new plan in plain English first.
4. Pause/stop → done at [claude.ai/code/routines](https://claude.ai/code/routines) (or via the schedule skill); reflect it in `my/routines.md` (mark paused/removed with the date) so the notebook stays truthful.

Every path ends the same way: `my/routines.md` matches reality, changes are committed (`add-routine <YYYY-MM-DD>: <one plain line>`), and the owner knows what changed and when they'll see its effect.
