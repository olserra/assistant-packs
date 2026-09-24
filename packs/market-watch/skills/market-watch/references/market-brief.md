# Market brief

**When:** daily at the user's brief time (default 07:00 on weekdays).
**Goal:** the user knows how the markets they follow closed and what may move them today, in under a minute.

## Sections (each starts with an emoji header)

1. **📈 Indices** - each chosen index with its level and percent change, marked "at close" or with the time of the quote. Group by region if there are more than three.
2. **💱 Currencies** - each chosen pair with its rate and change since the previous close.
3. **₿ Crypto** - each chosen asset in the chosen currency, with the 24-hour change.
4. **🛢️ Commodities** - only if the user chose any.
5. **📰 Market news** - 2-4 headlines that explain the moves or can move markets today (central bank decisions, big earnings, key data releases, major company news). One line each, factual, with a link.
6. **📅 Today** - scheduled events worth knowing: data releases, central bank meetings, earnings of companies the user follows. Skip if there are none.
7. **🔔 Alerts** - price alerts that fired since the last brief, in one line, and alerts that are close to firing. Skip if there are none.

## Rules

- Fetch every number at send time from a live source. Never reuse yesterday's.
- Mark closed markets "at close" and holidays "closed today".
- Use the same order and format every day so the user can scan it.
- Changes: up and down with a sign (+1.2% / -0.8%). No colours or arrows needed; keep it plain text so it reads on any phone.
- If a source fails for one item, keep the rest and write "unavailable" for that item.
- No advice and no predictions. "Why it moved" lines state what happened, with a link.
- Omit any section the user turned off. Order can change on request.

## Example (shape only, values are illustrative)

```
📈 Thu 24 Sep · at close
S&P 500 5,712 (+0.4%) · Nasdaq 18,080 (+0.6%) · Local index 6,890 (-0.3%)
💱 EUR/USD 1.112 (+0.1%)
₿ BTC $63.1k (+1.8% 24h)
📰 Tech led gains after strong chip earnings (link) · Oil fell on supply news (link)
📅 Today: US jobless claims 13:30 · ECB speakers
🔔 BTC alert at $65k: 3% away
```
