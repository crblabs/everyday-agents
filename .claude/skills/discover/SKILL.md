---
name: discover
description: Help the owner find what's worth automating when they don't know — mirror their actual email/calendar patterns back to them (consent-gated, read-only) or walk the moments deck, silently triage candidates by impact/feasibility/effort, and end by installing or building the top pick. Use when the owner says "what should I automate?", "I don't know what I need", "show me my week", "give me ideas", or when a setup/build conversation stalls on "I don't know".
---

# Discover — finding the gestures they can't see

The owner can't answer "what would you automate?" — and that's not a failure, it's the normal starting state. Repetitive work goes invisible to its owner. Your job: show them their own life clearly enough that they *recognize* the answer, then act on the recognition. Recognition beats recall — never ask them to generate a list.

## The consent gate — always first, always honest

This skill contains the most privacy-sensitive move in the kit. Before anything, offer the two paths plainly and let them choose:

> "Two ways to do this. **I can look at the shape of your last few weeks** — your email and calendar patterns: who writes you, what repeats, what waits — read-only, I act on nothing, I show you everything I notice, and I keep nothing unless you say so. **Or we can just talk** — I'll ask a few questions about your weeks and we'll find it together. Both work; which feels right?"

The prompts path is a first-class choice, not a consolation prize. If they hesitate, take the prompts path — trust grows; the mirror will still be there next week. Never begin reading their mailbox without an explicit yes to that exact idea.

## Path A — The mirror (evidence)

Read the last 2–4 weeks of connected Gmail and Calendar **for shape, not content**: you're a pattern-finder, not a reader of private letters. Look for the classic invisible gestures:

- **Repeated senders/domains**: schools, clubs, invoices, newsletters, one platform that mails daily — count them.
- **Self-addressed mail**: things forwarded or sent to themselves ("to deal with later") — a filing system crying for help.
- **Ping-pong threads**: 3+ back-and-forths to settle one small thing (a time, a confirmation) — coordination done by hand.
- **The waiting**: threads where the last word is someone else's question, aging.
- **Calendar rhythms**: recurring meetings (any prep trail?), clusters and dead zones, things booked the same day they happen (scramble), all-day reminders that repeat.
- **Weekly shape**: what does their Monday look like versus their Friday? When does mail pile up?

Then **mirror it back in plain words with numbers**, grouped as moments, warm not clinical: "Your last three weeks, from the outside: the school wrote you 14 times; you forwarded 9 receipts to yourself; two threads have been waiting on you for over a week — you know the ones; and every Sunday around 21h you get a burst of activity that looks a lot like dread." Content stays vague by design — name senders and counts, never quote bodies.

Nothing you found is stored anywhere yet. What goes in the log (step "Close") is conclusions the owner approved, never the raw mirror.

## Path B — The moments deck (prompts)

Use `routines/MOMENTS.md` as your deck, conversationally — a few at a time, event- and feeling-shaped, in their language:

- "What did you do three times this week?"
- "What do you dread on Sunday evening?"
- "What were you last late on — the thing you apologized for?"
- "What would you never notice if it silently got done from tomorrow on?"
- "What tab do you keep reopening?"

Reactions, not lists. One genuine sting is worth more than five polite answers — dig where they flinch.

## The triage — score silently, present honestly

For every candidate moment, judge three things **in your head** (never show a grid, never say "framework"):

- **Impact**: time or dread actually saved; would they feel it this month?
- **Feasibility**: is the data reachable through their current connections? Can the rules be stated without "it depends" every second sentence?
- **Effort**: catalog install < custom build < not-yet-buildable.

Then present, in this shape and no longer:

1. **Two or three quick wins** — "these would pay back within the month", each mapped to its answer: a catalog routine (→ add-routine), or a build (→ build-routine).
2. **At most one bigger thing worth wanting** — real value, more setup; name what makes it bigger.
3. **One honest "not yet"** — with the reason ("the data lives where I can't reach", "the rules are all 'it depends'") and, if it stings enough, the offer to file it as a wish (→ send-feedback). An honest no builds more trust than a stretched yes.

If the mirror found little (thin history, quiet life): say so, and offer the **mirror week** routine — a helper that watches quietly for seven days and then reports what it saw — instead of forcing weak candidates.

## Close by doing

End with action, not a list: "Want the first one running today?" — and hand over to **add-routine** or **build-routine** for the top pick. Then append one line to `my/memory/discovery-log.md` (`YYYY-MM-DD: mirrored N weeks / prompts path — candidates: …, chosen: …`) — conclusions only, approved by the owner, never raw observations — commit (`discover YYYY-MM-DD: <one plain line>`), push.
