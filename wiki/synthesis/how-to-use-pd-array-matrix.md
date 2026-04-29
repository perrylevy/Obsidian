---
type: synthesis
aliases: [PD Array Matrix Playbook, Matrix Playbook, PD Matrix Playbook]
tags: [synthesis, playbook, pd-array, structure]
---

# How to Use PD Array Matrix

This page is the operator guide for ICT's **PD Array Matrix**. The source's practical message is that not every FVG, OB, or inefficiency is equally useful: the matrix grades the working range, identifies the high-probability quadrants, and only then tells you which array is worth acting on ([[concepts/pd-array]], [[sources/2025-pd-array-matrix]] @ 25:03, @ 38:09).

A useful simplification from the TTrades clip "Why You're Failing with ICT Concepts" is to choose one PD array as the primary trigger, then let highs and lows or liquidity frame the trade. The test is whether the model yields repeatable entry, stop, and journaling rules, not whether it can annotate every possible ICT concept on the chart ([[sources/why-youre-failing-with-ict-concepts]]).

## Core idea

The matrix is a selection framework, not just a chart annotation method. It answers:
- which price range is currently in play,
- where equilibrium sits,
- which quadrant line the array overlaps,
- and whether time has aligned yet.

If the range does not make the array salient, the array is just a mark on the chart.

## Live selection cues

The 2025-10-14 PD-array review makes the matrix feel more like a radar than a static map. The market advertises the right array through a few repeatable signatures:

- an old inefficiency that immediately rebalances instead of simply getting revisited later ([[sources/ict-secret-to-selecting-algorithmic-pd-arrays-october-14-2025]] @ 1:27:58, @ 1:28:30),
- relative equal highs / lows where the smoother side is the likely draw ([[sources/ict-secret-to-selecting-algorithmic-pd-arrays-october-14-2025]] @ 1:30:01),
- first-presented FVGs and new-week opening gaps that line up with the active draw and give the kickoff reference ([[sources/ict-secret-to-selecting-algorithmic-pd-arrays-october-14-2025]] @ 1:39:54, @ 1:41:44, @ 1:43:17),
- and a refusal to demand a full gap fill when the market is clearly leaving the bullish discount portion open ([[sources/ict-secret-to-selecting-algorithmic-pd-arrays-october-14-2025]] @ 1:28:46, @ 1:29:28).

## How to read the matrix

### 1. Establish the working range

Start with the highest high and lowest low of the last 20 trading days. If the market is parabolic or otherwise extended, widen the lookback to 40 or 60 days. In a dominant event candle, grade that range first before returning to the 20-day frame ([[concepts/pd-array]], [[sources/2025-pd-array-matrix]] @ 11:30, @ 24:02).

### 2. Quarter the range

Split the range into four bands:
- lower extreme,
- lower-mid,
- upper-mid,
- upper extreme.

The midline is the consequent-encroachment / equilibrium reference. The inner two quadrants are where the best actionable arrays tend to sit.

### 3. Grade the candlestick wick

Each important wick is also subdivided into quadrants. The source emphasis is to grade the wick from close to high for premium wicks, then log the internal levels in order. That lets you see whether the wick itself contains actionable delivery structure or only noise.

### 4. Only trust arrays that straddle a quadrant line

A fair value gap, suspension block, or similar inefficiency becomes high-probability when some part of it overlaps a quadrant boundary. If the array floats neatly between two lines, the source treats it as common-grade and therefore not especially compelling.

### 5. Confirm price and time together

The matrix is not actionable until a macro window or session open agrees with it. Price alone is not enough. Time alone is not enough. The setup needs both.

## Practical operating rules

### A. Inner quadrants are the main hunting ground

When the market is inside the inner quadrants, keep your attention there. The source treats these zones as the main habitat of the algorithm's useful PD arrays.

### B. Extremes are context, not default entries

The outer quadrants matter when you are expecting a broader reversal or a large extension, but they are not where the matrix places the most routine emphasis.

### C. The matrix is the spine under the model family

The PD Array Matrix is the skeleton beneath the PD array family, the OB family, and the reaccumulation / redistribution models. The point is not just to identify a pattern; it is to decide which pattern is actually active.

## What to avoid

- Do not treat every FVG or OB as equal.
- Do not ignore equilibrium.
- Do not trade a matrix setup before time agrees.
- Do not assume the same lookback works in every market regime.
- Do not overfit to the extreme edges when the source is emphasizing the inner quadrants.

## Fast checklist

Before trading the matrix, ask:
1. What is the active working range?
2. Is the range 20 days, or does it need a 40/60 day override?
3. Where is equilibrium / CE?
4. Does the array straddle a quadrant line?
5. Has time aligned yet?

## See also

- [[concepts/pd-array]]
- [[concepts/consequent-encroachment]]
- [[concepts/order-block]]
- [[concepts/fair-value-gap]]
- [[concepts/discount-premium]]
- [[timing/macros]]
- [[sources/2025-pd-array-matrix]]
