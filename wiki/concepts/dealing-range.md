---
type: concept
aliases: [Dealing Range]
tags: [concept, structure]
---

# Dealing Range

A range qualifies as a **dealing range** only after price has taken **both sides of liquidity** — a swing high (buyside) AND a swing low (sellside) — on the trading time frame ([[sources/2024-04-18-ob-tape-reading]] @ 47:47, @ 48:26, @ 1:37:34).

The midpoint of a dealing range = **equilibrium**. Above midpoint = premium, below = discount ([[concepts/discount-premium]]).

## DRT / range grading

EP8 adds an explicit dealing-range-theory grading:
- **25 DRT** and **75 DRT** are the outer quartile levels where breakaway-gap / terminus-gap logic is expected.
- **50 DRT** is the equilibrium / measuring level.

In that framing, the range is not just split into premium vs discount; it is also read through 25 / 50 / 75 levels to decide whether price is reacting at the beginning of a leg, the midpoint of a leg, or the likely termination area ([[sources/ep8-the-daily-range]] @ 2:42, @ 4:04, @ 11:57).

## Quadrant overlay

The same quadrant grading used in the [[concepts/pd-array|PD array matrix]] applies inside any dealing range — divide the range into four quadrants with the equilibrium midline.

## OB as a micro dealing range

ICT explicitly: **"your order block is what — it's a dealing range — but very specific with this part"** ([[sources/2024-04-18-ob-tape-reading]] @ 2:08:29). An [[concepts/order-block|order block's]] internal range is graded with the same quadrant / equilibrium logic as a higher-timeframe dealing range. The bullish OB precision rule (look for the entry candle in the **upper portion** of the OB's internal range) follows from this.

## See also

- [[concepts/discount-premium]]
- [[concepts/pd-array]]
- [[concepts/order-block]]
- [[concepts/consequent-encroachment]]
