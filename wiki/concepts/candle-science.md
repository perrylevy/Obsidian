---
type: concept
aliases: [Candle Science]
tags: [concept, candles, orderflow]
---

# Candle Science

Candle science is the fractal read of candles as structural units of delivery. In the Turtle Soup material, the same sweep logic appears on multiple time frames: a candle can act as the swing, and the sweep / rejection can be read off the candle high or low directly ([[sources/how-to-trade-turtle-soups]] @ 19:13, @ 21:16, [[sources/2024-mentorship-lecture-1]] @ 1:17:22–1:18:04).

## Core idea

The practical use is simple:

- read the candle high/low as a working swing point,
- watch whether price takes it and rejects,
- and treat that behavior as a fractal liquidity event.

## Wick-size filter

The wick-size source sharpens the candle-science read:

- a shallow opposing run with a small wick supports expansion,
- a large opposing run with a large wick is more often a reversal candle,
- and when the wick is too large to support expansion, candle 3 is usually the cleaner continuation trade ([[sources/wick-size-matters-the-key-to-understanding-reversal-and-expansion-candles]] @ 0:11, @ 4:26, @ 5:36, @ 8:38).
The "Master Candlestick Wicks" clip generalizes the same rule across timeframes: the 50% mark of the wick is the decision line, respected wicks support continuation, and disrespected wicks usually point to the opposite extreme instead ([[sources/master-candlestick-wicks-the-key-to-catching-reversals]] @ 0:25, @ 1:18, @ 2:13, @ 4:15, @ 7:26, @ 11:13).

The "Never Miss Another Trade" clip turns that into a three-part candle sequence: one candle can offer a wick trade, an expansion trade, and a cap trade, with the trader choosing the part of the candle that fits the current model best ([[sources/never-miss-another-trade]]).

## Relationship to other concepts

Candle science is one layer of the same logic behind:

- [[concepts/swing-failure-pattern]]
- [[concepts/liquidity-sweep]]
- [[synthesis/how-to-use-order-flow-entries]]
- [[concepts/candle-science]]
- [[concepts/candle-science]]
- [[sources/wick-size-matters-the-key-to-understanding-reversal-and-expansion-candles]]

## Previous-candle references

The **previous candle high** and **previous candle low** are handled here as candle-science primitives rather than as separate top-level doctrine pages. They are simply the nearest candle-level swing references used for a fractal sweep, stop run, or rejection read inside the broader candle-science / turtle-soup framework ([[sources/how-to-trade-turtle-soups]] @ 18:53, @ 19:13, @ 19:54).

## Candle-behavior heuristic

The derivative-teacher 'candle behavior' material is also folded into this page as an execution heuristic: the first half of a candle can build the opposing wick, while the second half may decide whether the candle continues or reverses. Useful, but lower doctrinal weight than ICT-direct material ([[sources/always-wait-for-this-before-entering-a-trade-candle-behavior]] @ 0:25, @ 0:55, @ 1:32, @ 2:02).

## Directional candle resistance/support rules

ICT's 2022 mentorship Episode 12 provides structural candle rules tied to directional bias:

- **Bearish market (price going lower)**: up-closed candles act as resistance / speed bumps. Price should NOT trade above them. Violation of an up-closed candle signals the bearish idea is likely wrong.
- **Bullish market (price going higher)**: down-closed candles act as support. Price should NOT trade below them. Violation of a down-closed candle signals the bullish idea is likely wrong.

> "When price is moving higher, generally the candles will be predominantly green... but down-closed candles should support price." ([[sources/2022-ict-mentorship-episode-12]])

These rules are a real-time structural filter: they tell the trader whether the algorithm is still delivering in the expected direction by monitoring whether opposing-color candles are being respected or violated.

## Practical use

Use candle science when a lower-timeframe candle itself becomes the swing reference — especially in sweep-based setups where the high/low of the prior candle defines the next trap or rejection.

## See also

- [[concepts/candle-science]]
- [[concepts/candle-science]]
- [[concepts/swing-failure-pattern]]
- [[synthesis/how-to-use-order-flow-entries]]
- [[models/turtle-soup]]
- [[sources/always-wait-for-this-before-entering-a-trade-candle-behavior]]
