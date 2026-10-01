# ChatGPT Web adapter

Read [`AGENTS.md`](AGENTS.md) before acting. It is the canonical LifeOS configuration. Use the LifeOS repository configured for the current project as the authoritative versioned source. `AGENTS.md` and `protocols/` define canonical LifeOS behavior.

For a LifeOS trigger, read the matching file in `protocols/` first. Apply the cold-start and file-write rules in `AGENTS.md`, and ask one question at a time. Repository state outranks ChatGPT memory. Never invent unavailable local or git-ignored state; say when required state is unavailable and continue from what is accessible.

LifeOS is stored as plain Markdown. Privacy depends on the environment where the agent runs. Never publish or commit personal state unintentionally.
