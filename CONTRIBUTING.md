# Contributing

[English](#english) · [Português](#português)

## English

There are three ways to help, from quickest to biggest.

### 1. Vote and request

- 👍 the [pack requests](https://github.com/olserra/assistant-packs/issues?q=is%3Aissue+is%3Aopen+label%3Apack-request) you want. The most-voted get built first.
- Missing something? [Request a pack](https://github.com/olserra/assistant-packs/issues/new?template=pack-request.yml).
- Installed a pack? 👍 its [install issue](https://github.com/olserra/assistant-packs/issues/1). That is how install counts work.

### 2. Improve a pack

Found a better prompt, a clearer module, a missing adapter note, a translation fix? Open a pull request. Keep changes small and say what you tried and how it behaved.

### 3. Publish a new pack

1. Copy `packs/configured-assistant/` as a starting point and rename it.
2. Follow [FORMAT.md](FORMAT.md). English required, Portuguese encouraged.
3. Run the privacy check below.
4. Add yourself to `credits` in `pack.yaml` and to [CONTRIBUTORS.md](CONTRIBUTORS.md).
5. Open a PR. If it answers a pack request, write `Closes #<number>`.

### Privacy check (required)

Before opening a PR, search your pack for anything that identifies a real person or organization: names, employers, clients, addresses, cities you live in, phone numbers, emails, account names, health, relationships, finances. Replace them with placeholders (`{{city}}`, "a family member", "your team's CRM"). If unsure, leave it out. PRs that fail this check are closed without review.

### Credits

Every accepted contribution is credited in CONTRIBUTORS.md and in the pack's `pack.yaml`. Pack authors are shown on the pack page.

## Português

Há três formas de ajudar, da mais rápida à maior.

### 1. Votar e pedir

- Dá 👍 nos [pedidos de packs](https://github.com/olserra/assistant-packs/issues?q=is%3Aissue+is%3Aopen+label%3Apack-request) que queres. Os mais votados são construídos primeiro.
- Falta alguma coisa? [Pede um pack](https://github.com/olserra/assistant-packs/issues/new?template=pack-request.yml).
- Instalaste um pack? Dá 👍 na [issue de instalação](https://github.com/olserra/assistant-packs/issues/1). É assim que se contam as instalações.

### 2. Melhorar um pack

Encontraste um prompt melhor, um módulo mais claro, uma nota de adaptação em falta, uma correção de tradução? Abre um pull request. Mudanças pequenas, com o que experimentaste e como correu.

### 3. Publicar um pack novo

1. Copia `packs/configured-assistant/` como ponto de partida e muda o nome.
2. Segue o [FORMAT.md](FORMAT.md). Inglês obrigatório, português recomendado.
3. Faz a verificação de privacidade abaixo.
4. Acrescenta-te em `credits` no `pack.yaml` e no [CONTRIBUTORS.md](CONTRIBUTORS.md).
5. Abre um PR. Se responde a um pedido, escreve `Closes #<número>`.

### Verificação de privacidade (obrigatória)

Antes de abrir o PR, procura no pack qualquer coisa que identifique uma pessoa ou organização real: nomes, empregadores, clientes, moradas, a cidade onde vives, telefones, emails, contas, saúde, relações, finanças. Substitui por marcadores (`{{cidade}}`, "um familiar", "o CRM da tua equipa"). Na dúvida, deixa de fora. PRs que falhem esta verificação são fechados sem revisão.
