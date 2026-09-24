# Pack format

A pack is a folder of plain Markdown and one YAML file. Nothing to compile, nothing to run.

## Files

| File | Required | Purpose |
|------|----------|---------|
| `pack.yaml` | yes | Metadata: id, name, version, languages, modules, credits, install issue |
| `README.md` / `README.pt.md` | yes (EN), PT encouraged | What the pack does, for humans |
| `INSTALL.md` | yes | Copy-paste install prompts, one per language |
| `skills/<pack-id>/SKILL.md` | yes | The portable skill, in the open [Agent Skills](https://agentskills.io/specification) format |
| `skills/<pack-id>/references/*.md` | optional | One file per module, loaded only when needed |
| `skills/<pack-id>-pt/` | optional | The same skill in Portuguese (or `-<lang>` for other languages) |

## SKILL.md

Follows the Agent Skills specification: YAML frontmatter with `name` (lowercase, hyphens, same as the folder) and `description` (what it does and when to use it), then Markdown instructions.

```markdown
---
name: configured-assistant
description: Sets up and runs a chief-of-staff routine ... Use when ...
---

# The Configured Assistant
...
```

## Rules every pack follows

1. **No personal data.** No names of people, employers, companies, places, phone numbers, emails, health or relationship details. Use placeholders like `{{city}}` or phrases like "a family member".
2. **Setup interview first.** The skill asks for everything personal at install time and stores it in the assistant, never in the pack.
3. **Modules stand alone.** A user can install one module without the rest.
4. **Assistant-neutral wording.** Describe behavior ("every day at the user's chosen morning time, send..."), not a specific product's buttons. Product specifics go in [ADAPTERS.md](ADAPTERS.md).
5. **Confirm before acting for the user.** Anything that sends messages, spends money or changes someone else's calendar must ask first unless the user grants a standing permission.
6. **Bilingual when possible.** English is required; Portuguese is encouraged.

## pack.yaml

```yaml
id: configured-assistant
name: The Configured Assistant
version: 0.1.0
status: live                         # live, or draft while contributors build it
languages: [en, pt]
summary: One-line pitch.
modules:
  - id: morning-brief
    file: references/morning-brief.md
requires: [scheduling, web-search]   # capabilities, not products
install_issue: 1                     # GitHub issue used as the install counter
credits:
  - github: your-handle
    role: author
```
