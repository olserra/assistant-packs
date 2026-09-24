<p align="center"><a href="../README.pt.md">← Início</a> · <a href="pack-authoring.md">English</a> · <b>Português</b></p>

# ✍️ Guia para criar packs

Como desenhamos, escrevemos e publicamos um pack. Lê isto antes do teu primeiro módulo; são cerca de dez minutos.

**Conteúdo:** [O que faz um bom pack](#o-que-faz-um-bom-pack) · [Desenhar em 5 passos](#desenhar-em-5-passos) · [Escrever um módulo](#escrever-um-módulo) · [Regras de privacidade](#regras-de-privacidade) · [Critérios de qualidade](#critérios-de-qualidade) · [Publicar](#publicar)

## O que faz um bom pack

Um pack é uma rotina que alguém já faz à mão, escrita para que qualquer Instinct a possa correr. Os bons têm quatro coisas em comum:

| Traço | Quer dizer | Teste |
|-------|------------|-------|
| **Uma tarefa** | Resolve um problema recorrente ("o meu correio", "a logística da família") | Consegues dizer o que faz numa frase |
| **Poucos contactos** | Aparece em momentos fixos e úteis, não o dia todo | Conta as mensagens agendadas por dia. Menos de 4? Bom |
| **Adapta-se** | Encolhe nos dias difíceis em vez de acumular | Pergunta "o que acontece se o utilizador o ignorar 3 dias?" |
| **Seguro por defeito** | Nunca age pelo utilizador sem um sim | Procura "enviar", "reservar", "comprar", "apagar". Cada um precisa de confirmação |

## Desenhar em 5 passos

1. **Parte de uma rotina real.** A tua, ou uma de um [pedido de pack](https://github.com/olserra/assistant-packs/issues?q=is%3Aissue+is%3Aopen+label%3Apack-request). Escreve o que fazes hoje, passo a passo.
2. **Divide em módulos.** Cada módulo é uma rotina com um gatilho (uma hora, um evento, um pedido). Os módulos funcionam sozinhos.
3. **Lista o que é pessoal.** Cada nome, cidade, hora, conta ou preferência passa a ser uma pergunta da configuração. Nada pessoal fica no pack.
4. **Escreve a entrevista de configuração.** Até 8 perguntas, feitas em uma ou duas mensagens, cada uma com um valor por defeito para que "defaults" funcione.
5. **Escreve um exemplo por módulo.** Se não consegues mostrar como fica a mensagem, o módulo ainda não está claro.

Abre um PR em rascunho depois do passo 2. Feedback cedo poupa reescritas.

## Escrever um módulo

Cada ficheiro de módulo em `references/` segue a mesma forma. Copia o [resumo-matinal.md](../packs/configured-assistant/skills/configured-assistant-pt/references/resumo-matinal.md) como modelo.

```markdown
# Nome do módulo

**Quando:** gatilho e hora por defeito.
**Objetivo:** o que o utilizador recebe, numa frase.

## Secções        (ou Passos)
1. **emoji Título** - o que vai aqui, que tamanho, de onde vêm os dados.

## Regras
- O que fazer quando faltam dados, o dia é difícil ou o utilizador pede para parar.

## Exemplo (só a forma, valores ilustrativos)
```

Notas de estilo:

- **Tamanho de telemóvel.** Cada mensagem lê-se em menos de um minuto.
- **Palavras simples.** "Enviar", não "despachar".
- **Comportamento, não botões.** Descreve o que o assistente faz ("todos os dias úteis à hora da manhã do utilizador, envia..."), não os menus de um produto. Detalhes de produto vão para o [ADAPTERS.md](../ADAPTERS.md).
- **Factos ao vivo.** Tempo, preços, notícias e horários vêm de uma fonte ao vivo no momento do envio. Diz o que fazer quando a fonte falha.
- **Exemplos ilustrativos.** Os valores nos exemplos são genéricos e claramente inventados.

## Regras de privacidade

São regras fixas. Um PR que falhe uma fica fechado até ser corrigido.

1. **Nada de pessoas reais.** Sem nomes, iniciais, contas, fotos ou descrições que apontem para uma pessoa real. Usa "um familiar", "a tua chefia", `{{nome}}`.
2. **Nada de organizações ligadas a ti.** Sem empregador, clientes, escola ou clínica. Serviços públicos genéricos ("um serviço de meteorologia") estão bem.
3. **Nada de lugares onde vives ou vais.** Sem cidade, bairro, morada, ginásio ou escritório. Usa `{{cidade}}`.
4. **Nada de contactos ou contas.** Sem telefones, emails, nomes de utilizador, IDs de conta, links para documentos privados.
5. **Nada de detalhes sensíveis.** Nada sobre saúde, relações, finanças, religião ou assuntos legais, mesmo anonimizado.
6. **Nada de segredos.** Sem chaves de API, tokens ou palavras-passe, nem que pareçam falsos.
7. **Os dados pessoais são perguntados, nunca guardados no pack.** A entrevista recolhe-os; o assistente guarda-os.

Verificação rápida antes de cada PR: procura nos teus ficheiros por `@`, números que pareçam telefones, nomes com maiúscula e o nome da tua cidade.

## Critérios de qualidade

Copia esta lista para a descrição do PR.

```markdown
- [ ] Resolve uma tarefa recorrente, descrita numa frase no README
- [ ] Cada módulo funciona sozinho e tem Quando / Objetivo / Regras / Exemplo
- [ ] Entrevista de configuração: 8 perguntas ou menos, cada uma com valor por defeito
- [ ] Tudo o que envia, reserva, compra, apaga ou muda dados partilhados pergunta antes
- [ ] Dados em falta são tratados ("mercados indisponíveis hoje"), nunca inventados
- [ ] Dias difíceis: o módulo encolhe em vez de acrescentar lembretes
- [ ] Cada mensagem agendada lê-se em menos de um minuto no telemóvel
- [ ] Regras de privacidade cumpridas (sem pessoas, lugares, contas, detalhes sensíveis, segredos)
- [ ] pack.yaml lista módulos, requisitos, idiomas e créditos
- [ ] README (EN) feito; README.pt.md feito ou marcado como "procura ajuda"
- [ ] Instalei no meu assistente e corri cada módulo pelo menos uma vez
```

## Publicar

1. Coloca o pack em `packs/<id-do-pack>/` seguindo o [FORMAT.md](../FORMAT.md).
2. Acrescenta-te em `credits` no `pack.yaml` e no [CONTRIBUTORS.md](../CONTRIBUTORS.md).
3. Abre um PR com a lista de qualidade. Se responde a um pedido, escreve `Closes #<número>`.
4. Um maintainer revê em poucos dias. Podemos pedir pequenas mudanças; é normal.
5. Depois do merge, entra na tabela de packs, criamos a issue de contagem de instalações e ficas nos créditos na página do pack.

Dúvidas? Pergunta nas [Discussions](https://github.com/olserra/assistant-packs/discussions).
