<p align="center"><a href="../../README.pt.md">← Todos os packs</a> · <a href="README.md">English</a> · <b>Português</b> · <a href="INSTALL.md">Instalar</a></p>

# 📈 Pack n.º 3 · De Olho no Mercado

<p>
  <img alt="Feito para o Instinct" src="https://img.shields.io/badge/feito%20para-Instinct-0F5E5A?style=flat-square">
  <img alt="Versão" src="https://img.shields.io/badge/vers%C3%A3o-0.1.0-6B6258?style=flat-square">
  <img alt="Módulos" src="https://img.shields.io/badge/m%C3%B3dulos-3-E07A5F?style=flat-square">
  <img alt="Línguas" src="https://img.shields.io/badge/l%C3%ADnguas-PT%20%C2%B7%20EN-6B6258?style=flat-square">
  <img alt="Preço" src="https://img.shields.io/badge/pre%C3%A7o-gr%C3%A1tis-0F5E5A?style=flat-square">
</p>

**O teu Instinct acompanha os mercados por ti: um resumo curto antes da abertura, alertas quando um preço passa o teu nível ou varia mais do que definiste, e um balanço semanal. Só factos. Nunca dá conselhos e nunca negoceia.**

A tua lista e os teus alertas vêm de uma entrevista curta de configuração e ficam no teu Instinct.

## ⚡ Instalar

Envia isto ao teu Instinct:

```text
Instala o pack "De Olho no Mercado" do Assistant Packs.
Instruções: https://raw.githubusercontent.com/olserra/assistant-packs/main/packs/market-watch/skills/market-watch-pt/SKILL.md
Os módulos estão na pasta references/ ao lado.
Faz a entrevista de configuração comigo, agenda só o que eu aprovar
e mostra-me primeiro um exemplo do resumo de mercados com os números de hoje.
```

Só queres os alertas? Vê o [INSTALL.md](INSTALL.md).

## 👀 Como fica

```text
📈 Qui 24 set · no fecho
S&P 500 5.712 (+0,4%) · Nasdaq 18.080 (+0,6%) · Índice local 6.890 (-0,3%)
💱 EUR/USD 1,112 (+0,1%)
₿ BTC 63,1 mil $ (+1,8% 24h)
📰 Tecnológicas lideram após bons resultados de chips (link) · Petróleo cai com notícias da oferta (link)
📅 Hoje: pedidos de subsídio de desemprego nos EUA 13:30 · intervenções do BCE
🔔 Alerta BTC nos 65 mil $: a 3%
```

```text
🔔 BTC a 54.820 $ (09:40), abaixo do teu alerta de 55.000 $. Alerta removido - defino um novo nível?
```

<sub>Valores ilustrativos. As mensagens reais usam a tua lista e preços ao vivo na hora do envio.</sub>

## 🧩 Os três módulos

| | Módulo | Quando | O que recebes | Experimenta já |
|:-:|--------|--------|---------------|----------------|
| 📈 | [Resumo de mercados](skills/market-watch-pt/references/resumo-de-mercados.md) | 07:00 dias úteis | Os teus índices, moedas e cripto com a variação, notícias de mercado com links, eventos agendados do dia, alertas perto de disparar | *"manda o meu resumo de mercados"* |
| 🔔 | [Alertas de preço](skills/market-watch-pt/references/alertas-de-preco.md) | Quando uma regra se cumpre | Passagem de níveis, variações diárias acima de um limite, saídas de intervalo, decisões de bancos centrais. Com limite diário, uma linha cada | *"avisa-me se o BTC cair abaixo dos 55 mil"* |
| 🗓️ | [Balanço semanal](skills/market-watch-pt/references/balanco-semanal.md) | Sexta ao fim do dia | A semana em números, os maiores movimentos e porquê, o que está agendado para a próxima semana | *"como correram os meus mercados esta semana?"* |

## 🗣️ A entrevista de configuração

O teu Instinct pergunta isto em uma ou duas mensagens. Diz "padrão" para avançar.

1. Língua e formato de números.
2. Índices a seguir (padrão: S&P 500, Nasdaq e o índice principal do teu país).
3. Pares de moedas (padrão: a tua moeda contra USD ou EUR).
4. Cripto e a moeda em que a cotar (padrão: BTC em USD).
5. Matérias-primas, se quiseres (ouro, petróleo...).
6. Foco das notícias e setores ou empresas que segues. Opcional.
7. Hora e dias do resumo (padrão 07:00 nos dias úteis) e o balanço semanal (padrão sexta ao fim do dia).
8. Alertas iniciais e o limite de alertas por dia (padrão 3).

Depois envia um exemplo com os números reais de hoje e pergunta "mantenho este formato?".

## 🎛️ À tua medida

- *"Junta o DAX e o ouro."*
- *"Avisa-me se o S&P 500 variar mais de 2% num dia."*
- *"Sem alertas ao fim de semana."*
- *"Põe as linhas de mercado dentro do meu resumo matinal."* (funciona com o [Pack n.º 1](../configured-assistant/README.pt.md))

## 🛡️ O que este pack nunca faz

- Dizer-te para comprar, vender ou manter, dar preços-alvo ou prever preços.
- Dar ordens, movimentar dinheiro ou entrar na tua corretora ou banco.
- Partilhar a tua lista ou os teus alertas com alguém.
- Enviar mensagens "não aconteceu nada".

Este pack reporta dados e notícias de mercado. Não é aconselhamento financeiro.

## 📄 Ficheiros

```text
pack.yaml                   metadados, módulos, créditos
INSTALL.md                  mensagens de instalação (EN + PT)
skills/market-watch/        skill em inglês + 3 módulos
skills/market-watch-pt/     skill em português + 3 módulos
```

## 🙌 Créditos e alterações

- **0.1.0** - primeira versão, PT + EN. Por [@olserra](https://github.com/olserra).
- Melhoraste um módulo? Abre um PR e junta-te ao [CONTRIBUTORS.md](../../CONTRIBUTORS.md).

<sub>Projeto comunitário, sem afiliação com o Instinct. Usas outro assistente? Vê o [ADAPTERS.md](../../ADAPTERS.md).</sub>
