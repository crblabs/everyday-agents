# Everyday Agents

**Your everyday team of Claude helpers.**

This is a starter kit that turns [Claude Code](https://claude.com/claude-code) into a set of small personal assistants — *routines* — that run on a schedule, in the cloud, whether your computer is on or not. They can sort your email, prepare your mornings, watch topics you care about, and remind you of the dates that matter — and they report back to you in plain English.

You don't need to know how to code. You don't even need to know what Claude Code or GitHub *are* — if you can use email and a web browser, you're the intended audience.

## Start here — one message

Open **[claude.ai/code](https://claude.ai/code)** and paste this:

```
I want my own team of everyday helpers — sort my email, prep my
mornings, watch the topics I care about, remember what I'd forget.

Their starter kit is at github.com/crblabs/everyday-agents.
Take me from zero to my first running helpers: my own private copy
of the kit, the accounts they need, everything. You drive — I'll
answer questions.
```

That's genuinely it. Claude reads the kit, interviews you about your life, and about fifteen minutes later your first helpers are scheduled and running — whether your computer is on or not.

Two honest notes before you paste: this needs a **paid Claude plan** ([the 20-second check below](#what-you-need--check-before-you-start) says exactly what), and if claude.ai/code first asks you to **connect GitHub** or **pick a repository**, just go along — connecting with zero repositories is fine, and picking this very kit (`crblabs/everyday-agents`) is a perfectly good place to start: Claude will make your own private copy from there.

*Prefer to see the road before walking it? [Getting started](GETTING-STARTED.md) walks the same path step by step, assuming nothing.*

## What you get

Two things: a **guided builder** that turns any wish — "I want something that…" — into a working routine tailored to you, and a **catalog of starting points** to steal from. During setup, Claude interviews you and recommends what fits your life; you'll typically start with two or three:

| Routine | What it does for you |
|---|---|
| 📥 **Email triage** | Sorts new inbox email into a few simple labels you choose, every day |
| 🧹 **Email cleanup** | Archives stale, low-priority mail so your inbox stays breathable |
| ✉️ **Reply radar** | A daily short list of the emails that genuinely need an answer from you |
| ☕ **Morning brief** | Your day on one phone screen: meetings, prep notes, anything urgent |
| 🗓 **Week ahead** | A Sunday look at next week: commitments, conflicts, things to prepare |
| 🔭 **Watchlist** | Keeps an eye on topics or websites you care about; tells you only when there's news |
| 🎂 **Life admin** | Remembers birthdays, renewals, and deadlines — and warns you in time to act |
| 🪞 **Weekly review** | A weekly recap of what your agents did and what needs a decision from you |
| 🧰 **Kit news** | Tells you when the community adds new helpers to this kit |

Every routine is **read-mostly and cautious by design**: none of them ever sends an email, deletes anything, or spends money. They sort, summarize, and remind. You stay the only person who acts.

### And then: build your own

The catalog is where most people start — not where they end up. Say **"build me a routine that…"** and Claude walks you through the whole thing, no technical knowledge needed: shaping the idea, connecting any account it requires (guided, click by click), **rehearsing the routine live once so you see exactly what it will do**, then scheduling it. School-mail digests, travel prep, price watches, subscription audits — see [ideas people actually build](routines/BUILD-YOUR-OWN.md).

## What you need — check before you start

Twenty seconds here saves you a frustrating half hour later:

- ✅ **A paid Claude plan** — Pro or Max ([pricing](https://claude.ai/pricing)). This is the kit's only cost. **The Free plan can't run scheduled helpers.** *(Claude through your employer? It may work, but your company's admin controls what's allowed — check the [FAQ](docs/faq.md#is-this-for-me) first.)*
- ✅ **A Google account for the email & calendar helpers** — a free personal **@gmail.com is enough; you do NOT need Google Workspace.** *(A work Google account works only if your admin allows connecting apps.)*
- ✅ **An email address** — that's all it takes to create the free GitHub account during setup.
- ✅ **A web browser** — any modern one, on any computer. Nothing gets installed.
- ⚠️ **Your mail lives in Outlook, iCloud, or Yahoo?** Honest answer: the email and calendar helpers won't work for you *today* — most of the catalog is built on Gmail and Google Calendar. The watchlist, life-admin, and kit-news helpers still work (they need no accounts at all), but if email help is why you came, better to know now. More providers can arrive as connections do.

All green? Carry on.

## Setup

**New to all of this?** Follow **[Getting started](GETTING-STARTED.md)** — the same path as below, but assuming nothing: it explains what Claude Code and GitHub are and walks you through creating the two accounts first. Budget 20–30 relaxed minutes.

**Already have a Claude plan and a GitHub account?** The short version, about 15 minutes:

1. **Make your own private copy of this kit.**
   Click the green **"Use this template"** button at the top of this page → **"Create a new repository"**. Name it anything (e.g. `my-agents`) and set it to **Private**. This copy is yours: your helpers will keep their notes in it, and nobody else can see it.

2. **Connect your accounts.**
   Go to [claude.ai/customize/connectors](https://claude.ai/customize/connectors) and connect **Gmail** and **Google Calendar** (that covers most of the catalog). You're granting access to *your* Claude — not to this kit or its author.

3. **Open your copy with Claude Code.**
   Easiest path, no install: go to [claude.ai/code](https://claude.ai/code) and open the repository you created in step 1. (Desktop app or terminal work too.)

4. **Say: "set me up"** — or paste the message from [Start here](#start-here--one-message); both land in the same place. Claude interviews you for a few minutes, recommends starter routines, and schedules them. That's it.

From then on, your routines run on their schedule. You can see, pause, or delete any of them at any time at [claude.ai/code/routines](https://claude.ai/code/routines).

## The community

Your copy is private, but the kit is shared — and it grows by gifts. All of it by talking to Claude in your copy, never by learning GitHub:

- **"What's new in the kit?"** — see and install what others contributed since your copy was made. Your copy never goes stale.
- **"Share my … routine"** — give a routine you built. It's scrubbed of everything personal (you see exactly what's removed), credited to you, and **a human reads every line** before anyone else can install it.
- **"I wish a helper could…"** — can't build it? Wishing for it is a real contribution; someone else may build it, and you're credited for the idea.
- **"This routine keeps doing X wrong"** / **"I got lost"** — field reports and confusion reports make the kit better for the next person. Confusion is a contribution here, not a failure.

The promises: sharing is always opt-in and previewed, every gift is credited your way, and everything installable was human-reviewed against a [public checklist](CONTRIBUTING.md). More in [the community page](docs/community.md).

## Good to know

- **Privacy** — Your copy of this repository is private. Routines write their notes into it and nowhere else. Nothing is shared back to this public kit. See the [FAQ](docs/faq.md).
- **Cost** — Routines run on your Claude subscription and count toward its usage, like any conversation. Each routine here is designed to be a short, few-minute run. See [How it works](docs/how-it-works.md).
- **Control** — Every routine reports what it did, *even when the answer is "nothing"*. A missing report means something's wrong, not that all is quiet.
- **Off switch** — Pause or delete everything anytime at [claude.ai/code/routines](https://claude.ai/code/routines). Disconnect accounts anytime at [claude.ai/customize/connectors](https://claude.ai/customize/connectors).

## Learn more

- [Getting started, step by step](GETTING-STARTED.md) — the detailed walkthrough of the four steps above
- [How it works](docs/how-it-works.md) — what a routine actually is, in plain English
- [Build your own](routines/BUILD-YOUR-OWN.md) — how the builder works, and ideas to steal
- [The community](docs/community.md) — sharing, wishing, and what's new, all by conversation
- [Connections, in plain English](docs/connections.md) — what connecting an account means, and how to undo it
- [FAQ](docs/faq.md) — privacy, cost, safety, and how to stop
- [What's new](CHANGELOG.md) — the kit's news, in plain words

## For the curious

The kit is 100% plain text — no code to run, nothing to install. `routines/` holds the catalog (each routine is a readable instruction sheet), `my/` is where *your* helpers keep their configuration and notes, and `.claude/skills/` teaches Claude how to set you up. Read any of it; it's written for humans too.

---

*Made with Claude Code. Share the kit, keep your copy private.*
