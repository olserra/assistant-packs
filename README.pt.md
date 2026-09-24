# Assistant Packs

**Packs prontos que transformam um assistente de IA em branco num chefe de gabinete já configurado.**

[English](README.md) · [Formato dos packs](FORMAT.md) · [Adaptadores](ADAPTERS.md) · [Contribuir](CONTRIBUTING.md) · [Pedir um pack](https://github.com/olserra/assistant-packs/issues/new?template=pack-request.yml)

A maioria das pessoas ganha um assistente de IA pessoal e fica a olhar para uma caixa de chat vazia. As configurações que realmente ajudam (um resumo matinal útil, um plano ao fim do dia para amanhã, um único lembrete de responsabilidade por dia, vigilantes que avisam antes de algo correr mal) levam semanas de tentativa e erro a acertar.

Um **pack** é essa tentativa e erro, escrita uma vez e partilhada. Instala, responde a algumas perguntas e o teu assistente passa a trabalhar como um bom chefe de gabinete.

## Como funciona

1. **Escolhe um pack** no catálogo abaixo.
2. **Instala-o** no teu assistente. Os packs são Markdown simples no formato aberto [Agent Skills](https://agentskills.io/specification) (`SKILL.md`), com [notas de adaptação](ADAPTERS.md) curtas para Instinct, Claude, ChatGPT e agentes open source.
3. **Responde às perguntas de configuração.** Cada pack começa com uma entrevista: a tua cidade, os teus horários, o que importa para ti. O pack não contém dados pessoais.
4. **Conta aos outros que funcionou.** Reage com 👍 na [issue de instalação](https://github.com/olserra/assistant-packs/issues/1) do pack. É esse o contador de instalações.

## Catálogo

| # | Pack | O que faz | Estado |
|---|------|-----------|--------|
| 1 | [O Assistente Configurado](packs/configured-assistant/README.pt.md) | Resumo matinal, resumo do dia seguinte à noite, um lembrete diário, placar semanal de pontos, vigilantes de eventos, cadência de coaching | ✅ Disponível (EN + PT) |
| 2 | Chefe da Caixa de Entrada | Regras de triagem, rascunhos de resposta no teu tom, limpeza semanal de subscrições | 🔜 Em breve |
| 3 | Logística Familiar | Calendários partilhados, prazos da escola, recolhas, aniversários e presentes | 🔜 Em breve |
| 4 | Copiloto de Procura de Emprego | Pipeline de candidaturas, briefings de entrevista, lembretes de follow-up | 🔜 Em breve |

Queres outro? [Pede um pack](https://github.com/olserra/assistant-packs/issues/new?template=pack-request.yml) e dá 👍 nos [pedidos](https://github.com/olserra/assistant-packs/issues?q=is%3Aissue+is%3Aopen+label%3Apack-request) que mais queres. Os mais votados são construídos primeiro.

## Princípios

- **Formato neutro.** Um pack, vários assistentes. O núcleo é um `SKILL.md` portátil; os adaptadores tratam das diferenças.
- **Zero dados pessoais.** Os packs são modelos. Os teus dados são recolhidos na instalação e ficam no teu assistente.
- **Adaptar, não chatear.** Um bom assistente reduz o ritmo nos dias difíceis em vez de acumular tarefas.
- **Pequeno e combinável.** Cada módulo funciona sozinho. Instala o pack inteiro ou só o resumo matinal.

## Contribuidores

Cada pack ou melhoria aceite fica creditado em [CONTRIBUTORS.md](CONTRIBUTORS.md) e no `pack.yaml` do próprio pack. Vê [CONTRIBUTING.md](CONTRIBUTING.md).

## Licença

[MIT](LICENSE).
