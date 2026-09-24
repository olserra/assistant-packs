<p align="center"><a href="../README.pt.md">← Início</a> · <a href="translating.md">English</a> · <b>Português</b></p>

# 🌍 Traduzir um pack

As traduções são a forma mais rápida de tornar um pack útil a mais gente, e uma ótima primeira contribuição. Precisas de uma conta GitHub e do idioma. Sem programação.

## Onde ficam os ficheiros

Cada idioma tem a sua pasta de skill ao lado da inglesa, com o código do idioma como sufixo:

```text
packs/configured-assistant/skills/
  configured-assistant/        inglês (original)
  configured-assistant-pt/     português
  configured-assistant-es/     espanhol   ← crias esta
```

Os nomes dos ficheiros dos módulos também se traduzem (o português usa `resumo-matinal.md` para `morning-brief.md`). Depois acrescenta o caminho no `pack.yaml`, dentro do módulo:

```yaml
  - id: morning-brief
    en: references/morning-brief.md
    pt: references/resumo-matinal.md
    es: references/resumen-matutino.md
```

**Traduções parciais são bem-vindas.** Uma pasta com um só módulo é um bom PR. O idioma entra em `languages:` no `pack.yaml` quando o `SKILL.md` e todos os módulos estiverem traduzidos.

## Como traduzir

- **Sentido acima das palavras.** Deve ler-se como se tivesse sido escrito no teu idioma.
- **Mantém a estrutura.** Mesmas secções, mesma ordem, mesmos emojis, mesmas regras. Não cortes uma regra para encurtar.
- **Informal e curto.** Os packs falam com o utilizador como um amigo prestável: "tu" em português, francês e espanhol.
- **Traduz os exemplos**, com valores ilustrativos. Adapta formatos (hora 24h, vírgula decimal) ao idioma.
- **Mantém os marcadores** como `{{city}}` tal como estão.

## Glossário

| English | Português (PT) | Español | Français |
|---------|----------------|---------|----------|
| morning brief | resumo da manhã | resumen de la mañana | briefing du matin |
| evening brief | resumo da noite | resumen de la noche | briefing du soir |
| coaching ping | lembrete de coaching | recordatorio de coaching | rappel de coaching |
| scoreboard | placar | marcador | tableau des scores |
| watcher | vigilante | vigilante | veilleur |
| setup interview | entrevista de configuração | entrevista de configuración | questionnaire de configuration |
| streak | sequência | racha | série |

Sugestões para o glossário são bem-vindas no mesmo PR.

## Traduções em aberto

Vê as issues com a etiqueta [`translation`](https://github.com/olserra/assistant-packs/issues?q=is%3Aissue+is%3Aopen+label%3Atranslation). Comenta "fico com esta" antes de começar.
