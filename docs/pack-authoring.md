<p align="center"><a href="../README.md">← Home</a> · <b>English</b> · <a href="pack-authoring.pt.md">Português</a></p>

# ✍️ Pack-authoring guide

How we design, write and ship a pack. Read this before your first module; it takes about ten minutes.

**Contents:** [What makes a good pack](#what-makes-a-good-pack) · [Design in 5 steps](#design-in-5-steps) · [Writing a module](#writing-a-module) · [Privacy rules](#privacy-rules) · [Quality bar](#quality-bar) · [Shipping](#shipping)

## What makes a good pack

A pack is a routine someone already runs by hand, written down so anyone's Instinct can run it. The good ones share four traits:

| Trait | Means | Test |
|-------|-------|------|
| **One job** | It solves one recurring problem ("my inbox", "my family's logistics") | You can say what it does in one sentence |
| **Few touchpoints** | It shows up at fixed, useful moments, not all day | Count the scheduled messages per day. Fewer than 4? Good |
| **Adapts** | It scales down on hard days instead of piling on | Ask "what happens if the user ignores it for 3 days?" |
| **Safe by default** | It never acts for the user without a yes | Search for "send", "book", "buy", "delete". Each one needs a confirmation step |

## Design in 5 steps

1. **Start from a real routine.** Yours, or one from a [pack request](https://github.com/olserra/assistant-packs/issues?q=is%3Aissue+is%3Aopen+label%3Apack-request). Write down what you do today, step by step.
2. **Cut it into modules.** Each module is one routine with one trigger (a time, an event, a request). Modules must work alone.
3. **List what is personal.** Every name, city, time, account or preference becomes a setup question. Nothing personal lives in the pack.
4. **Write the setup interview.** Up to 8 questions, asked in one or two messages, each with a default so "defaults" works.
5. **Write one example per module.** If you can't show what the message looks like, the module isn't clear yet.

Open a draft PR after step 2. Early feedback saves rewrites.

## Writing a module

Every module file in `references/` follows the same shape. Copy [morning-brief.md](../packs/configured-assistant/skills/configured-assistant/references/morning-brief.md) as a template.

```markdown
# Module name

**When:** trigger and default time.
**Goal:** what the user gets, in one sentence.

## Sections        (or Steps)
1. **emoji Title** - what goes here, how long, where the data comes from.

## Rules
- What to do when data is missing, the day is hard, or the user says stop.

## Example (shape only, values are illustrative)
```

Style notes:

- **Phone-sized.** Every message reads in under a minute.
- **Plain words.** "Send", not "dispatch". "Check", not "leverage".
- **Behavior, not buttons.** Describe what the assistant does ("every weekday at the user's morning time, send..."), not a product's menus. Product specifics go in [ADAPTERS.md](../ADAPTERS.md).
- **Live facts.** Weather, prices, news and schedules come from a live source at send time. Say what to do when the source fails.
- **Illustrative examples.** Values in examples are generic and obviously made up.

## Privacy rules

These are hard rules. A PR that breaks one is closed until fixed.

1. **No real people.** No names, initials, handles, photos or descriptions that point to a real person. Use "a family member", "your manager", `{{name}}`.
2. **No real organizations tied to you.** No employer, client, school or clinic names. Generic public services ("a weather service") are fine.
3. **No places you live or go.** No home city, neighborhood, address, gym or office. Use `{{city}}`.
4. **No contact details or accounts.** No phone numbers, emails, usernames, account IDs, links to private docs.
5. **No sensitive life details.** Nothing about health, relationships, finances, religion or legal matters, even anonymized.
6. **No secrets.** No API keys, tokens or passwords, not even fake-looking ones.
7. **Personal data is asked, never stored in the pack.** The setup interview collects it; the assistant keeps it.

Quick check before every PR: search your files for `@`, digits that look like phone numbers, capitalized names, and the name of your own city.

## Quality bar

Copy this checklist into your PR description.

```markdown
- [ ] Solves one recurring job, described in one sentence in the README
- [ ] Every module works alone and has When / Goal / Rules / Example
- [ ] Setup interview: 8 questions or fewer, each with a default
- [ ] Anything that sends, books, buys, deletes or changes shared data asks first
- [ ] Missing or failed data is handled ("markets unavailable today"), never guessed
- [ ] Hard days: the module scales down instead of adding pings
- [ ] Every scheduled message reads in under a minute on a phone
- [ ] Privacy rules pass (no people, places, accounts, sensitive details, secrets)
- [ ] pack.yaml lists modules, requires, languages and credits
- [ ] README (EN) done; README.pt.md done or marked as help wanted
- [ ] I installed it on my own assistant and ran every module at least once
```

## Shipping

1. Put the pack in `packs/<pack-id>/` following [FORMAT.md](../FORMAT.md).
2. Add yourself to `credits` in `pack.yaml` and to [CONTRIBUTORS.md](../CONTRIBUTORS.md).
3. Open a PR with the quality-bar checklist. If it answers a request, write `Closes #<number>`.
4. A maintainer reviews within a few days. We may ask for small changes; that's normal.
5. Once merged, we add it to the packs table, create its install-counter issue and credit you on the pack page.

Questions? Ask in [Discussions](https://github.com/olserra/assistant-packs/discussions).
