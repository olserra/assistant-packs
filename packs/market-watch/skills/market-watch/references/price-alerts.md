# Price alerts

**When:** only when a rule the user set is met.
**Goal:** the user hears about the moves they care about without watching screens.

## Rule types

| Type | Example | Fires when |
|------|---------|------------|
| Level | "BTC below 55,000 USD" | The price crosses the level in the stated direction |
| Daily move | "S&P 500 moves more than 2% today" | The change since the previous close passes the threshold, up or down |
| Range break | "EUR/USD leaves 1.08-1.12" | The price leaves the range |
| Scheduled event | "tell me the ECB rate decision" | The result is published |

Save each rule with: asset, type, threshold, direction, and whether it is one-time (default) or repeating.

## How to check

- Check on a steady cadence the user agrees to (default: every 60 minutes while the asset's market is open; crypto around the clock but no alerts during the user's quiet hours unless they ask).
- Use a live price each time. If you cannot get one, skip that check silently and try again next time; tell the user only if a rule could not be checked for a whole day.
- Do not check more often than the user agreed. More frequent checks are their choice, not yours.

## Sending an alert

- One line: what crossed, the current price, the time, and the rule. "BTC at $54,820 (09:40), below your $55,000 alert."
- Add one factual line on why it moved only if a clear, linked reason exists.
- One-time rules end after firing: say "alert removed" and offer to set a new level.
- Repeating rules wait for a reset before firing again (the price returns past the level, or the next trading day for daily moves).
- Respect the daily cap (default 3). If more rules fire, send one grouped message.

## Rules

- No advice. An alert says what happened, not what to do.
- Never place orders or touch accounts, even if the user once said "sell if it drops".
- Review the list with the user once a month: "You have 4 alerts. Keep them?" Remove ones they no longer want.
- A rule that has done its job is cleaned up.
