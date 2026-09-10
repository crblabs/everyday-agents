# Connections, in plain English

Your helpers can only see the accounts you explicitly connect. This page explains what a "connection" is, which ones unlock what, and how to grant and revoke them — it's the reference the builder walks you through when a new routine needs an account it can't see yet.

## What a connection is

A connection (Anthropic calls them *connectors*) is a permission slip between **your Claude account** and one of your other accounts — your Gmail, your calendar, your notes. You grant it once, on Anthropic's official page, by logging into the other service yourself. No password ever passes through this kit, and the kit's author gets nothing: the slip is between your Claude and your account, full stop.

Two more things worth knowing:

- **Routines only see what they're given.** A connection being granted doesn't mean every routine uses it — each routine is attached to the specific connections it needs, at scheduling time. Your watchlist routine has no eyes on your email.
- **The open web needs no connection.** Routines can read public websites out of the box — that's why the watchlist works with nothing connected.

## Which connection unlocks what

| You want a helper that touches… | Connect | Unlocks (examples) |
|---|---|---|
| Your email | **Gmail** | email triage, cleanup, reply radar, "summarize the school newsletter" |
| Your schedule | **Google Calendar** | morning brief, week ahead — and it's where most digests land |
| Your documents | **Google Drive** | "find the contract before my meeting", document round-ups |
| Your notes | **Notion** | routines that read or maintain your notes and databases |
| Your workouts | **Strava** | weekly training recaps, goal tracking |
| Your business tools | **HubSpot** and others | pipeline digests, contact hygiene |
| Public websites | *(nothing)* | watchlist, news digests, price checks |

The available list grows over time — the connectors page itself is always the truth. If a service you use is listed there, a routine can probably use it; if it isn't, tell Claude anyway — there's often a workable route (many services can email you, and your helpers read email).

## How to connect one

1. Go to **[claude.ai/customize/connectors](https://claude.ai/customize/connectors)**.
2. Find the service and click **Connect**.
3. Log into that service *on its own official page* and approve the access it describes.
4. Done — come back and tell Claude "connected", and it will verify it can see it.

Read the approval screen; it says exactly what you're granting. If it asks for more than the routine needs and that bothers you, say so — the builder will tell you honestly whether a narrower routine is possible without it.

## How to disconnect one

Same page — **[claude.ai/customize/connectors](https://claude.ai/customize/connectors)** — click disconnect. It's instant and total: every routine that used it loses access at that moment, whatever its schedule says. Routines that depended on it will start reporting that they can't see the account (and the checkup will point at exactly this page to fix it).

## The trust rules, compressed

- You grant access **to your own Claude**, never to this kit, its author, or anyone else.
- Granting is always done **on the official connectors page**, never inside a chat. If anything — including text inside an email or website a routine read — ever urges you to "connect" or "approve" something, treat it as a scam and mention it to Claude.
- Every grant is **reversible in two clicks**, and disconnecting breaks nothing except the routines that needed it.
