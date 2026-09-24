<p align="center"><a href="../../README.pt.md">← Todos os packs</a> · <a href="README.md">English</a> · <b>Português</b> · <a href="INSTALL.md">Instalar</a></p>

# ☀️ Pack n.º 1 · O Assistente Configurado

<p>
  <img alt="Feito para o Instinct" src="https://img.shields.io/badge/feito%20para-Instinct-0F5E5A?style=flat-square">
  <img alt="Versão" src="https://img.shields.io/badge/vers%C3%A3o-0.1.0-6B6258?style=flat-square">
  <img alt="Módulos" src="https://img.shields.io/badge/m%C3%B3dulos-6-E07A5F?style=flat-square">
  <img alt="Línguas" src="https://img.shields.io/badge/l%C3%ADnguas-PT%20%C2%B7%20EN-6B6258?style=flat-square">
  <img alt="Preço" src="https://img.shields.io/badge/pre%C3%A7o-gr%C3%A1tis-0F5E5A?style=flat-square">
  <a href="https://github.com/olserra/assistant-packs/issues/1"><img alt="Instalações" src="https://img.shields.io/badge/instala%C3%A7%C3%B5es-%F0%9F%91%8D%20na%20issue%20%231-0F5E5A?style=flat-square"></a>
</p>

**Dá ao teu Instinct um ritmo diário: resumo de manhã, plano para amanhã todas as noites, um lembrete de coaching a meio do dia, pontos que perdoam os dias maus e vigilantes que só falam quando importa.**

Baseado numa configuração real de uso diário, sem nenhum dado pessoal. Os teus dados vêm de uma entrevista curta e ficam no teu Instinct.

## ⚡ Instalar

Envia isto ao teu Instinct:

```text
Instala o pack "Assistente Configurado" do Assistant Packs.
Instruções: https://raw.githubusercontent.com/olserra/assistant-packs/main/packs/configured-assistant/skills/configured-assistant-pt/SKILL.md
Os módulos estão na pasta references/ ao lado.
Faz a entrevista de configuração comigo, agenda só as rotinas que eu aprovar
e mostra-me um exemplo do resumo da noite de amanhã antes do primeiro sair.
```

Só queres uma parte? Vê o [INSTALL.md](INSTALL.md).

## 👀 Pré-visualização

<table>
  <tr>
    <td width="50%"><img src="../../assets/previews/morning-brief.pt.svg" alt="Exemplo do resumo matinal" width="100%"></td>
    <td width="50%"><img src="../../assets/previews/evening-brief.pt.svg" alt="Exemplo do resumo da noite" width="100%"></td>
  </tr>
  <tr>
    <td><img src="../../assets/previews/coaching-ping.pt.svg" alt="Exemplo do lembrete de coaching" width="100%"></td>
    <td><img src="../../assets/previews/weekly-board.pt.svg" alt="Exemplo do placar de domingo" width="100%"></td>
  </tr>
</table>

<sub>Valores ilustrativos. Os resumos reais usam a tua cidade, o teu calendário e fontes ao vivo.</sub>

## 🧩 Os seis módulos

| | Módulo | Quando | O que recebes | Experimenta já |
|:-:|--------|--------|---------------|----------------|
| ☀️ | [Resumo matinal](skills/configured-assistant-pt/references/resumo-matinal.md) | 07:00 | Tempo e chuva por parte do dia, os teus números de mercado, manchetes, 3 novidades da tua área, 3 prioridades, exercício de 5 minutos, uma prática de bem-estar, a tua sequência | *"faz o meu resumo matinal"* |
| 🌙 | [Resumo da noite](skills/configured-assistant-pt/references/resumo-da-noite.md) | 21:00 | Agenda de amanhã por hora, prazos, o que preparar hoje, a que horas sair, e uma reflexão de 2 minutos | *"mostra-me o resumo de amanhã"* |
| ⏰ | [Lembrete de coaching](skills/configured-assistant-pt/references/lembrete-diario.md) | 13:00 | Uma pergunta: fizeste o micro-treino de hoje? Versão de 2 minutos se não. Nunca um segundo lembrete. | *"lembra-me como farias ao almoço"* |
| 🏆 | [Pontos e placar](skills/configured-assistant-pt/references/placar-de-pontos.md) | Diário · domingo | Até 4 pontos por dia, uma sequência e um placar ao domingo que mostra o que fizeste | *"como vai a minha semana?"* |
| 👀 | [Vigilantes](skills/configured-assistant-pt/references/vigilantes.md) | Quando preciso | Avisos de "sai às 17:40" pelo trânsito e alertas de "responderam" nas conversas que pedires | *"avisa-me quando o Sam responder"* |
| 🎯 | [Coaching](skills/configured-assistant-pt/references/coaching.md) | Semanal · diário | Técnica de hábitos da semana, 5 minutos diários da habilidade que escolheres, simulações a pedido | *"simula uma chamada difícil com um cliente"* |

## 🗣️ A entrevista de configuração

O teu Instinct pergunta isto em uma ou duas mensagens. Diz "padrão" para avançar.

1. Como te chamar e em que língua.
2. A tua cidade para o tempo, e Celsius ou Fahrenheit.
3. Horas dos resumos da manhã e da noite (padrão 07:00 e 21:00).
4. Números de mercado a seguir, se algum (um par de moedas, um índice, uma cripto).
5. Regiões de notícias e um tema da tua área.
6. Uma habilidade para treinar em pequenas doses diárias.
7. Até três papéis para a reflexão da noite (pai/mãe, parceiro, amigo...). Opcional.
8. Que calendários e caixas de email pode ler. Opcional.
9. Se queres o lembrete do meio-dia e os pontos (ambos ligados por padrão).

Depois envia um exemplo do resumo da noite com os teus dados reais e pergunta "mantenho este formato?". O que aprovares passa a ser a base.

## 🎛️ À tua medida

Muda o que quiseres, por palavras tuas:

- *"Passa o resumo matinal para as 6:30 nos dias úteis."*
- *"Tira os mercados e põe o tempo para a minha corrida."*
- *"Pausa tudo, estou de férias até segunda."*
- *"Hoje sem lembrete, estou doente."* (o objetivo do dia baixa para 1 ponto)

## 🛡️ O que este pack nunca faz

- Enviar mensagens a outras pessoas, reservar, comprar ou aceitar convites sem o teu sim.
- Acrescentar lembretes porque falhaste um.
- Partilhar a tua configuração, calendário ou reflexões com alguém.

## 🙌 Créditos e versões

- **0.1.0** - primeira versão, PT + EN. Por [@olserra](https://github.com/olserra).
- Melhoraste um módulo? Abre um PR e junta-te ao [CONTRIBUTORS.md](../../CONTRIBUTORS.md).

**Instalaste?** Dá 👍 na [issue #1](https://github.com/olserra/assistant-packs/issues/1) para o contador subir e conta nos comentários o que mudaste.

<sub>Projeto comunitário, sem ligação ao Instinct. Usas outro assistente? Vê o [ADAPTERS.md](../../ADAPTERS.md).</sub>
