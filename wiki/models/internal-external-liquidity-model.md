---
type: model
aliases: [Internal External Liquidity Model, IRL ERL Model, I-E Liquidity Model]
tags: [model, liquidity]
---

# Internal-External Liquidity Model

The internal-external liquidity model describes how price moves from **external liquidity** to **internal liquidity** and then back to external liquidity again. In the simplest form, it is the sequence:

1. raid an obvious swing pool,
2. retrace into the in-range inefficiency,
3. deliver toward the next external pool ([[concepts/internal-liquidity]], [[concepts/external-liquidity]], [[sources/internal-external-liquidity]] @ 1:28).

## Status in this wiki

For Hermes-trading-analyst, this is a **routing / target-path framework**, not usually a standalone trade trigger. Use it to refine where price should raid, rebalance, and deliver next after a primary model has already been identified.

## Core structure

The model comes from the idea that:
- **external liquidity** is the visible swing high / swing low stop pool,
- **internal liquidity** is the in-range imbalance, often FVG-like,
- and price often oscillates **external → internal → external** rather than moving in a straight line ([[concepts/liquidity]], [[sources/internal-external-liquidity]] @ 0:37, @ 0:58, @ 1:17, @ 1:28).

## How the model is used

The source presents the model as a practical nesting process:
- start from a higher-time-frame draw,
- drop to a lower time frame,
- require the relevant killzone,
- then wait for a stop raid, market structure shift, and FVG entry before targeting 2R ([[sources/internal-external-liquidity]] @ 1:56).

The 2024–2025 derivative sources sharpen the same stack: IRL/ERL is the basis for drawing from external to internal and back again, and the order-block / lunch-macro examples both keep the same structure of a higher-time-frame draw, a liquidity raid, and a lower-timeframe confirmation ([[sources/trading-irl-erl-with-order-blocks-ict-concepts]] @ 0:05, @ 1:32, [[sources/game-changer-irl-erl]] @ 0:01, @ 4:28, [[sources/nq-ny-lunch-macro-02242025]] @ 1:18, @ 4:50).

That makes the model less about abstract labels and more about a repeatable execution stack.

## Relationship to IRL and ERL

In the working vocabulary of this wiki:
- [[concepts/internal-liquidity|IRL]] is the in-range pocket of delivery,
- [[concepts/external-liquidity|ERL]] is the obvious edge liquidity at the swing extremes.

Derivative-teacher sources also equate IRL with FVG as a primitive, though the stricter ICT-direct framing is still pending confirmation ([[concepts/fair-value-gap]], [[sources/internal-external-liquidity]] @ 0:37, [[sources/game-changer-irl-erl]] @ 1:32).

## Practical applications

This model helps with:
- identifying whether price is targeting the obvious high/low or the in-range inefficiency first,
- deciding whether a sweep is likely to continue or revert into the gap,
- reading the market as a sequence of liquidity raids rather than isolated candles ([[concepts/draw-on-liquidity]], [[concepts/liquidity-sweep]], [[sources/internal-external-liquidity]] @ 1:28),
- and deciding when the target is too ambiguous to justify a trade, in which case no-trade is the better choice ([[sources/the-3-step-a-plus-ict-strategy-that-actually-works]]).

## Risk & stop placement

- **Entry trigger**: the canonical sequence — killzone + stop raid of external liquidity + [[concepts/market-structure-shift|MSS]] + entry on the newly-created [[concepts/fair-value-gap|FVG]] inside the internal-liquidity zone ([[sources/internal-external-liquidity]] @ 1:56).
- **Stop placement**: beyond the external-liquidity wick that was swept — above the raided high for a short, below the raided low for a long. The sweep IS the invalidation reference; anything back through it means the external pool was real, not engineered.
- **Target**: the opposite external-liquidity pool (other side of the dealing range). Internal-liquidity entries target external-liquidity exits. Scale at the nearest relative equal high/low inside the range; trail the runner to the opposite extreme.
- **Invalidation**: a second sweep in the original direction without MSS reclaim — the model requires the MSS to validate the raid as manipulation rather than breakout.

## Related examples

The source applies the model to:
- low-resistance liquidity formed by lined-up previous-day lows,
- equal lows after a prior month's low is taken,
- and a market-maker buy-model example where the retracement lines up with a breaker block and discount FVG ([[sources/internal-external-liquidity]] @ 8:06, @ 10:47, @ 11:16, @ 14:23, @ 14:38).

## See also

- [[concepts/internal-liquidity]]
- [[concepts/external-liquidity]]
- [[concepts/liquidity]]
- [[concepts/fair-value-gap]]
- [[concepts/draw-on-liquidity]]
- [[models/market-maker-buy-model]]
- [[models/turtle-soup]]
- [[sources/trading-irl-erl-with-order-blocks-ict-concepts]]
- [[sources/game-changer-irl-erl]]
- [[sources/nq-ny-lunch-macro-02242025]]
