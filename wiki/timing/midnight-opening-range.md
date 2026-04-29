---
type: timing
aliases: [Midnight Open Range, Midnight OR, Midnight Opening Range]
tags: [timing, session, range]
---

# Midnight Opening Range

The midnight opening range is the first 30 minutes from 00:00 to 00:30 New York time. In the daily-high / daily-low workflow, the range is measured and then projected with standard-deviation levels to estimate where the session may pivot. The range starts at the [[concepts/midnight-opening-price|midnight opening price]], which is a separate anchor point from the range itself. The SMC midnight-opening lecture uses this scaffold as a practical daily-high / daily-low map and explicitly treats the opening price, range high, and range low as separate reference points ([[sources/smc-midnight-opening-range]]).

## Core idea

Use the range high, range low, and midpoint/standard-deviation projections as a rough map for the day.

The common workflow is:

- mark the 00:00–00:30 range,
- project the range up and down with standard-deviation levels,
- watch whether price respects those levels during London or the New York morning,
- and use the result as a confluence tool, not a certainty.

## Why it matters

The midnight opening range is useful because it creates a repeatable frame before the main New York session begins. In the derivative material, the session’s daily high or low often prints near one of the projected levels when volatility is normal and the market has a clear narrative.

## Practical use

Use it with:

- [[timing/new-york-local-time]] for the session clock,
- [[timing/opening-range]] for the broader opening logic family,
- [[models/power-of-three]] for the daily expansion structure,
- [[concepts/fair-value-gap]] for confluence,
- [[concepts/draw-on-liquidity]] for target logic.

## See also

- [[timing/opening-range]]
- [[concepts/midnight-opening-price]]
- [[models/power-of-three]]
- [[concepts/fair-value-gap]]
- [[concepts/draw-on-liquidity]]
- [[sources/how-to-predict-daily-highs-and-lows]]
- [[sources/smc-midnight-opening-range]]
