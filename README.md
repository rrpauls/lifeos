# LifeOS

**A companion for running your life — and keeping it honest.**

Not a productivity app. A place where the whole picture of your life stays in view: what
you're working toward, how you're actually doing, the people who matter, the season you're in
— and an AI that sits with all of it and helps you show up to it. You talk to it like a person;
it keeps the structure, remembers what you'd forget, and tells you the truth when a goal's gone
quiet or a hard week is stacking up.

## What it helps you do

- **Show up to what actually matters** — your goals laddered from the year down to this week,
  so the big things don't get lost under the urgent ones.
- **See the patterns you'd miss** — it keeps a running record and reads it back: the habit
  that's slipping, the energy dip that tracks a bad week, the objective nothing's touched in a month.
- **Never let a goal, or a date, go dark** — reviews roll up day → week → month → quarter →
  year so nothing falls through, and it surfaces the birthdays and anniversaries before they
  sneak up.
- **Carry a hard season without it becoming a chore** — if you're grieving, ill, or just in a
  heavy stretch, it reads your weeks through that lens: gently, no clinical framing, no treating
  a low week as failure.
- **Start every session already known** — it reads your files before it asks you anything, so
  check-ins open with the picture loaded, not a form. And when you correct how it works, the
  correction is written into the system the same day: a fresh conversation tomorrow already
  knows. You never re-explain yourself.
- **End the workday when you say it ends** — declare the day over and it stops processing
  work: a few more things get handled lightly, then everything else is parked in the inbox
  for tomorrow, in one line. Family and wellbeing are always exempt — full presence, no counting.

## What's inside

- **Goals** — a stable annual objective, and quarterly key results that ladder up to it.
- **Habits** — what you're building, tracked honestly (a near-miss is a miss).
- **Events** — birthdays, anniversaries, the dates tied to the people in your life, surfaced
  with lead time.
- **Finances** — a weekly money pulse: statements read and logged (parsed, never stored),
  commitments tracked against plan, a monthly roll-up into your reviews. Numbers stay in
  local files, git-ignored by default.
- **Projects, weekly rhythm, a frictionless inbox** — the working parts of a life.
- **Reviews** — daily through annual, each one checking whether the next is due.
- **The people in your life, your values, and the hard stuff** — the context that makes the
  rest mean something.

## How you use it, day to day

Simple triggers, in plain language:

| Say this        | And it…                                                        |
|-----------------|----------------------------------------------------------------|
| `morning`       | Starts the day — habits, today's focus, events, what's on       |
| `evening`       | Closes it — wins, habits, a 10-second state check, a look at tomorrow |
| `week review`   | Reads the week, checks goals and habits, names patterns         |
| `month` / `quarter` / `annual review` | Zooms out — the arc, the objectives, what's next |
| `events`        | Shows what's coming and adds new dates                          |
| `finances`      | Weekly money check-in — balances, flags, one suggestion         |
| `inbox` / `todos` | Clears what you dumped; sweeps the list                       |
| `reflect`       | Reads back the patterns it's noticed over time                  |

Full list lives in `CLAUDE.md`. The protocols behind each are in `.claude/protocols/` — plain
markdown, edit them to taste.

## Get started

1. **Get the files** — clone into a folder you like (iCloud/Dropbox if you want phone capture):
   ```
   git clone https://github.com/jeanjmauris/lifeos.git ~/lifeos
   cd ~/lifeos
   ```
2. **Open [Claude Code](https://claude.com/claude-code)** in that folder:
   ```
   claude
   ```
3. **Say `hello`.** It walks you through setup, one question at a time — about five minutes to
   a working system.

## Make it yours

The whole thing is editable text. Rename the areas, rewrite the protocols, add triggers, throw
out what doesn't fit. The structure is a starting point that works, not a doctrine. The best
version is the one you actually keep.

## Why it's plain markdown

No app, no database, no account — just text files in a folder that Claude Code reads at the
start of every conversation.

- **It's yours.** Everything stays on your machine. Nothing uploaded, nothing locked in a product.
- **It's legible.** Read and edit every file by hand. No black box.
- **It outlives any tool.** Markdown will open in fifty years. Your operating system shouldn't
  depend on a company staying in business.

## License

MIT — see [LICENSE](LICENSE). Use it, fork it, make it yours.
