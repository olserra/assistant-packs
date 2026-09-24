<p align="center"><a href="../../README.md">← All packs</a> · <b>English</b> · <a href="README.pt.md">Português</a> · <a href="INSTALL.md">Install</a></p>

# 📈 Pack #3 · Market Watch

<p>
  <img alt="Built for Instinct" src="https://img.shields.io/badge/built%20for-Instinct-0F5E5A?style=flat-square">
  <img alt="Version" src="https://img.shields.io/badge/version-0.1.0-6B6258?style=flat-square">
  <img alt="Modules" src="https://img.shields.io/badge/modules-3-E07A5F?style=flat-square">
  <img alt="Languages" src="https://img.shields.io/badge/languages-EN%20%C2%B7%20PT-6B6258?style=flat-square">
  <img alt="Price" src="https://img.shields.io/badge/price-free-0F5E5A?style=flat-square">
</p>

**Your Instinct follows the markets for you: a short market brief before the open, alerts when a price crosses your level or moves more than you set, and a weekly wrap. Facts only. It never gives advice and never trades.**

Your watchlist and alerts come from a short setup interview and stay in your Instinct.

## ⚡ Install

Send this to your Instinct:

```text
Install the "Market Watch" pack from Assistant Packs.
Instructions: https://raw.githubusercontent.com/olserra/assistant-packs/main/packs/market-watch/skills/market-watch/SKILL.md
Modules are in the references/ folder next to it.
Run the setup interview with me, schedule only what I approve,
and show me a sample market brief with today's numbers first.
```

Only want the alerts, or setting it up in Portuguese? See [INSTALL.md](INSTALL.md).

## 👀 What it looks like

```text
📈 Thu 24 Sep · at close
S&P 500 5,712 (+0.4%) · Nasdaq 18,080 (+0.6%) · Local index 6,890 (-0.3%)
💱 EUR/USD 1.112 (+0.1%)
₿ BTC $63.1k (+1.8% 24h)
📰 Tech led gains after strong chip earnings (link) · Oil fell on supply news (link)
📅 Today: US jobless claims 13:30 · ECB speakers
🔔 BTC alert at $65k: 3% away
```

```text
🔔 BTC at $54,820 (09:40), below your $55,000 alert. Alert removed - set a new level?
```

<sub>Illustrative values. Real messages use your list and live prices at send time.</sub>

## 🧩 The three modules

| | Module | When | What you get | Try it now |
|:-:|--------|------|--------------|------------|
| 📈 | [Market brief](skills/market-watch/references/market-brief.md) | 07:00 weekdays | Your indices, currency pairs and crypto with the change, market headlines with links, today's scheduled events, alerts close to firing | *"run my market brief"* |
| 🔔 | [Price alerts](skills/market-watch/references/price-alerts.md) | When a rule is met | Level crossings, daily moves over a threshold, range breaks, central bank decisions. Capped per day, one line each | *"alert me if BTC drops below 55k"* |
| 🗓️ | [Weekly wrap](skills/market-watch/references/weekly-wrap.md) | Friday evening | The week in numbers, biggest moves and why, what is scheduled next week | *"how did my markets do this week?"* |

## 🗣️ The setup interview

Your Instinct asks these in one or two messages. Say "defaults" to skip ahead.

1. Language and number format.
2. Indices to follow (default: S&P 500, Nasdaq and your country's main index).
3. Currency pairs (default: your currency against USD or EUR).
4. Crypto and the currency to price it in (default: BTC in USD).
5. Commodities, if any (gold, oil...).
6. News focus, plus sectors or companies you follow. Optional.
7. Brief time and days (default 07:00 on weekdays) and the weekly wrap (default Friday evening).
8. Starting alerts and the daily alert cap (default 3).

Then it sends a sample brief with today's real numbers and asks "keep this format?".

## 🎛️ Make it yours

- *"Add the DAX and gold."*
- *"Alert me if the S&P 500 moves more than 2% in a day."*
- *"No alerts on weekends."*
- *"Put the market lines inside my morning brief instead."* (works with [Pack #1](../configured-assistant/))

## 🛡️ What this pack never does

- Tell you to buy, sell or hold, give price targets or predict prices.
- Place orders, move money or log into your broker or bank.
- Share your watchlist or alerts with anyone.
- Send "nothing happened" messages.

This pack reports market data and news. It is not financial advice.

## 📄 Files

```text
pack.yaml                   metadata, modules, credits
INSTALL.md                  install messages (EN + PT)
skills/market-watch/        English skill + 3 module files
skills/market-watch-pt/     Portuguese skill + 3 module files
```

## 🙌 Credits & changelog

- **0.1.0** - first release, EN + PT. By [@olserra](https://github.com/olserra).
- Improved a module? Open a PR and add yourself to [CONTRIBUTORS.md](../../CONTRIBUTORS.md).

<sub>Community project, not affiliated with Instinct. Using another assistant? See [ADAPTERS.md](../../ADAPTERS.md).</sub>
