---
type: concept
aliases: [Protected Highs, Protected Lows, Protected High/Low]
tags: [concept, risk, structure, stop-loss]
---

# Protected Highs & Lows

A protected high or low is a swing point that has enough confluence to justify placing the stop beyond it instead of using a tight, cheeky stop directly at the obvious high or low.

In the 04/26/2025 lesson, the definition is explicit: a protected high / low is a swing with SMT attached, and the best examples are time-based highs or lows rather than random local pivots.

The Protected Swings lesson adds a cleaner candle-cluster rule: once price closes through the series of candles that formed the swing, that high or low becomes protected and can hold for trend continuation.

## Core idea

The point is not to maximize reward by squeezing the stop as tight as possible. The point is to avoid unnecessary stop-outs by placing risk beyond a level that has actually earned protection.

## What makes it protected

The clip emphasizes three ingredients:

- SMT must exist at the swing.
- The SMT should be time-based, not just a random swing.
- The swing should sit inside the correct higher-time-frame context.

## Practical use

Use protected highs and lows as stop-placement references when:

- the higher-time-frame bias is already established,
- the lower-time-frame entry is nested inside that context,
- and the sweep / divergence at the swing supports the idea that price should not easily run the stop before moving in the intended direction.

The TTrades clip "Why You're Failing with ICT Concepts" generalizes the same habit: once you pick one PD array, highs and lows should stay the structural context around that array, not a second competing model. The protection logic still belongs on the swing that actually justifies the stop, rather than on an obvious wick extreme ([[sources/why-youre-failing-with-ict-concepts]]).

## Related concepts

- [[concepts/smt]]
- [[concepts/time-frame-alignment]]
- [[concepts/market-structure-shift]]
- [[concepts/smart-money-reversal]]
- [[concepts/liquidity]]

## See also

- [[concepts/smt]]
- [[concepts/time-frame-alignment]]
- [[concepts/smart-money-reversal]]
- [[sources/protected-swings-understanding-trend-and-invalidations]]
- [[models/market-maker-buy-model]]
- [[models/market-maker-sell-model]]
