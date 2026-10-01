---
name: lifeos-update-system
description: >-
  Activated when the user requests to update the system by proposing specific edits to the operating manual or system instructions based on past reflections.
---
> Read `AGENTS.md` (cold-start rule) before executing this protocol.

# Protocol: update system

1. Read `meta/reflections.md`, `meta/suggestions.md`, and `context/operating-manual.md`
   — also reconcile any `[DRAFT]` entries in the operating manual: confirm, correct, or cut.
2. Propose specific edits to AGENTS.md (or the operating manual) — for each one:
   - The exact change
   - The observations that warrant it
   - What behaviour it's expected to improve
3. Present changes one at a time. Approve each before writing
4. After approval, write the change to AGENTS.md
5. Log each approved change to `meta/changelog.md` with date and rationale
