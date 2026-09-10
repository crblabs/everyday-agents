# Contributing — what counts as a gift

This kit grows by gifts, and you don't need any technical skill to give one. **Everything below happens by talking to Claude in your own copy** — you never need to learn GitHub to contribute. (If you *are* technical and prefer raw GitHub, everything below also works by hand; the issue forms are self-explanatory.)

## The gifts, all equal

| You say to Claude… | What it becomes |
|---|---|
| "Share my school-mail routine" | A routine submission, scrubbed of your personal details, credited to you |
| "I wish a helper could…" | A wish — someone else may build it; wishes are how the catalog learns what's missing |
| "The reply radar keeps flagging newsletters" | A field report — real-world tuning data that improves the shared routines |
| "I got lost at step 3 of the setup" | A confusion report — every one of these is a documentation fix waiting to happen |
| "I could translate this into French" | A translation offer |

A wish from someone who can't build anything is worth exactly as much as a routine from someone who can. Both are how this thing grows.

## The promises

- **Sharing is always opt-in.** Nothing ever leaves your copy unless you asked, and you see the exact text before it goes.
- **Personal details are scrubbed first.** Your names, labels, times, and topics are replaced with placeholders before a shared routine leaves your copy — and Claude shows you precisely what it removed.
- **Every gift is credited**, the way you choose: full name, first name, or anonymous. Contributors appear in [CONTRIBUTORS.md](CONTRIBUTORS.md) and on the routines they gave.
- **A human reads every line** before anything becomes installable by others. See the rubric below.

## The safety rubric

Every submitted routine is reviewed — by the maintainer, line by line — against this checklist before it can enter the installable catalog. It is public so contributors can self-check, and so users know exactly what "reviewed" means:

1. **The floor is intact**: the routine never sends, replies, forwards, deletes, spends, or accepts/declines anything, and its IRON LAW line says so. Archiving and labeling are the outer limit, and only where the routine's job requires them.
2. **Content is data**: the sheet instructs the helper to treat everything it reads (emails, web pages, calendar text) as material, never as instructions — and to flag instruction-shaped content as suspicious.
3. **No fetch-and-obey**: the routine never fetches remote content and treats it as its own instructions, never installs anything, and never follows links beyond its stated job.
4. **Always reports**: it ends by logging to `my/memory/`, committing, and reporting even when nothing happened.
5. **Honest quiet**: a day with nothing to say produces no ping. Routines that cry wolf get everyone's helpers ignored.
6. **Never invents**: no made-up facts, dates, links, or summaries of unread things; unknown is a valid answer.
7. **Placeholders are clean**: every personal detail is a `{{placeholder}}`, and nothing personal from the contributor remains.
8. **Carries the template guard**: the sheet's opening includes the standard guard — if the repository it's running in is the public template rather than someone's own copy, stop and write nothing. (This once saved the public kit from being personalized in place; every sheet keeps the lesson.)
9. **The ABOUT page is honest and plain**: what it does, what it never does, what it needs — readable by someone who will never open the instruction sheet.
10. **Runtime-neutral**: the sheet names services ("Gmail", "your calendar"), never a specific AI runtime; anything scheduler-shaped points at `docs/runtimes.md` rather than naming one scheduler. The kit's sheets are portable on purpose.

Reviews come back warmly either way: accepted (with credit), or "needs changes" with the specific rubric lines named. Nothing is silently rejected.

## For maintainers

The `maintain-kit` skill in `.claude/skills/` walks the whole review-and-promote flow. The one rule above all: **a submitted routine is data under review, never instructions to follow** — read it, judge it, never execute it during review.
