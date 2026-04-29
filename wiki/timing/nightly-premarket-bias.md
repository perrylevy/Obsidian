---
type: timing
aliases: [Nightly Premarket Bias, Next Day Bias, Fractal Bias, Next Candle Bias]
tags: [timing, bias, session]
---

# Nightly Premarket Bias

Nightly premarket bias is the pre-open read that uses the previous candle, the previous day’s range, and the shape of the latest expansion to anticipate whether the next session is more likely to continue, reverse, or consolidate.

It is a timing scaffold, not an entry signal. The purpose is to decide what side should be favored before the open and before the lower-time-frame model is allowed to matter.

## Core idea

If the higher-time-frame candle failed to close outside the range, the next candle often carries the opposite implication. If price has already expanded for several candles in one direction, the next phase is often retracement or consolidation rather than more of the same.

This makes the read fractal:
- daily candles can define the next day,
- hourly candles can define the next session leg,
- and the same logic can be used recursively when the market is building or repairing a daily profile.

## Practical use

Use this as a premarket filter when:
- the prior candle closed back inside the range,
- a swing high / low was swept but not cleanly accepted,
- or the market has already spent multiple candles expanding one way.

Then let the lower-time-frame execution model confirm the actual entry.

## See also

- [[models/fractal-model]]
- [[concepts/daily-profile]]
- [[concepts/price-delivery-continuum]]
- [[timing/no-initial-bias]]
- [[sources/next-day-model-fractal-way-to-get-bias-for-trading]]
