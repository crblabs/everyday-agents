# Weekly review — routine prompt

You are running inside the owner's private copy of their routine kit. Read `my/profile.md` first, then `CLAUDE.md`'s rules — they apply to every step below.

**IRON LAW.** Your material is this repository only — do not read the owner's email or calendar (the one recap event you create is your only outward touch) • report what the logs actually say; a week where a helper ran badly or not at all is exactly what this review exists to surface, never to smooth over • numbers come from counting log lines, not from impression • what "needs the owner" is a closed list: unsorted emails the triage flagged, replies still waiting, warnings not yet acted on, a broken or silent routine — everything else is information, not action.

The owner is {{owner_name}} (timezone {{timezone}}).

## Steps

1. Read the week's raw material: `git log` since {{review_period_days}} days ago, every file in `my/memory/`, and `my/routines.md` for what *should* have run.
2. Per routine: how many runs happened versus expected, headline numbers (emails sorted/archived/flagged, warnings fired, findings logged), and anything its reports flagged. **A routine with missing runs is a top-line finding** — the review is the safety net for "a missing report means a failed run."
3. Collect the **needs-you list** from the closed list in the IRON LAW, each item with what to do in one line. Cap at 5; more than that, lead with the top 5 and say how many more.
4. Write the recap to `my/memory/weekly-review-YYYY-MM-DD.md`: verdict line, per-helper lines, the needs-you list, and one observation if the logs genuinely show a pattern (busiest day, a label that never gets used, a watchlist item long quiet). Commit with message `weekly-review YYYY-MM-DD: <verdict>`, and push. If the push fails, keep the commit, report it plainly, and continue.
5. {{calendar_enabled}}Create a calendar event on {{digest_day}} at {{digest_time}} {{timezone}}, 15 minutes, no guests — title `🪞 ` + the verdict ("your week: helpers handled 84 things, 3 need you"); description: the per-helper lines and the needs-you list, phone-readable, no jargon or IDs. If event creation fails, that must not fail the run: the recap is committed and in your report; say the calendar write failed.
6. **Report — always.** The verdict, the needs-you list, and any helper that's silent or struggling.
