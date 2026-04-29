---
type: model
aliases: [Cameron's Model, Cameron Model]
tags: [model, liquidity, entry, ict-core]
---

# Cameron's Model

A **liquidity-and-stop-raid execution model**: identify a higher-time-frame draw on liquidity, wait for a lower-time-frame stop raid in the opposite direction, then use a fair value gap for entry ([[sources/every-ict-trading-strategy-explained-in-13-minutes]] @ 1:47, @ 2:13, @ 2:39, @ 3:12).

## Status in this wiki

For Hermes-trading-analyst, Cameron's model is best treated as a **compact derivative variant** of the broader liquidity-sweep / Turtle Soup family. It is useful as a simple checklist, but it should not sit at the same decision weight as the stronger canonical model pages.

## Working definition

- First, find a key high or low on the 1-hour chart that price is moving toward — the draw on liquidity ([[sources/every-ict-trading-strategy-explained-in-13-minutes]] @ 2:13).
- If no clean hourly draw is visible, zoom into the 15-minute chart ([[sources/every-ict-trading-strategy-explained-in-13-minutes]] @ 2:13).
- Next, on the 5-minute chart, look for a stop raid in the opposite direction of that draw — e.g. a swing low taken out when the market is targeting higher liquidity ([[sources/every-ict-trading-strategy-explained-in-13-minutes]] @ 2:39).
- Finally, find a fair value gap and place the limit entry at the start of the gap; if needed, drill down to 1-minute or 30-second for a tighter FVG ([[sources/every-ict-trading-strategy-explained-in-13-minutes]] @ 2:39, @ 3:12).
- The source explicitly warns against stops that are too tight ([[sources/every-ict-trading-strategy-explained-in-13-minutes]] @ 3:12).

## Relationship to other models

- Similar to [[models/turtle-soup]] because both use liquidity logic plus reversal-style entry.
- Similar to [[models/silver-bullet]] because both combine liquidity structure with FVG-based execution.
- Different from [[models/silver-bullet]] because Cameron's model is sequence-based rather than primarily time-window-based.

## See also

- [[concepts/draw-on-liquidity]]
- [[concepts/liquidity-sweep]]
- [[concepts/liquidity-sweep]]
- [[concepts/fair-value-gap]]
- [[models/turtle-soup]]
- [[models/silver-bullet]]
- [[sources/every-ict-trading-strategy-explained-in-13-minutes]]
