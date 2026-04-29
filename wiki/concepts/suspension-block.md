---
type: concept
aliases: [Suspension Block, Suspension Blocks, SB]
tags: [concept, pd-array, fvg]
---

# Suspension Block

A **suspension block** is an ICT-specific PD array formed by a single candle whose body sits **between an upper volume imbalance and a lower volume imbalance**. The body is held in place — "suspended" — between the two VIs, which is why ICT named it this way ([[sources/ict-suspension-block-review-september-30-2025]] @ 10:54, @ 11:20, @ 11:37).

## Construction (ICT-direct definition)

- Upper **volume imbalance** above the body.
- Candle **body** (up-close for bullish, down-close for bearish).
- Lower **volume imbalance** below the body.
- Prior wicks crossing the area do **not** invalidate the construction — the sandwich is what matters ([[sources/ict-suspension-block-review-september-30-2025]] @ 11:20, @ 13:16).

By the original three-candle-no-overlap FVG definition, a suspension block would not qualify as an FVG; the algorithm still treats it as a valid PD array ([[sources/ict-suspension-block-review-september-30-2025]] @ 10:57).

## Behavior

- Bullish suspension block: used in bullish orderflow, body of the down-close or up-close array acts as support on revisit ([[sources/ict-suspension-block-review-september-30-2025]] @ 12:00).
- Bearish suspension block: the mirror — used when a down-close candle has VIs above and below and orderflow is pointing lower.
- **Inversion mode**: once price reverses cleanly through the suspension block, its character flips. A prior bullish suspension block now acts as a premium array on revisit ([[sources/ict-suspension-block-review-september-30-2025]] @ 14:51, @ 15:18). This mirrors [[concepts/inversion-fair-value-gap|IFVG]] logic.
- Quality grading is done the same way as any dealing range — watch **bodies** respect upper/lower quadrants and [[concepts/consequent-encroachment|consequent encroachment]], not wicks ([[sources/ict-suspension-block-review-september-30-2025]] @ 15:18, @ 15:38).

## Relationship to the PD Array Matrix

The matrix lesson frames suspension blocks as part of the FVG family for grading purposes and treats them as high-probability when aligned with the matrix quadrant structure ([[sources/2025-pd-array-matrix]] @ 43:55–43:58, [[sources/how-do-i-engage-markets-when-i-dont-have-an-initial-bias]] @ 26). The September 30, 2025 review gives the construction rules the matrix lesson implies.

The 03/27/2026 commentary adds a live charting rule: when a bullish suspension block is used as bearish context, price should trade in the lower half of the block and candle **bodies** should stay out of the upper half if the downside thesis is still intact ([[sources/ict-2026-market-commentary-march-27-2026]]). The 03/21/2026 dollar-index commentary frames a suspension block as a line-in-the-sand level whose loss supports HTF continuation ([[sources/ict-2026-market-commentary-march-21-2026]]).

## Operator use

1. Identify the up-close or down-close candle whose body is sandwiched between an upper VI and a lower VI on the execution chart (typically 1m for NQ).
2. Require narrative + orderflow aligned in the suspension block's direction.
3. On revisit, wait for **bodies** to respect consequent encroachment or the correct quadrant before entering.
4. If price breaks cleanly through, flip the read — subsequent revisits are inversion suspension block context.
5. Use PD array matrix rules to decide whether the suspension block is in the correct quadrant and the correct time window; if not, defer.

## See also

- [[concepts/volume-imbalance]]
- [[concepts/fair-value-gap]]
- [[concepts/inversion-fair-value-gap]]
- [[concepts/consequent-encroachment]]
- [[concepts/pd-array]]
- [[concepts/order-block]]
- [[timing/macros]]

