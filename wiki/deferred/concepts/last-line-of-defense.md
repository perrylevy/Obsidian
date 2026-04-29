---
type: concept
aliases: [Last Line of Defense, LLOD]
tags: [concept, liquidity, orderflow]
---

# Last Line of Defense

The last line of defense is the final price array supporting a move into a swing point. In the Turtle Soup framing, it is the leg into the swing point with no FVG left in front of the level — meaning price has no further PD array to lean on before the sweep ([[sources/how-to-trade-turtle-soups]] @ 11:25, @ 12:29, [[concepts/liquidity]]).

## Core idea

If the leg into a target still contains an FVG, the better expectation is a run. If the leg has no FVG — the last line of defense has already been used up — the setup is more vulnerable to a sweep / reversal ([[concepts/liquidity]], [[models/turtle-soup]]).

That makes the last line of defense a small but important orderflow filter:

- presence of a fresh imbalance in the leg = more room to continue,
- no imbalance remaining = the market is more exposed at the swing point.

## Why it matters

This phrase sharpens the Turtle Soup / sweep logic by telling you whether the approach into the level still has structural support.

It is not the entry itself; it is the condition that helps decide whether the market is more likely to run through the level or reverse from it ([[models/turtle-soup]]).

## Practical use

Use it to ask:

- Is the market still delivering through an imbalance before the swing?
- Or has it already exhausted the leg and is arriving at the level with no further support?

If there is no FVG in the leg, the swing point is sitting on its last line of defense.

## See also

- [[models/turtle-soup]]
- [[concepts/liquidity-sweep]]
- [[concepts/failure-swing]]
- [[concepts/liquidity]]
- [[concepts/fair-value-gap]]
