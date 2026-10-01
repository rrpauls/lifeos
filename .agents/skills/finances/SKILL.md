---
name: lifeos-finances
description: >-
  Activated when the user asks to run a weekly money check-in, often triggered by the word "finances" and accompanied by account statements or screenshots.
---
> Read `AGENTS.md` (cold-start rule) before executing this protocol.

# Protocol: finances

Weekly money check-in. Trigger: `finances` — normally with account statements attached
(exports/screenshots/PDFs from any account) plus the user's comments. Statements are
parsed, never stored — the numbers land in the log, the source files stay wherever
the user keeps them.

1. Read `finances/overview.md` (accounts, recurring flows, commitments) and the most
   recent entry in `finances/log/`.
2. Parse the uploaded statements + comments. Ask at most ONE clarifying question,
   only if a number genuinely can't be placed.
3. Write `finances/log/[YEAR]-W[WEEK].md`:

   ```
   # Finances — YYYY-W## (dates)

   ## Balances
   | Account | Balance | Δ vs last entry |

   ## In this week
   - [source — amount — note]

   ## Out this week (significant only — not every coffee)
   - [item — amount — note]

   ## vs Plan
   [One line per active commitment: on track / ahead / behind + number]

   ## Flags
   - [anomalies: unknown charges, doubled subscriptions, missed expected inflows,
     renewal dates approaching]

   ## One suggestion
   [Exactly one, or "none this week." Never a list.]
   ```

4. Update `finances/overview.md` only when something structural changes (new account,
   new recurring flow, commitment added/completed/resized).
5. **Cascade check:** at the last weekly entry of a month, write a month roll-up section
   at the bottom of that entry (totals in/out, commitments progress, one-line trend) —
   the month review reads it. Quarter reviews read the month lines against the
   Financial-area goals.

Notes:
- Same honesty rules as habit tracking: numbers are observations, not grades.
  A bad money week logged plainly is the system working.
- One suggestion per week maximum — same principle as one adjustment per week review.
- Sensitive data: Privacy depends on the environment where the agent runs. Never quote full account numbers
  in logs — last 4 digits at most.
