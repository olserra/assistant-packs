# Assistant Packs

**Ready-made packs that turn a blank AI assistant into a configured chief of staff.**

[Português](README.pt.md) · [Pack format](FORMAT.md) · [Adapters](ADAPTERS.md) · [Contribute](CONTRIBUTING.md) · [Request a pack](https://github.com/olserra/assistant-packs/issues/new?template=pack-request.yml)

Most people get a personal AI assistant and then stare at an empty chat box. The useful setups (a morning brief that actually helps, an evening plan for tomorrow, one accountability nudge a day, watchers that warn you before things go wrong) take weeks of trial and error to get right.

A **pack** is that trial and error, written down once and shared. You install it, answer a few setup questions, and your assistant starts working the way a good chief of staff would.

## How it works

1. **Pick a pack** from the catalog below.
2. **Install it** in your assistant. Packs are plain Markdown in the open [Agent Skills](https://agentskills.io/specification) `SKILL.md` format, with short [adapter notes](ADAPTERS.md) for Instinct, Claude, ChatGPT and open-source agents.
3. **Answer the setup questions.** Every pack starts with an interview: your city, your hours, what matters to you. No personal data lives in the pack itself.
4. **Tell others it worked.** React 👍 on the pack's [install issue](https://github.com/olserra/assistant-packs/issues/1). That is the install counter.

## Catalog

| # | Pack | What it does | Status |
|---|------|--------------|--------|
| 1 | [The Configured Assistant](packs/configured-assistant/) | Morning brief, next-day evening brief, one daily accountability ping, weekly points scoreboard, event watchers, coaching cadence | ✅ Live (EN + PT) |
| 2 | Inbox Zero Chief | Triage rules, reply drafts in your voice, weekly unsubscribe sweep | 🔜 Coming soon |
| 3 | Family Logistics | Shared calendars, school deadlines, pickups, birthdays and gifts | 🔜 Coming soon |
| 4 | Job Search Copilot | Pipeline tracking, interview prep briefs, follow-up nudges | 🔜 Coming soon |

Want a different one? [Request a pack](https://github.com/olserra/assistant-packs/issues/new?template=pack-request.yml) and 👍 the [requests](https://github.com/olserra/assistant-packs/issues?q=is%3Aissue+is%3Aopen+label%3Apack-request) you want most. The most-voted requests get built first.

## Principles

- **Neutral format.** One pack, many assistants. The core is a portable `SKILL.md`; adapters cover the differences.
- **Zero personal data.** Packs are templates. Your details are collected at install time and stay in your assistant.
- **Adapt, don't nag.** Good assistants scale down on hard days instead of piling on.
- **Small and composable.** Each module works alone. Install the whole pack or just the morning brief.

## Repository layout

```
packs/
  <pack-name>/
    pack.yaml            # metadata: name, version, languages, modules, credits
    README.md            # what it does, in plain English
    README.pt.md         # same in Portuguese
    INSTALL.md           # copy-paste install prompts
    skills/
      <pack-name>/        # English skill
        SKILL.md
        references/*.md   # one file per module
      <pack-name>-pt/     # Portuguese skill
.github/ISSUE_TEMPLATE/   # pack request form
```

## Contributors

Every merged pack or improvement is credited in [CONTRIBUTORS.md](CONTRIBUTORS.md) and in the pack's own `pack.yaml`. See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

[MIT](LICENSE).
