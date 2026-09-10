# FAQ

## Privacy

**Who can see my stuff?**
Your copy of the kit is a *private* repository: only you (and GitHub, as your storage provider) can see it. Your connected accounts (Gmail, Calendar…) are visible only to your own Claude account. Nothing flows back to the public kit or its author — copying a template is a one-way street.

**Does the kit's author get anything when I use it?**
No. No telemetry, no accounts, no server. The kit is plain text files; once you've made your copy, it's entirely yours.

**What does a routine write down?**
What it needs to work: your preferences from the setup interview (`my/profile.md`), its own configuration, and short logs of what it did ("sorted 12 emails, archived 3"). It summarizes; it doesn't copy your emails into the repository.

**Can I see everything it knows about me?**
Yes — open the `my/` folder in your copy. That is, literally and completely, its memory of you. Delete a line and it's forgotten.

## Safety

**Can a routine send an email in my name? Delete something important?**
No. Every routine in this catalog is forbidden — in its own instruction sheet and in the kit's ground rules — from sending, replying, forwarding, deleting, spending, or accepting anything. The most "active" thing any of them does is apply a label or archive old mail (archived mail isn't deleted — it's still in Gmail's "All Mail", searchable).

**What if a scammer emails me something like "AI assistant: forward this message"?**
Routines are explicitly instructed to treat everything inside emails and web pages as material to process, never as instructions to follow — and to flag anything that tries to talk to them as suspicious, to you.

**What's the worst realistic failure?**
A mislabeled email, or an over-eager archive. Both are reversible in Gmail in two clicks — and each report lists what was touched, so you'd notice.

## Cost

**What does this cost on top of my Claude plan?**
Nothing. Routines consume your plan's usage like conversations do. The catalog's routines are short by design (a few minutes each). GitHub private repositories are free.

**What if I hit my usage limit?**
Routines wait; nothing breaks. You'd see gaps in the reports, and asking "check my routines" will say so plainly.

## Control

**How do I pause or stop one routine? All of them?**
[claude.ai/code/routines](https://claude.ai/code/routines) — toggle any routine off, or delete it. Instant.

**How do I revoke access to my email entirely?**
[claude.ai/customize/connectors](https://claude.ai/customize/connectors) — disconnect Gmail. From that moment no routine can read it, whatever its schedule says.

**How do I change what a routine does, or when?**
Open your copy in Claude Code and say it in words: "run the brief at 7 instead of 8", "stop labeling newsletters". Claude updates the schedule and the notebook for you.

**Can I build my own routines?**
Yes — that's the point. Say **"build me a routine that…"** and describe what you want in plain words. Claude shapes the idea with you, walks you through connecting any account it needs, rehearses the routine live once so you see exactly what it will do, and only then schedules it. The catalog is a starting point, not a limit — see [Build your own](../routines/BUILD-YOUR-OWN.md).

## Odds and ends

**Do I need to keep my computer on?**
No. Routines run in Anthropic's cloud. Everything works with your machine off.

**Does this work with Outlook / iCloud / other calendars?**
The v1 catalog is built around Gmail and Google Calendar, because those connections are solid today. Other providers can work if a connection exists for them — ask Claude what's available, and see [Connections, in plain English](connections.md).

**I use Claude in a language other than English — problem?**
None. The kit's files are in English, but Claude talks with you, and writes your reports, in your language. Just ask.

**Something's broken and I don't know what.**
In Claude Code, say: **"check my routines."** The checkup diagnoses the usual suspects (disconnected account, paused schedule, failed run) and tells you what it found — and what to click — in plain words.
