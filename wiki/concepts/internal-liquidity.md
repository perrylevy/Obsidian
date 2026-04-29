---
type: concept
aliases: [Internal Liquidity, Internal LQ, IRL]
tags: [concept, liquidity]
---

# Internal Liquidity

Internal liquidity is the liquidity that exists **inside a dealing range** rather than at the obvious swing extremes. In this wiki's working usage, it most often refers to inefficiencies and hidden pockets of delivery inside the range — especially FVG-style imbalance areas ([[concepts/liquidity]], [[sources/internal-external-liquidity]] @ 0:37, @ 1:28).

The 2022 mentorship Episode 3 provides the earliest ICT-direct definition: **"internal range liquidity is looking for short-term lows or short-term highs inside a price leg that we're retracing back into"** ([[sources/2022-ict-mentorship-episode-3]]). This is the foundational source for the IRL concept, predating the derivative-teacher consensus that equates IRL with FVG.

## Core idea

If external liquidity is the obvious swing high / swing low liquidity, internal liquidity is the in-range fuel the algorithm can use before, during, or after a raid on the extremes.

Derivative-teacher consensus on the simpler model equates internal range liquidity with a FVG primitive, though ICT-direct confirmation of that strict equivalence remains pending ([[concepts/fair-value-gap]], [[sources/internal-external-liquidity]] @ 0:37, [[sources/game-changer-irl-erl]] @ 1:32, [[sources/trading-irl-erl-with-order-blocks-ict-concepts]] @ 1:32, [[sources/game-changer-irl-erl]] @ 1:32).

## How it behaves

Internal liquidity is often the intermediate destination after a sweep of external liquidity:
- price raids an obvious high or low,
- then retraces into the internal imbalance,
- then delivers back toward another external pool ([[concepts/external-liquidity]], [[concepts/fair-value-gap]], [[sources/internal-external-liquidity]] @ 1:28).

## Practical uses

Internal liquidity is useful for:
- identifying the next likely retracement target after a raid,
- separating the obvious swing pool from the in-range inefficiency,
- and framing FVGs as something more structural than a random gap ([[concepts/draw-on-liquidity]], [[concepts/fair-value-gap]], [[models/internal-external-liquidity-model]]).

## See also

- [[concepts/liquidity]]
- [[concepts/external-liquidity]]
- [[concepts/fair-value-gap]]
- [[models/internal-external-liquidity-model]]
- [[concepts/draw-on-liquidity]]
- [[sources/trading-irl-erl-with-order-blocks-ict-concepts]]
- [[sources/game-changer-irl-erl]]
