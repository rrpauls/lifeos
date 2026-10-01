---
name: lifeos-quarter-review
description: >-
  Activates at the end of the quarter, or when the user requests a quarterly review to score key results and draft the next quarter's goals.
---
> Read `AGENTS.md` (cold-start rule) before executing this protocol.

# Protocol: quarter review

Run at the end of the quarter.

1. Read all monthly reviews and the current quarter goal file
2. Score each **KR** in `goals/this-quarter.md`: % complete + one sentence, noting which annual
   objective it advanced. (Objectives are annual — `goals/year.md`; KRs ladder to them. No
   quarterly objectives; no separate annual KRs.)
3. Pull top 3 patterns from `meta/reflections.md`
4. Read the state curves from the monthly reviews — one paragraph on the quarter's
   arc (what recovered, what tracked up or down, and with what). If the season was
   about recovery or wellbeing, this paragraph is the headline result, ahead of OKRs.
5. Write `reviews/quarterly/YYYY-QN.md`
6. Draft next quarter's goal file: `goals/this-quarter.md` (archive the old one first) —
   **KRs only, each tagged to an annual objective** (no quarterly objectives)
7. **Annual alignment.** Read `goals/year.md`; score the quarter against each annual objective
   in one paragraph, and check next quarter's KRs serve them.
8. Propose specific edits to AGENTS.md based on what was learned
   — present as "Here's what I'd change and why." Approve before writing.
9. Log approved changes to `meta/changelog.md`
10. **Cascade check.** If this is the Q4 / year-end review (December), tell the user the
    **annual review is due** — run `annual-review.md` next.
