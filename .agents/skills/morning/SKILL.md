---
name: lifeos-morning
description: >-
  Activates when the user starts their day, says "morning", or requests a morning check-in to review yesterday's state and set today's focus.
---
> Read `AGENTS.md` (cold-start rule) before executing this protocol.

# Protocol: morning

Target: under 10 minutes. Don't turn this into a planning session.

**Read first, ask second (cold-start rule):** do all file reads — steps 1, 4, 4a, 5, 6 —
*before* the step-2 question, so the question lands as a check-in from someone who
already knows the picture, not a report request.

1. Read `habits/log/[yesterday].md` and `reviews/daily/[yesterday].md` if they exist
   — including yesterday's State line. If it was a rough one (energy at the bottom,
   stress at the top), size today accordingly: one focus, nothing added, gentler
   framing. Don't mention the numbers unless the user does; just let them shape
   the day you propose.
2. Ask one question: "How did yesterday end — anything to carry forward?"
3. After response: mark habits in yesterday's log (ask which were done if unclear)
3a. **State backstop.** If yesterday's evening was skipped (no State line in
    `reviews/daily/[yesterday].md`), capture yesterday's state now as part of "how did
    yesterday end" — the three scales, 1–5 — and log it to yesterday's daily review. The
    evening check-in is the ideal (same-day is more accurate); the morning is the
    **backstop** so the state line never goes dark — state that lives only in the evening
    disappears whenever the evening slips.
4. Check `inbox.md` — flag anything time-sensitive
4a. **Events check** (`events.md`): surface any event dated *today*, plus any whose lead-time
    nudge window opens today. **If it's Monday, also surface the coming 7 days' events** so the
    week starts with them in view. Handle sensitive dates gently, with weight.
5. Glance at `todos.md` "This week" section — surface anything overdue or blocking today
6. Reference today's theme from `schedule/themes.md`
7. State one sentence: today's single most important focus, grounded in current quarter goals
8. **Name today's active habits explicitly as reminders** — read `habits/active.md` and
   list each active (non-paused) habit by name so the user has them stated, not assumed.
   Don't grade them here; just surface them. A standing rule — never skip it, even on
   light mornings.
9. Write `habits/log/[today].md` with this morning's habit status
