---
type: concept
aliases: [Volume Imbalance, VI]
tags: [concept, pd-array, candle-science]
---

# Volume Imbalance (VI)

A gap between the **bodies** (not wicks) of two **immediately adjacent candles** ([[sources/2024-04-18-ob-tape-reading]] @ 1:54:54).

## Distinction from FVG

- A [[concepts/fair-value-gap|FVG]] requires a 3-candle pattern with a wick-to-wick gap.
- A volume imbalance is the body-only gap between candles 2 and 3 of *any* sequence — wicks may overlap.

## Strength

**Weaker than an FVG.** Price can pass through a VI multiple times without invalidation ([[sources/2024-04-18-ob-tape-reading]] @ 1:59:08).

## Stop placement rule

When using a VI as confluence, the stop must sit **outside the candle that creates the imbalance** — not at the VI midpoint or edge ([[sources/2024-04-18-ob-tape-reading]] @ 2:00:47).

The "Keys To Success In Troubled Markets" clip uses the same idea live: a small one-minute imbalance inside the larger daily structure becomes the precision reference for the trade, but the real thesis still comes from the larger range and quadrant context ([[sources/2025-lecture-series-keys-to-success-in-troubled-markets-june-16-2025]] @ 17:52, @ 18:55, @ 19:48).

The 02/13/2025 Telegram execution uses the same body-vs-wick lesson in live form: bodies stay organized inside the upper half while the market works through the first-presented FVG / opening-range structure, even as the wick colors outside the lines and tags the PPI reaction ([[sources/nq-live-execution-using-analysis-i-shared-in-telegram-02132025]] @ 4:01, @ 6:12, @ 7:15, @ 8:28, @ 11:03, @ 12:23, @ 14:43).

The 05/08/2024 premium-wick entry clip uses VIs in the same live-scaling way: a small body imbalance can be used for adds, partials, and stop management while the larger daily FVG remains the real target ([[sources/nq-premium-wick-entry-live-execution-may-08-2024]]).

## Inclusion in FVG boundary

When drawing an FVG that has an adjacent VI, **include the VI inside the FVG range** — boundary expands to consume the VI ([[sources/mnq-pm-silver-bullet-walkthrough]] @ 0:36, @ 6:46). This produces a wider but more defensible FVG.

## See also

- [[concepts/fair-value-gap]]
- [[concepts/balanced-price-range]]
- [[concepts/candle-science]]
