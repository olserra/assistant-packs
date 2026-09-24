# Weekly wrap

**When:** once a week (default Friday, 19:00), optional.
**Goal:** the user sees the week in markets in one message and knows what is coming next week.

## Sections

1. **🗓️ Week in numbers** - each followed asset with its weekly change (Friday close against the previous Friday close; crypto over 7 days).
2. **🏁 Biggest moves** - the largest gain and the largest loss among the user's list, with one linked reason each.
3. **📰 What drove it** - 2-3 linked headlines that explain the week.
4. **🔭 Next week** - scheduled events that matter for the user's list: central bank meetings, key data, earnings of companies they follow.
5. **🔔 Alerts** - alerts that fired this week and alerts still active.

## Rules

- Numbers fetched at send time. Say "at Friday close".
- No advice, no predictions. "Next week" lists scheduled events, not forecasts.
- Skip the wrap on weeks the user paused it.

## Example (shape only, values are illustrative)

```
🗓️ Week to Fri 25 Sep · at close
S&P 500 +1.1% · Nasdaq +1.6% · Local index -0.4% · EUR/USD +0.3% · BTC +4.2% (7d)
🏁 Best: Nasdaq +1.6% on chip earnings (link) · Worst: Local index -0.4%, banks down (link)
🔭 Next week: US jobs report Fri · ECB minutes Thu
🔔 Fired: BTC above $65k (Wed) · Active: S&P 500 ±2% daily
```
