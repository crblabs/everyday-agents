---
name: setup
description: First-run onboarding for this personal routine kit — interview the owner, recommend starter routines from the catalog, schedule them as cloud routines, and record everything in my/. Use when the owner says "set me up", "get started", or starts any first conversation in a fresh copy.
---

# Setup — onboard the owner

You are talking to the owner of a fresh copy of this kit — very likely a non-technical person. Your job: a warm, short interview; two or three well-chosen routines scheduled and recorded; zero jargon. Read `CLAUDE.md` first if you haven't; its rules apply throughout.

**Tone contract**: short questions, one at a time or in small groups. Explain any term you can't avoid. Never show IDs, cron syntax, or file paths unless asked — translate ("every weekday at 7am", not `0 6 * * 1-5`).

## Step 0 — Already set up?

Read `my/routines.md`. If routines are already recorded there, this isn't a first run — tell the owner what's installed and switch to the **add-routine** skill instead.

## Step 1 — Interview

Learn, conversationally (not as a form):

1. **First name** and **timezone** (or city — derive the timezone; confirm it, since every schedule depends on it).
2. **Life shape**: work situation, roughly what their inbox and calendar look like, what regularly eats their time or gets forgotten.
3. **Pain picker** — offer the catalog's jobs as outcomes, not names: "Would it help if something sorted your inbox every day? Gave you your day on one screen each morning? Watched a topic for you? Remembered birthdays and renewals?" Let them react.

## Step 2 — Recommend 2–3 routines (not more)

From their answers, pick the two or three best-fit routines from `routines/` and read each one's `ABOUT.md` and `ROUTINE.md`. When their life shape matches a pack in `packs/`, lead with the pack ("this sounds like the freelancer pack") — its page explains the why of each pick. Present each recommendation as: what it does for them, when it would run, where its report lands. Starting small is deliberate — say so, and mention they can add more any day with "add a routine". Offer **kit news** as an optional extra — the helper that tells them when the community adds new ones.

If the interview surfaced a need the catalog doesn't cover, don't force a poor fit and don't lose it either: name it back to them ("a helper for X doesn't exist yet — we can build it together after your starters are running, just say 'build me a routine'"), and note it in `my/profile.md`. The **build-routine** skill handles that path.

Take their picks. For each, gather what its `ROUTINE.md` placeholders need (label names, brief time, watch topics, dates…). Prefer sensible defaults offered for confirmation over open questions.

## Step 3 — Check connections

Each `ABOUT.md` names the connectors its routine needs (Gmail, Google Calendar, …). Verify those are connected — if the scheduling tool below is available, its connector list is the truth; otherwise ask the owner to check [claude.ai/customize/connectors](https://claude.ai/customize/connectors). If one is missing, walk them through connecting it the way `docs/connections.md` describes — exactly what to click and what the approval screen will say — then wait, and verify with a harmless read before moving on. Do not schedule a routine whose connector is absent.

## Step 4 — Fill and confirm each prompt

For each chosen routine, produce its live prompt: take `routines/<name>/ROUTINE.md` verbatim and replace every `{{placeholder}}` with the owner's values. Rules:

- **No `{{` survives.** Grep your result; an unfilled placeholder is a bug.
- **Never weaken the IRON LAW line or the report contract** — they are the safety promise the docs make.
- Times inside the prompt are written in the owner's local timezone, named explicitly (e.g. "09:00 Europe/Paris").

Show the owner a plain-English summary of each (not the raw prompt, unless they want it): "Every weekday at 7am your time, it will…". Get an explicit OK per routine.

## Step 5 — Schedule

Convert each agreed schedule to a UTC cron expression (minimum interval: 1 hour; confirm the local→UTC conversion in your summary). Then:

**Path A — the schedule skill is available** (check your available skills for `schedule`): invoke it to create each routine — name from the catalog (e.g. "Morning brief"), the filled prompt as the message, the repo's own GitHub URL (from `git remote get-url origin`) as the source, and the needed connectors attached. Confirm each creation and keep the returned routine link.

**Path B — it isn't**: give the owner their finished prompt in a copy-paste block plus exact click-by-click steps for [claude.ai/code/routines](https://claude.ai/code/routines): New routine → paste the prompt → pick their repository → set the schedule → attach the connectors → save.

## Step 6 — Record everything

Write, then commit (message: `setup <YYYY-MM-DD>: onboarded <first name>, installed <routine names>`):

- `my/profile.md` — name, timezone, the useful context from the interview, preferences. This is the file every routine reads first; keep it current and free of anything the owner wouldn't want written down.
- `my/routines.md` — one entry per installed routine: name, what it does in one line, schedule (local **and** UTC cron), routine link if you have it, date installed.
- Config files any chosen routine needs (`my/dates.md`, `my/watchlist.md`) — filled from the interview.

Push if you can; a push failure is reported in plain words, never silently swallowed (the owner may need to click "authorize" somewhere — help them).

## Step 7 — Close the loop

Tell the owner: which helpers now exist, when the first one runs, **where its report will appear**, and the magic phrases — "check my routines", "add a routine", "build me a routine" for anything the catalog doesn't cover, and "what's new?" to see what the community has added. Offer a test-fire of one routine now if they'd like to see a report immediately.
