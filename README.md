# LifeOS

**A plain Markdown framework for working with the parts of life that matter to you.**

LifeOS gives an AI agent a consistent structure for goals, routines, projects, important dates, and regular reviews. The files are editable Markdown, and the workflows are defined in a vendor-neutral core with adapters for supported agents.

## What it provides

- A hierarchy for annual objectives and quarterly key results.
- Routines and check-ins that can be adapted to the user.
- Daily, weekly, monthly, quarterly, and annual review protocols.
- A working inbox, tasks, projects, and important dates.
- A cold-start approach that loads available state before asking questions.
- Explicit rules for file updates, personal context, and one question at a time.

The framework is a starting point. Personalize an initialized copy to fit your needs.

## Architecture

`AGENTS.md` defines the shared behavior. `protocols/` contains the trigger workflows. Agent-specific files are thin adapters that direct each environment to the same core.

| Agent | Adapter |
|---|---|
| Antigravity | `.agents/GEMINI.md` and `.agents/skills/` |
| Claude Code | `CLAUDE.md` |
| ChatGPT Web | `CHATGPT.md` |
| Codex | `codex.md` |
| OpenClaw | `SOUL.md`, `USER.md`, and `IDENTITY.md` |
| Hermes | `meta/hermes-setup.md` |

The public reusable framework is [`rrpauls/lifeos`](https://github.com/rrpauls/lifeos), a fork of [`jeanjmauris/lifeos`](https://github.com/jeanjmauris/lifeos).

## Setup

Clone the framework and open its directory in an agent environment that can read and edit Markdown:

```bash
git clone https://github.com/rrpauls/lifeos.git ~/lifeos
cd ~/lifeos
```

Read `AGENTS.md`, then use `hello` to personalize an initialized copy. Keep that personal instance in a private repository or a local environment you control. Do not commit initialized personal LifeOS state to this public framework repository.

## Privacy

LifeOS is stored as plain Markdown. Privacy depends on the environment where the agent runs. Never publish or commit personal state unintentionally. The tracked state directories and files are part of the framework's starter tree; they are not a safe destination for personal data in this public repository.

The repository has no build step, runtime dependencies, or startup command. See [`CLOUD_SETUP.md`](CLOUD_SETUP.md) for cloud-environment notes.

## Make it yours

After creating a private or local initialized copy, edit the life areas, files, and protocols to suit your needs. Keep `AGENTS.md` as the canonical behavior and maintain the thin adapters for whichever agents you use.

## License

MIT — see [LICENSE](LICENSE).
