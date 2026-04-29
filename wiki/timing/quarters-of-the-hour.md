---
type: timing
aliases: [Quarter of the Hour, Quarters of the Hour, QOH]
tags: [timing, delivery, quarter-hour]
---

# Quarters of the Hour

The **quarters of the hour** are the recurring 15-minute subdivisions inside each hour: :00–:15, :15–:30, :30–:45, and :45–:00. In the price-delivery continuum material, these are the smallest repeating timing cells that let the operator watch for fresh FVG formation and session repricing on a stable cadence.

## Core idea

ICT repeatedly ties valid delivery to quarter-hour closes and the structures that appear at those boundaries. The useful working habit is:

- wait for the current 15-minute cell to complete,
- inspect whether it produced a valid array or imbalance,
- and then decide whether the next quarter has permission to continue, reverse, or stand still.

## Why it matters

This page exists because the quarter-hour grid is the timing scaffold underneath several other pages:

- [[timing/macros]] are the shorter entry windows that sit inside this grid,
- [[timing/first-presented-fvg]] often depends on the first 1-minute FVG that appears inside a quarter,
- and [[concepts/price-delivery-continuum]] treats the quarter as the natural evaluation unit for delivery.

## Practical use

Use the quarter-hour grid when you want to:

- anchor your read to the next 15-minute close,
- see whether a new FVG is being created or respected,
- or map a macro window onto the 15-minute rhythm instead of reading every candle in isolation.

## See also

- [[timing/macros]]
- [[timing/first-presented-fvg]]
- [[concepts/price-delivery-continuum]]
- [[sources/2025-price-delivery-continuum]]
