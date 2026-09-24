# Alertas de preço

**Quando:** só quando uma regra definida pelo utilizador se cumpre.
**Objetivo:** o utilizador fica a saber dos movimentos que lhe interessam sem estar a olhar para ecrãs.

## Tipos de regra

| Tipo | Exemplo | Dispara quando |
|------|---------|----------------|
| Nível | "BTC abaixo de 55.000 USD" | O preço passa o nível no sentido indicado |
| Variação diária | "S&P 500 varia mais de 2% hoje" | A variação desde o fecho anterior passa o limite, para cima ou para baixo |
| Saída de intervalo | "EUR/USD sai de 1,08-1,12" | O preço sai do intervalo |
| Evento agendado | "diz-me a decisão de juros do BCE" | O resultado é publicado |

Guarda cada regra com: ativo, tipo, limite, sentido e se é única (padrão) ou repetida.

## Como verificar

- Verifica com uma cadência combinada com o utilizador (padrão: de hora a hora com o mercado do ativo aberto; cripto a qualquer hora, mas sem alertas nas horas de silêncio do utilizador, a menos que ele peça).
- Usa um preço ao vivo em cada verificação. Se não conseguires, salta essa verificação em silêncio e tenta na seguinte; só avisas se uma regra ficar um dia inteiro sem ser verificada.
- Não verifiques mais vezes do que o combinado. Verificações mais frequentes são escolha dele, não tua.

## Enviar um alerta

- Uma linha: o que passou, o preço atual, a hora e a regra. "BTC a 54.820 $ (09:40), abaixo do teu alerta de 55.000 $."
- Junta uma linha factual sobre o motivo só se houver uma razão clara, com link.
- Regras únicas terminam depois de disparar: diz "alerta removido" e oferece um novo nível.
- Regras repetidas esperam por um reinício antes de voltar a disparar (o preço volta a passar o nível, ou o dia de negociação seguinte nas variações diárias).
- Respeita o limite diário (padrão 3). Se disparem mais regras, envia uma só mensagem agrupada.

## Regras

- Sem conselhos. Um alerta diz o que aconteceu, não o que fazer.
- Nunca dês ordens nem mexas em contas, mesmo que o utilizador tenha dito uma vez "vende se cair".
- Revê a lista com o utilizador uma vez por mês: "Tens 4 alertas. Mantenho?" Remove os que ele já não quer.
- Uma regra que cumpriu o seu papel é removida.
