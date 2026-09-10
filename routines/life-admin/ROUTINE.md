# Life admin — routine prompt

You are running inside the owner's private copy of their routine kit. Read `my/profile.md` first, then `CLAUDE.md`'s rules — they apply to every step below.

**IRON LAW.** Warn only — never cancel, book, renew, pay, or email anyone about any of these dates • the dates file is the single source of truth: never invent a date, and never silently "fix" one that looks wrong (flag it instead) • warn inside the warning window and not before — a warning that fires too early teaches the owner to ignore warnings • on a day with nothing due, create no event and send no ping.

The owner is {{owner_name}} (timezone {{timezone}}).

## Steps

1. Read `my/dates.md` — each entry has a name, a date (some yearly like birthdays, some one-off like a contract end), a warning lead time, and optionally what-to-do notes. Read the tail of `my/memory/life-admin-log.md` to see what's already been warned about; each entry gets **one** warning when it enters its window and at most one reminder at {{final_reminder_days}} days out — never a daily drumbeat.
2. Compute today's date in {{timezone}} and find every entry now inside its warning window and not yet warned (or due its final reminder).
3. {{calendar_enabled}}For each, create a calendar event today at {{digest_time}} {{timezone}}, 15 minutes, no guests — title: the entry's own emoji if it has one (else 🎂 for people, ⚠️ for money/contracts) + a phone-glance line ("Ana's birthday in 10 days — gift time"); description: the what-to-do notes from the file and the exact remaining time. If event creation fails, that must not fail the run: put the warning in your report and say the calendar write failed.
4. If an entry's date is malformed, past without resolution, or ambiguous, do not guess — list it in the report as needing the owner's attention.
5. Append one line to `my/memory/life-admin-log.md`: `YYYY-MM-DD: warned about X, Y` (or `all quiet`). Commit with message `life-admin YYYY-MM-DD: N warnings` (or `all quiet`), and push. If the push fails, keep the commit, report it plainly, and continue.
6. **Report — always, even on an all-quiet day.** One short paragraph: what was warned about, anything in the file needing attention, or the quiet verdict.
