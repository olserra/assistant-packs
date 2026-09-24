# Using a pack outside Instinct

Packs are written for [Instinct](https://instinct.com) first; the [README](README.md) covers that path. If you use another assistant, these notes help.

Every pack's core is a portable `SKILL.md`. Assistants differ in two things: **how you add instructions** and **whether they can act on a schedule**. These notes cover both. If your assistant cannot run things on a schedule, every module still works on demand ("run my morning brief").

Capabilities a pack may use: scheduled messages, web search, calendar read, email read, reminders. Each pack lists what it needs in `pack.yaml` under `requires`.

## Instinct

- **Install:** open [INSTALL.md](packs/configured-assistant/INSTALL.md), copy the prompt for your language and send it to your Instinct in chat. It will run the setup interview and schedule the routines.
- **Scheduling:** native. Briefs and the daily ping arrive on the channel you already use with it.
- **Watchers:** native, when your calendar and email are connected.
- **Tip:** say "show me tomorrow's evening brief now" right after setup to check the format before the first scheduled one.

## Claude

- **Install:** add the skill folder (`skills/<pack-id>/`) as a Skill. See Anthropic's [Agent Skills overview](https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview) for where skills go in your Claude surface.
- **Scheduling:** depends on your setup. Where scheduled runs are not available, trigger modules on demand ("morning brief").
- **Watchers:** need calendar/email connectors; otherwise run the check manually.

## ChatGPT

- **Install:** paste the INSTALL prompt into a new chat or a Project, or put the `SKILL.md` body into a custom GPT's instructions.
- **Scheduling:** use scheduled tasks where your plan offers them; one task per module (morning, evening, midday ping, Sunday scoreboard).
- **Watchers:** limited to what your connected apps allow; fall back to on-demand checks.

## Open-source agents

- Any agent that reads the [Agent Skills](https://agentskills.io/specification) format can load `skills/<pack-id>/` directly.
- Wire the schedule with your agent's scheduler or plain cron calling the agent with the module name.
- Keep the user's setup answers in the agent's own memory or a local config file, never in the pack folder.

## Adding an adapter

Open a PR that adds a section here. Keep it to install, scheduling and watchers, with a link to the assistant's official docs.
