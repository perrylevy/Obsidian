---
type: concept
aliases: [LRLR, Low Resistance Liquidity Run, Low-Resistance Liquidity Run]
tags: [concept, liquidity, order-flow]
---

# Low-Resistance Liquidity Run (LRLR)

A directional run that meets **little or no resistance** — fluid, one-directional delivery toward an unsweep target.

## Defining feature

LRLR targets are **unsweep liquidity pools** — pools that have not yet been visited / consumed in the current leg ([[sources/hrlr-vs-lrlr]]). Contrast with [[concepts/high-resistance-liquidity-run|HRLR]], where the target has already been swept.

## Signatures while a LRLR is in progress

- **Speed through swing highs / lows** — price punches through pivots without hesitation.
- **FVGs stay open** — created [[concepts/fair-value-gap|FVGs]] are not retested or filled during the run.
- **Fluid one-directional delivery** — minimal back-and-forth ([[sources/mnq-pm-silver-bullet-walkthrough]] @ 13:42).

## What catalyzes a LRLR

LRLRs are catalyzed by **HTF [[concepts/pd-array|PD arrays]]** — monthly, weekly, or daily FVGs / OBs — not by small / fragile chart patterns ([[sources/game-changer-irl-erl]] @ 18:12). When a HTF FVG aligns with an unsweep liquidity pool, the run from one to the other tends to be low-resistance.

## Use as a directional bias filter

When a LRLR is in progress, do **not** fade it. Sit on the bid / offer in the direction of the run; counter-trend entries fail because there is no resting opposing liquidity to cause a reversal.

In the derivative-teacher framing, low-resistance liquidity is the side you want to target, while high-resistance liquidity is the side you use for stop placement / the side of the curve that is already post-sweep ([[sources/hrlr-vs-lrlr]] @ 1:42).

## See also

- [[concepts/high-resistance-liquidity-run]]
- [[concepts/draw-on-liquidity]]
- [[concepts/liquidity]]
- [[concepts/fair-value-gap]]
- [[concepts/failure-swing]]
