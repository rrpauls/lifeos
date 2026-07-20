# Protocol: events

Manage and surface events — one-time and recurring (birthdays, anniversaries, deadlines),
mostly tied to people in `context/people.md`. Events live in `events.md`.

## On the `events` trigger
1. Read `events.md`.
2. Show upcoming events for the next 30 days, soonest first, each with who it's tied to and
   its lead-time nudge.
3. Add / edit / remove as asked. **Recurring** events use `MM-DD`; **one-time** use `YYYY-MM-DD`.
   Each event may carry a **lead-time nudge** (days before) so there's time to act.

## Automatic surfacing (no trigger needed — wired into other protocols)
- **Daily (morning protocol):** surface any event dated *today*, plus any whose lead-time
  window opens today (e.g. an anniversary with a 5-day nudge, surfaced 5 days out).
- **Weekly (Monday morning):** surface every event falling in the coming 7 days, so the week
  starts with them in view.

## Handling
- Tie events to people where relevant; a person's key dates can also live in `context/people.md`.
- **Sensitive events** (a loss anniversary, a hard date) — surface gently, with weight, no
  frameworks or solutions. Name it, then follow the person's lead.
- The lead-time nudge exists so meaningful dates never sneak up (e.g. an anniversary that needs
  a gift or a plan). Default nudge: 3 days; longer for dates that need real preparation.
