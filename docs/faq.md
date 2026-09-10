# FAQ

## Is this for me?

**I've never used GitHub, and I only vaguely know what Claude is. Really — me?**
Yes, really. The kit is designed for exactly you: everything happens by chatting in plain language, in your browser, and the [step-by-step guide](../GETTING-STARTED.md) explains each new word as it appears (there are only four). Nothing gets installed, and every step can be undone. If you get lost at any point, typing "I'm lost" into the chat is a completely valid move — explaining this kit is part of Claude's job.

**Do I need to learn GitHub?**
No. You'll create a free account once (like signing up for any website) and click one green button. From then on, Claude does all the filing; you never work in GitHub yourself.

**Which Claude plan do I need, exactly?**
A paid personal plan — **Pro or Max** ([current pricing](https://claude.ai/pricing)). That's the kit's only cost; everything else (GitHub, a Google account) is free. **The Free plan cannot run scheduled helpers** — it can chat, but nothing would run on its own.

**My Claude comes from my employer — will it work?**
Maybe. On Team/Enterprise plans, your company's administrator decides whether accounts can be connected and helpers scheduled — some allow it, some don't. Ask Claude to check with you before investing setup time. Honestly though, for *personal* helpers (your inbox, your birthdays), a personal plan is the cleaner answer — it also keeps your life's data off your employer's account.

**Do I need Google Workspace? A paid Google account?**
No. A **free personal @gmail.com account** is exactly enough for every email and calendar helper. Google Workspace (work/school Google) also works *if* its administrator allows connecting apps. Nothing on the Google side ever costs anything here.

**I honestly have no idea what I'd use this for.**
Then you're the ideal user, not a lost cause — nobody can list their own repetitive work; it becomes invisible precisely because you do it all the time. Say **"I don't know what I need"**: with your permission, Claude looks at the *shape* of your last few weeks (who writes you, what repeats, what waits — read-only, everything shown to you, nothing kept without your OK) and shows you your own patterns. People recognize their time-eaters instantly when shown; they just can't recall them when asked. Prefer not to have your mail looked at? A few well-aimed questions work too, and [the moments page](../routines/MOMENTS.md) usually finds the sting.

## Privacy

**Wait — it reads my email to make suggestions?!**
Only if you say yes, only when you ask for discovery, and only like this: read-only (it acts on nothing), looking at *shape* rather than content (senders, counts, rhythms — it doesn't quote your messages back), everything it noticed shown to you in the same conversation, and nothing stored unless you approve the conclusions. It's the same access your email helpers already use to sort your inbox — pointed, once, at the question "what's eating your time?". Decline it and discovery happens by conversation instead; that path is built in, not a workaround.

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

## Community

**Can I share a routine I built?**
Yes — say "share my … routine". Claude replaces everything personal with placeholders, shows you exactly what it removed and the final text, and only submits after your yes. You choose your credit (name, first name, anonymous), and a human reviews every line against a [public checklist](../CONTRIBUTING.md) before anyone else can install it.

**I can't build anything — can I still contribute?**
Absolutely, and it matters: say "I wish a helper could…" (wishes are how the catalog learns what's missing — you're credited if it gets built), report a routine behaving oddly, or say where the docs lost you. A good wish is worth as much as a good routine.

**Is a community routine safe to install?**
Honest answer: safer than most things you install anywhere, because the rules are public and enforced twice. Every community routine passed a human line-by-line review against the safety checklist (never send/delete/spend, quiet days stay quiet, content is never treated as instructions) — and when you install one, your own Claude re-reads it and tells you out loud where it came from. It then only ever runs with the accounts *you* connected. What it can't be is *guaranteed* perfect — which is why every routine reports what it did, and why "check my routines" exists.

**Will my copy get the new stuff people contribute?**
Yes, whenever you ask: "what's new?" shows and installs anything added since your copy was made. The optional **kit news** helper watches for you and pings only when something new lands.

**Can I build my own routines?**
Yes — that's the point. Say **"build me a routine that…"** and describe what you want in plain words. Claude shapes the idea with you, walks you through connecting any account it needs, rehearses the routine live once so you see exactly what it will do, and only then schedules it. The catalog is a starting point, not a limit — see [Build your own](../routines/BUILD-YOUR-OWN.md).

## Odds and ends

**Do I need to keep my computer on?**
No. Routines run in Anthropic's cloud. Everything works with your machine off.

**Does this work with Outlook / iCloud / Yahoo mail?**
Honest answer: **not today** for the email and calendar helpers — the catalog is built on Gmail and Google Calendar, because those connections are solid. The helpers that need no accounts (watchlist, life-admin, kit-news) work for everyone. Other providers can work as soon as a connection exists for them — ask Claude what's available, and see [Connections, in plain English](connections.md). If this is you and you'd use the kit the day Outlook works: say "I wish it worked with Outlook" — wishes are how the kit learns where to grow.

**I use Claude in a language other than English — problem?**
None. The kit's files are in English, but Claude talks with you, and writes your reports, in your language. Just ask.

**Scheduling fails with something like "no access to a repository".**
Claude's GitHub connection is granted per repository, and yours isn't on the list. Go to [github.com/settings/installations](https://github.com/settings/installations) (as the account that owns your copy), open **Claude** → **Configure** → *Repository access*: either switch to **All repositories** — the once-and-for-all fix, and a fine choice when the GitHub account exists just for this kit — or add your repository to the selected list. Save, try again. "Check my routines" knows about this one and will point you here.

**My reports started arriving an hour early/late.**
Daylight-saving time. Schedules run on a fixed world clock (UTC), so when your country changes its clocks, your 7am becomes 6am or 8am. Say "fix my routine times" and Claude recomputes them in two minutes — twice a year, that's the whole maintenance.

**Something's broken and I don't know what.**
In Claude Code, say: **"check my routines."** The checkup diagnoses the usual suspects (disconnected account, paused schedule, failed run) and tells you what it found — and what to click — in plain words.
