# Protocol: month review

Run on the last day of the month.

1. Read all weekly reviews from this month
2. Score each life area 1–5 with one honest sentence each
3. Chart the state curve across the weeks (the three scales' averages, week by
   week). Name what moved and what likely moved it. This is where slow trends
   become visible.
4. Check progress against monthly milestones in `goals/areas/`
4a. **Annual objective reminder.** Read the annual objectives in `goals/year.md` and restate
    them plainly — is the year on track, and did this month serve it? (Monthly surfacing of the
    year, so the annual layer never goes dark.)
4b. **KR check.** Restate this quarter's KRs (`goals/this-quarter.md`, tagged to the annual
    objectives) and mark movement; flag any stalled KR, and any objective going unserved.
5. Write `reviews/monthly/YYYY-MM.md` — include a `## State curve` section with
   the week-by-week numbers and one paragraph of reading
6. Ask: "Is there a habit that should be retired, added, or scaled up?"
6a. **Distill and rotate reflections.** Go through this month's entries in
    `meta/reflections.md`: anything that has hardened into a durable rule graduates to
    its home (`context/operating-manual.md` for how-I-work rules, `context/people.md`
    for person-specific rules, the Current Season block for season-level rules) — state
    each graduation to the user before writing it. Then move the month's raw entries to
    `meta/reflections-archive-[YEAR].md`, keeping in `meta/reflections.md` only the
    current month and a short "Active patterns" header (max ~10 lines) of what's still
    being watched. Reflections is a capture buffer, not a warehouse.
6b. **Finance roll-up.** If the finances system is in use, read the month's entries in
    `finances/log/` (the last weekly entry carries the month summary). One paragraph in
    the review: totals in/out, commitments progress, trend. If no entries exist, note
    the gap — don't skip silently.
7. Propose one edit to the Current Season block in CLAUDE.md if priorities have shifted
8. **Cascade check.** If this is the last month of a quarter (Mar / Jun / Sep / Dec), tell the
   user the **quarter review is due**. If it's December, flag that the **annual review** is due
   after the quarter.
