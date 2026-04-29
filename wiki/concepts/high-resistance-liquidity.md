---
type: concept
aliases: [High Resistance Liquidity, High-Resistance LQ, HRL]
tags: [concept, liquidity]
---

# High-Resistance Liquidity

High-resistance liquidity is the liquidity pool on the **already-swept** side of the market — the side that now requires more structure, time, or opposing order flow to work through. In the resistance-liquidity framing, it is the post-sweep side of the curve, contrasted with the cleaner low-resistance target side ([[concepts/low-resistance-liquidity]], [[sources/hrlr-vs-lrlr]] @ 1:21, @ 1:42).

The 02/23/2026 SMC lecture sharpens this into a session-state read: when the market is staying inside the same previous-candle range, ICT calls it high-resistance liquidity run conditions; if the discount wick cannot close below the relevant consequent encroachment, the market stays in that high-resistance state and the lower objective is still deferred ([[sources/ict-2026-smart-money-concepts-lecture-february-23-2026]] @ 4:54, @ 9:04, @ 10:05, @ 13:00, @ 13:32).
The 10/28/2024 mentorship lecture gives the direct Monday-session version: premarket can be the lower-resistance opportunity, but the 9:30 opening session is often higher resistance and should be treated with smaller expectations and lower leverage when the calendar is quiet ([[sources/ict-2024-mentorship-high-resistance-low-resistance-conditions-october-28-2024]] @ 6:34, @ 8:53, @ 12:38, @ 14:52).

## Core idea

If low-resistance liquidity is the unswept target side, high-resistance liquidity is the side that has already been consumed and now acts as the more obstructed path.

This makes it useful as:
- the stop-loss / invalidation side of a trade,
- the side of the curve that is already post-sweep,
- and the area where a move is less likely to continue cleanly without further confirmation.

## How it behaves

High-resistance liquidity commonly appears after:
- a sweep of the obvious extreme,
- a reversal that leaves the opposite side unswept,
- or a structure-heavy move where the market has already worked through the easy pool.

In the source framing, that post-sweep condition is what turns the prior target into resistance rather than a clean objective.

## Relationship to HRLR

The concrete run associated with this side is [[concepts/high-resistance-liquidity-run|high-resistance-liquidity-run]]: a move that must work through the already-swept side and tends to be choppier or more structurally burdened.

## See also

- [[concepts/low-resistance-liquidity]]
- [[concepts/high-resistance-liquidity-run]]
- [[concepts/failure-swing]]
- [[concepts/market-structure-shift]]
- [[sources/hrlr-vs-lrlr]]