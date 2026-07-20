# Protocol: evening

1. Read today's habit log from `habits/log/[today].md`
2. Ask one question: "How did today go?" — let response complete before doing anything
3. Update today's habit log with completions
4. Ask for the state line, as one question: "State check — energy, motivation,
   stress, 1–5?" (Scales are configurable — see note below.) Numbers are
   observations, not grades — a 2-energy day logged honestly is the system working,
   not failing. Never moralize a number.
5. Write `reviews/daily/[today].md` using this format:

   ```
   # Daily Review — YYYY-MM-DD (Weekday)

   [One-line read of the day — honest, not summary-bland.]

   ## Wins
   - [even small ones]

   ## What didn't happen
   - [what] — [one honest sentence why]

   ## State
   energy N · motivation N · stress N
   [Optional: one line of context — what drove the numbers. No more.]

   ## Carry-forward
   - [one item for tomorrow]
   ```

6. If `inbox.md` has more than 3 unprocessed items, process them now
7. **Cascade check.** If today is Friday or a weekend day, check whether this week's weekly
   review exists in `reviews/weekly/`. If it doesn't, tell the user the **week review is due**
   before the week closes. (The roll-up guard — a smaller review always checks whether the
   next-bigger one is owed. See §Cascade note below.)

Notes:
- The State line is fixed-format so weekly/monthly reviews can read trends from it.
- **Cascade note:** the review chain is day → week → month → quarter → year. Each level's
  protocol ends by checking whether the next-bigger review is due, so nothing falls through.
  Never silently skip a due roll-up — surface it.
- The three scales are chosen at onboarding (defaults: energy, motivation, stress —
  rename to what matters: anxiety, focus, pain, whatever is live for this person).
  Keep them stable once chosen, or trends break.
- Don't comment on the numbers nightly. Trends are the week review's job — unless
  the user raises it, or a difficult scale sits at the bad end two days running
  (then one gentle question, per the Sensitive Context section if filled).
- Three scales only. Don't add a fourth until these have run a full month.
