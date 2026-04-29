---
type: concept
aliases: [Sellside Liquidity, Sell-Side Liquidity, Sellside LQ]
tags: [concept, liquidity]
---

# Sellside Liquidity

Sellside liquidity is the pool of resting **sell-stops below swing lows**. In practical ICT usage, it is the visible low-side liquidity that breakout traders leave behind when they place stops below prior lows ([[concepts/liquidity]], [[sources/internal-external-liquidity]] @ 1:17, [[sources/how-to-trade-turtle-soups]] @ 6:26, @ 7:14).

## Core idea

When price reaches a sellside pool, it can either:
- **sweep** it and reverse, or
- **run** through it and continue lower.

That sweep-vs-run distinction is central to turtle soup and liquidity-sweep logic ([[concepts/liquidity-sweep]], [[models/turtle-soup]], [[sources/how-to-trade-turtle-soups]] @ 3:48, @ 4:15, @ 8:30).

## Why it matters

Sellside liquidity is one of the market’s most common targets for delivery:
- it marks where breakout sell orders cluster,
- it often becomes the draw on liquidity below price,
- and it can serve as the trap level that fuels a reversal after a sweep ([[concepts/draw-on-liquidity]], [[sources/internal-external-liquidity]] @ 1:28, [[sources/nq-heavy-manipulation-review]] @ 13:09).

## Common forms

Sellside liquidity often appears as:
- prior swing lows,
- relative equal lows,
- prior session lows,
- prior day lows,
- or other obvious lows that attract stop placement ([[concepts/liquidity]], [[concepts/relative-equal-highs-lows]], [[sources/internal-external-liquidity]] @ 11:16, [[sources/2023-mentorship-silver-bullet]] @ 3:47–6:41).

## Sweep behavior

When sellside liquidity is swept:
- price trades below the obvious low,
- breakout traders get trapped,
- and a reversal can follow if the move fails to hold below the level.

That is the classic Turtle Soup / liquidity sweep pattern on the sell side ([[models/turtle-soup]], [[concepts/liquidity-sweep]], [[sources/how-to-trade-turtle-soups]] @ 2:11, @ 2:35, @ 8:30).

## See also

- [[concepts/liquidity]]
- [[concepts/buyside-liquidity]]
- [[concepts/liquidity-sweep]]
- [[concepts/draw-on-liquidity]]
- [[concepts/relative-equal-highs-lows]]
- [[models/turtle-soup]]
- [[models/internal-external-liquidity-model]]
