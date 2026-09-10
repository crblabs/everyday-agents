# Getting started, step by step

This is the long version of the four steps on the front page. Nothing here requires technical knowledge. Budget about 15 minutes.

## Before you begin

You need:

- A **Claude account** with a paid plan (Pro or Max) — routines run on your subscription.
- A **GitHub account** (free) — this is where your private copy of the kit will live. If you don't have one, create it at [github.com/signup](https://github.com/signup). Think of GitHub as a filing cabinet for your helpers' notebooks; you'll rarely need to look at it directly.

## Step 1 — Make your own private copy

Your helpers need a notebook of their own: a place to keep your preferences, their notes, and their instructions. That's what your copy of this kit is.

1. At the top of [the kit's page](https://github.com/matt-crblabs/everyday-agents), click the green **Use this template** button, then **Create a new repository**.
2. **Repository name**: anything you like — `my-agents` works fine.
3. **Visibility**: choose **Private**. This matters — your helpers will write personal things (your schedule, your reminders) into it.
4. Click **Create repository**.

You now have your own copy. It is yours alone: making it didn't share anything with the kit's author, and nothing your helpers write ever flows back to the public kit.

## Step 2 — Connect your accounts

Your helpers can only see what you explicitly connect.

1. Go to [claude.ai/customize/connectors](https://claude.ai/customize/connectors).
2. Connect **Gmail** and **Google Calendar** — these cover the email routines, the morning brief, and the week ahead.
3. That's usually enough. You can connect more (Google Drive, Notion, …) later if a routine you want needs it.

You're granting access to *your* Claude account — the same Claude you talk to — not to any third party.

## Step 3 — Open your copy with Claude Code

The easiest path needs no installation:

1. Go to [claude.ai/code](https://claude.ai/code).
2. Connect your GitHub account if asked, and open the repository you created in Step 1.

Prefer an app? Claude Code also exists as a [desktop app and terminal tool](https://claude.com/claude-code); open your repository folder with it. Any of these paths ends the same way: a chat with Claude that can see your copy of the kit.

## Step 4 — Say "set me up"

Type exactly that, or anything like it. Claude will:

1. **Interview you** for a few minutes — your first name, your timezone, what eats your time, what you'd like off your plate.
2. **Recommend 2–3 starter routines** from the catalog. (Starting small is deliberate; you can add more any day by saying "add a routine".)
3. **Show you each routine's plan in plain English** — what it will do, when it will run — and ask for your OK.
4. **Schedule them** so they run automatically in the cloud, and write down everything it learned in the `my/` folder of your copy.

When it's done, it will tell you when to expect your first report.

## Living with your helpers

- **Where reports arrive.** Each routine tells you at setup where its report lands — for most, it's a small calendar event on your day (easy to glance at on your phone) and a note in your copy's history.
- **See or pause your routines** any time at [claude.ai/code/routines](https://claude.ai/code/routines). Pausing is instant and harmless.
- **Change anything** by opening your copy with Claude Code again and just saying so: "make the morning brief earlier", "stop watching that topic", "add the birthday reminders".
- **Check on things** the same way: "are my routines OK?" gets you a health report.

## The emergency stops

Two switches, both instant, both always available:

1. [claude.ai/code/routines](https://claude.ai/code/routines) — pause or delete any routine, or all of them.
2. [claude.ai/customize/connectors](https://claude.ai/customize/connectors) — disconnect an account (Gmail, Calendar, …) and no routine can see it anymore, scheduled or not.

Deleting your GitHub repository is a third, final switch: the helpers' notebook is gone, and every routine that depends on it stops working.

## If something doesn't work

Say "check my routines" in Claude Code — the checkup routine diagnoses the common problems (a disconnected account, a paused schedule, a failed run) and explains what it found in plain words. The [FAQ](docs/faq.md) covers the rest.
