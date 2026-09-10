# Runtimes — what the kit needs, and where it's been verified

The kit's soul is portable on purpose: plain-markdown instruction sheets, a git repo as memory, and a safety contract any capable agent can read. What varies by runtime is the plumbing. This page is the honest map.

## The four things a runtime must provide

1. **A scheduler** — something that runs an agent on a cron, with your copy of this repo cloned for it.
2. **Reach into your accounts** — read access to your mail/calendar, however your assistant connects to them.
3. **Git hands** — the ability to commit and push to your copy (the helpers' notebook).
4. **A digest channel** — somewhere glanceable for reports (a calendar event is the kit's favorite).

Anywhere those four exist, the sheets in `routines/` can run. The *interactive* half of the kit (setup, building, discovery, community) needs even less: just an agent in your copy that reads files — see `AGENTS.md`.

## The map, honestly

| Runtime | Interactive half | Scheduled half | Status |
|---|---|---|---|
| **Claude Code** (claude.ai/code) | native — skills auto-route | **Routines** (claude.ai/code/routines) + connectors | ✅ **Verified reference** — every claim in the docs was field-tested here |
| **OpenAI Codex** | reads `AGENTS.md` natively; skills are the same open format | **Automations** (cron + prompt + skills); Gmail-class connectors vary | 🔎 Ingredients present, **unverified** — [be the champion](https://github.com/crblabs/everyday-agents/issues/7) |
| **Grok Bots** | can read the repo and follow sheets | **Bot routines** on a persistent cloud computer; Gmail/Calendar plugins exist | 🔎 Ingredients present, **unverified** — and note Grok's culture includes agents that *act outward* (calls, purchases); the kit's floor forbids that, so fidelity matters doubly |
| **Gemini CLI, Cursor, others** | Agent Skills format is shared; `AGENTS.md` routes | check what your tool schedules | 🔎 Unverified |

**What "unverified" means**: the sheets are readable and the ingredients exist, but nobody has walked the full loop there and reported back. The first person who does becomes that port's champion — file a field report and the map updates.

## Two honesty notes that don't vary

- **The safety floor travels as prose, not as enforcement.** "Never send, delete, or spend" is written into every sheet; how faithfully a runtime's agent honors it is a property of that runtime. It has been verified on Claude. The sheets are deliberately written as explicit, checkable gates ("show the exact text", "get an unambiguous yes") so any runtime's behavior can be audited against them.
- **The interviews were tuned for one interpreter.** The conversational skills (setup, discover, build) were written and tested with Claude as the interpreter. Another model following the same file may interview more clumsily — the file is the contract; the warmth is the interpreter's.

## Per-skill portability

Most skills port clean — they're conversations plus file edits. The exceptions, marked honestly:

| Skill | Portability note |
|---|---|
| setup / build-routine / add-routine (scheduling steps) | The *scheduling* step is per-runtime: Claude → the routines page or schedule skill; Codex → an automation; Grok → a bot routine. Everything before and after those steps is portable. |
| checkup | Its "scheduler's truth" check is Claude-specific; the portable fallback it already contains (registry vs. git log vs. memory gaps) works everywhere. |
| power-up | Interactive installs use each collection's own per-runtime mechanism (it already says so); the vendoring path is portable. |
| everything else | Portable as written. |

## For contributors

Keep sheets **runtime-neutral**: name services ("Gmail", "your calendar"), never runtimes; let scheduling steps point here instead of naming one scheduler. It's part of the [review rubric](../CONTRIBUTING.md).
