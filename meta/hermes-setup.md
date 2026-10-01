# Hermes setup for LifeOS

This guide connects Hermes Agent to a LifeOS copy. Configure Hermes to use the directory containing the initialized LifeOS files; that directory may be local or provided through a cloud environment.

## Instructions

At session start, read `AGENTS.md`. For a LifeOS trigger, read the matching protocol in `protocols/` and follow the cold-start and file-write rules. Use the Hermes `SOUL.md` and `USER.md` adapters only when that installation supports them.

The `.agents/skills/` directory contains protocol skills that may be copied into a Hermes skills directory if the installed Hermes version supports the same `SKILL.md` format. Check the current Hermes documentation for its supported configuration paths and scheduling features.

LifeOS is stored as plain Markdown. Privacy depends on the environment where the agent runs. Never publish or commit personal state unintentionally. Keep initialized personal data in a private or local instance, not in the public framework repository.
