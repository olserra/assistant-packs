<p align="center"><a href="../README.md">← Home</a> · <b>English</b> · <a href="translating.pt.md">Português</a></p>

# 🌍 Translating a pack

Translations are the fastest way to make a pack useful to more people, and a great first contribution. You need a GitHub account and the language. No coding.

## Where files go

Each language has its own skill folder next to the English one, with the language code as a suffix:

```text
packs/configured-assistant/skills/
  configured-assistant/        English (source)
  configured-assistant-pt/     Portuguese
  configured-assistant-es/     Spanish   ← you create this
```

Module file names are translated too (Portuguese uses `resumo-matinal.md` for `morning-brief.md`). Then add the path to `pack.yaml` under the module:

```yaml
  - id: morning-brief
    en: references/morning-brief.md
    pt: references/resumo-matinal.md
    es: references/resumen-matutino.md
```

**Partial translations are welcome.** A folder with one module is a fine PR. The language is added to `languages:` in `pack.yaml` once its `SKILL.md` and all modules are translated.

## How to translate

- **Meaning over words.** It should read as if it was written in your language.
- **Keep the structure.** Same sections, same order, same emoji headers, same rules. Don't drop a rule to make it shorter.
- **Informal and short.** Packs talk to the user like a helpful friend: "tu" in Portuguese, French and Spanish.
- **Translate the examples**, keeping values illustrative. Adapt formats (24h time, decimal comma) to the language.
- **Keep placeholders** like `{{city}}` as they are.

## Glossary

| English | Português (PT) | Español | Français |
|---------|----------------|---------|----------|
| morning brief | resumo da manhã | resumen de la mañana | briefing du matin |
| evening brief | resumo da noite | resumen de la noche | briefing du soir |
| coaching ping | lembrete de coaching | recordatorio de coaching | rappel de coaching |
| scoreboard | placar | marcador | tableau des scores |
| watcher | vigilante | vigilante | veilleur |
| setup interview | entrevista de configuração | entrevista de configuración | questionnaire de configuration |
| streak | sequência | racha | série |

Suggestions to the glossary are welcome in the same PR.

## Open translation tasks

See issues labelled [`translation`](https://github.com/olserra/assistant-packs/issues?q=is%3Aissue+is%3Aopen+label%3Atranslation). Comment "I'll take this" before starting.
