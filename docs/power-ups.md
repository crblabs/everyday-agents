# Power-ups — other people's excellent work

The kit is complete on its own, and **installs none of these by default**. But some people have built remarkable skill collections for Claude, and if your ambitions grow in their direction, standing on their shoulders beats rebuilding worse. This shelf is short and curated on purpose: each entry is something we genuinely admire, credited to the human behind it.

## The shelf

### 🧭 PM Skills — what Pawel is doing

[Pawel Huryn's pm-skills](https://github.com/phuryn/pm-skills): 68+ product-management skills — discovery interviews, PRDs, OKRs, pricing, go-to-market, growth loops — encoding the frameworks of Teresa Torres, Marty Cagan and others into guided workflows. *"Generic AI gives you text. PM Skills gives you structure."*

- **For**: anyone doing product work — founders included.
- **Install** (interactive sessions, official mechanism): `claude plugin marketplace add phuryn/pm-skills`, then install the plugins you want.
- **Trust line**: distributed through Claude's plugin marketplace; MIT-licensed; updates when you update it.
- **Its companion, [pm-brain](https://github.com/phuryn/pm-brain)**: a markdown second brain for PM knowledge — ingest → synthesize → weekly sweep, every claim provenance-tagged, all of it plain files in your repo. Philosophically a sibling of this kit (*"the memory lives in your repo, not in Claude"*), which makes it the most natural vendoring source on this shelf for product-work routines.

### 🏭 gstack — what Garry is doing

[Garry Tan's gstack](https://github.com/garrytan/gstack): a full AI software factory — plan reviews from CEO/eng/design perspectives, browser QA, security audit, ship-and-deploy, retros — built for *"founders and CEOs, first-time Claude Code users"*, with the ambition that one person ships like a team of twenty.

- **For**: founders building product with Claude end-to-end.
- **Install** (interactive sessions): one clone + setup script — see its README.
- **Trust line, stated plainly**: gstack **auto-updates itself at session start** from its repository. That's convenient — and it means you're opting into a standing feed of executable instructions maintained by someone else. We admire it *and* we name the trade.

### 🥋 Superpowers — obra's methodology

[Jesse Vincent's superpowers](https://github.com/obra/superpowers): a complete development *methodology* — test-driven development, systematic debugging, brainstorming and planning workflows — that activates automatically when relevant. Narrower than gstack, deeper where it goes: *"mandatory workflows, not suggestions."*

- **For**: engineers who want discipline more than breadth.
- **Install** (interactive sessions): `/plugin install superpowers@claude-plugins-official` — the official Anthropic marketplace, the most vetted channel there is.
- **Trust line**: official-marketplace distribution; MIT.

## Which one? (opinionated, by who you are)

| You are… | Start with | The alternative |
|---|---|---|
| Doing product/PM work | **PM Skills** | — |
| A founder who wants the whole factory | **gstack** | Superpowers, if you'd trade breadth for discipline |
| An engineer who wants rigor | **Superpowers** | gstack, if you also want design/QA/ship |

## Powering your *routines* with them

Installing a power-up reaches your interactive conversations — **not** your scheduled helpers, which run in the cloud with only your copy's files. To give a *routine* a power-up skill, the kit's way is **vendoring with consent**: say **"power up my routines with …"** and Claude copies the specific skills you choose into your copy under `powerups/`, each stamped with where it came from and which version. Your helpers then use your copy — stable, auditable, offline from upstream. Updates happen only when you say "update my power-ups", with the changes summarized first. Nothing external ever updates itself inside your copy.

## The rules of this shelf

- **The kit never installs any of these for you** — every install is your explicit ask.
- **External means external**: these are third-party instruction sets we admire but do not review. Their tier is said out loud whenever one enters your copy — same as everything else here.
- Know a collection that belongs on this shelf? Say "I wish the shelf had …" — [that's a contribution](community.md).
