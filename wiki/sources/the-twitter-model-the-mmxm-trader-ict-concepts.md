---
type: source
title: "The \"Twitter Model\" The MMXM Trader - ICT Concepts"
source_type: youtube
raw: "[[Clippings/The Twitter Model The MMXM Trader - ICT Concepts.md]]"
date_ingested: 2026-04-22
key_concepts:
  - external-liquidity
  - internal-liquidity
  - fair-value-gap
  - market-structure-shift
  - inversion-fair-value-gap
  - change-in-state-of-delivery
  - midnight-opening-price
  - daily-open
  - order-block
  - smt
tags: [source, derivative, mmxm, twitter-model]
aliases: ["Twitter Model", "The MMXM Trader Twitter Model"]
---

# The "Twitter Model" The MMXM Trader - ICT Concepts

This clip presents the MMXM Trader's “Twitter model” as a compact external-liquidity-to-internal-liquidity framework. The idea is to raid a prior obvious liquidity pool such as PDH or PDL, then drop into a lower-time-frame fair-value-gap, and use SMT plus a market-structure-shift or change-in-state-of-delivery as the entry trigger.

The model is fractal: the same logic can be read on daily/hourly/15m, or pushed up to weekly/4h/1h if that is the cleaner expression of the same draw. The practical rule is simple: sweep the external liquidity, wait for the reaction into the hourly FVG, confirm with MSS / CISD and SMT on the lower time frame, then trade back toward the internal target. The clip also folds in the midnight-open filter, using shorts above midnight and longs below it, with the daily open as an optional refinement in the later examples.

This is a good bridge source because it doesn't introduce a brand-new doctrine family; it packages ERL→IRL, FVG confirmation, SMT, and opening-price filtering into one repeatable operator model.

## Extra linkage

- [[concepts/external-liquidity]] — the swept target that starts the model
- [[concepts/internal-liquidity]] — the internal target the trade is framed into
- [[concepts/fair-value-gap]] — the hourly / lower-time-frame confirmation zone
- [[concepts/market-structure-shift]] — the trigger used with SMT
- [[concepts/change-in-state-of-delivery]] — alternate wording for the trigger logic
- [[concepts/midnight-opening-price]] — directional filter for long/short selection
- [[concepts/order-block]] — later example entry / continuation structure
- [[concepts/smt]] — confirmation on the lower timeframe
- [[models/internal-external-liquidity-model]] — canonical ERL / IRL framing

## See also

- [[models/internal-external-liquidity-model]]
- [[concepts/external-liquidity]]
- [[concepts/internal-liquidity]]
- [[concepts/fair-value-gap]]
- [[concepts/midnight-opening-price]]
