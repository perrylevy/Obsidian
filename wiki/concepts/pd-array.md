---
type: concept
aliases: [PD Array, Premium-Discount Array, PD Arrays]
tags: [concept, pd-array, hub]
---

# PD Array

A **Premium-Discount array** is any chart structure ICT's algorithm references to reprice. PD arrays include [[concepts/fair-value-gap|FVGs]], [[concepts/order-block|order blocks]], [[concepts/breaker-block|breaker blocks]], [[concepts/balanced-price-range|balanced price ranges]], suspension blocks (a sub-class of FVG, see [[concepts/inversion-fair-value-gap|IFVG]]) and similar inefficiency / structural levels.

## The PD Array Matrix — selection framework

The matrix tells you **which** PD array the algorithm will use. Without it, every FVG / OB looks equally tradeable. With it, the high-probability arrays are isolated.

ICT calls the matrix "the source code" / "the sauce" of his methodology ([[sources/2025-pd-array-matrix]] @ 1:24:03 framing).

### Live selection signatures

The 2025-10-14 review adds a practical selection filter: the market often advertises the right array through a visible liquidity signature rather than through generic order-flow tools. In practice, watch for:

- an **old inefficiency** that behaves like an immediate rebalance rather than a deferred revisit ([[sources/ict-secret-to-selecting-algorithmic-pd-arrays-october-14-2025]] @ 1:27:58, @ 1:28:30),
- **relative equal highs** / lows where the smoother side is the likely draw ([[sources/ict-secret-to-selecting-algorithmic-pd-arrays-october-14-2025]] @ 1:30:01),
- a **new week opening gap** or first-presented FVG as the kickoff reference when it aligns with the active draw ([[sources/ict-secret-to-selecting-algorithmic-pd-arrays-october-14-2025]] @ 1:39:54, @ 1:41:44, @ 1:43:17),
- and the rule that a bullish array should not be forced into a full fill if the market is clearly leaving the discount portion open ([[sources/ict-secret-to-selecting-algorithmic-pd-arrays-october-14-2025]] @ 1:28:46, @ 1:29:28).

The TTrades clip "Why You're Failing with ICT Concepts" sharpens the same idea from the execution side: the problem is not lacking ICT concepts, but trying to trade too many arrays at once. The fix is to choose the one array you can see most cleanly, make the entry / stop rules repeatable, and let highs and lows or liquidity frame that array instead of competing with it ([[sources/why-youre-failing-with-ict-concepts]]).

### Quadrant grading

1. Take the **highest high and lowest low of the last 20 trading days** ([[sources/2025-pd-array-matrix]]).
2. Mark the **midline** = equilibrium / [[concepts/consequent-encroachment|consequent encroachment]] of the range.
3. Quarter the range with two more lines (upper-mid, lower-mid).
4. Only PD arrays in the **inner two quadrants** (upper-mid and lower-mid, around equilibrium) are considered "high probability." Extremes are ignored unless expecting full reversal ([[sources/2025-pd-array-matrix]]).

### Per-wick grading

Every premium candlestick wick is sub-divided the same way: high → upper quadrant → equilibrium → lower quadrant → close. Those four price levels get added to the notepad in order, highest to lowest ([[sources/2025-pd-array-matrix]]).

### High-probability qualifier

A FVG (or suspension block) is **smart-money grade** only when any part of its gap range **straddles / overlaps a quadrant line** ([[sources/2025-pd-array-matrix]] @ 43:55 vicinity). A gap floating entirely between two quadrant lines is "common grade" — 50/50.

The "Keys To Success In Troubled Markets" lecture reinforces the same matrix habit: the daily chart should be read in quadrants, with the lower half, upper half, and midpoint driving the decision instead of classic support/resistance line drawing ([[sources/2025-lecture-series-keys-to-success-in-troubled-markets-june-16-2025]] @ 6:04, @ 8:48, @ 15:20).

The 02/13/2025 Telegram execution shows the same structure in practice: the trader wants the first presented FVG, tracks the opening-range-gap high/low, and uses the halfway point / consequent encroachment as the active stop and management reference instead of treating the chart as a raw line grid ([[sources/nq-live-execution-using-analysis-i-shared-in-telegram-02132025]] @ 6:12, @ 9:03, @ 10:06, @ 13:09, @ 14:43, @ 15:30).

### Body-rule for bullish order flow

Bodies must stay **at or above the lower quadrant** of the relevant range. Equilibrium-to-upper-quadrant is "the meat." Closes below the lower quadrant make probability fall off sharply ([[sources/2025-pd-array-matrix]]).

### Upper-half vs lower-half behavior

- In the **lower half / at equilibrium**: rules are strict, no coloring outside the lines.
- In the **upper half**: price is permitted to consolidate, run stops, mark time — this is normal.

([[sources/2025-pd-array-matrix]])

The 04/20/2026 ATH lecture makes the matrix practical for a specific edge case: when price is at all-time highs with no structure above, toggle the **continuous contract** to bring previous ATHs back into view, then grade the longest premium wick to its consequent encroachment. That midpoint becomes the active PD array for the session. The lecture also introduces the **TGIF** level (20–30% weekly retracement) as a matrix-aligned target, and the **bolo** as a defensive stop placed outside the relevant quadrant line ([[sources/ict-2026-lecture-trading-ath-in-pd-array-matrix-april-20-2026]] @ premium wick grading, @ TGIF framework, @ bolo concept).

### Time + price agreement

A valid PD array at a quadrant is **not actionable until a [[timing/macros|macro window]] or session open aligns**. Time and price both must agree — this is the rule that links the matrix to the [[timing/silver-bullet-windows|Silver Bullet]] / macro framework ([[sources/2025-pd-array-matrix]]).

### Large-event override

When a single extreme daily candle dominates (range bigger than the prior 20-day range), grade **that candle's range first**; resume the 20-day look-back only after price escapes it ([[sources/2025-pd-array-matrix]]).

### Trending-market lookback

Use **40 or 60 day** look-back instead of 20 in parabolic / strongly trending markets (e.g. gold) ([[sources/2025-pd-array-matrix]]).

## The MM model nests inside the matrix

ICT states the second-stage reaccumulation / redistribution of the [[models/market-maker-buy-model|MMBM]] / [[models/market-maker-sell-model|MMSM]] "will always lay on one of these quadrants" ([[sources/2025-pd-array-matrix]] @ 1:24:03). The matrix is the substrate; the MM models walk across it.

## See also

- [[synthesis/how-to-use-pd-array-matrix]]
- [[concepts/fair-value-gap]]
- [[concepts/order-block]]
- [[concepts/consequent-encroachment]]
- [[concepts/discount-premium]]
- [[models/market-maker-buy-model]]
- [[timing/macros]]
