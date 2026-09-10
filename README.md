# Everyday Agents

**Your everyday team of Claude helpers.**

This is a starter kit that turns [Claude Code](https://claude.com/claude-code) into a set of small personal assistants — *routines* — that run on a schedule, in the cloud, whether your computer is on or not. They can sort your email, prepare your mornings, watch topics you care about, and remind you of the dates that matter — and they report back to you in plain English.

You don't need to know how to code. You don't even need to know what Claude Code or GitHub *are* — if you can use email and a web browser, you're the intended audience, and the [step-by-step guide](GETTING-STARTED.md) explains every word as it comes.

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

Every routine is **read-mostly and cautious by design**: none of them ever sends an email, deletes anything, or spends money. They sort, summarize, and remind. You stay the only person who acts.

### And then: build your own

The catalog is where most people start — not where they end up. Say **"build me a routine that…"** and Claude walks you through the whole thing, no technical knowledge needed: shaping the idea, connecting any account it requires (guided, click by click), **rehearsing the routine live once so you see exactly what it will do**, then scheduling it. School-mail digests, travel prep, price watches, subscription audits — see [ideas people actually build](routines/BUILD-YOUR-OWN.md).

## Setup

**New to all of this?** Follow **[Getting started](GETTING-STARTED.md)** — the same path as below, but assuming nothing: it explains what Claude Code and GitHub are and walks you through creating the two accounts first (a paid Claude plan is the kit's only cost; GitHub is free). Budget 20–30 relaxed minutes.

**Already have a Claude plan and a GitHub account?** The short version, about 15 minutes:

1. **Make your own private copy of this kit.**
   Click the green **"Use this template"** button at the top of this page → **"Create a new repository"**. Name it anything (e.g. `my-agents`) and set it to **Private**. This copy is yours: your helpers will keep their notes in it, and nobody else can see it.

2. **Connect your accounts.**
   Go to [claude.ai/customize/connectors](https://claude.ai/customize/connectors) and connect **Gmail** and **Google Calendar** (that covers most of the catalog). You're granting access to *your* Claude — not to this kit or its author.

3. **Open your copy with Claude Code.**
   Easiest path, no install: go to [claude.ai/code](https://claude.ai/code), and open the repository you created in step 1. (If you prefer the desktop app or terminal, that works too.)

4. **Say: "set me up".**
   Claude reads this kit, interviews you for a few minutes, recommends starter routines, and schedules them. That's it.

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
