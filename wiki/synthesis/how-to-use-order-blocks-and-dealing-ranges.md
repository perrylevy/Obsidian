---
type: synthesis
aliases: [Order Block and Dealing Range Playbook, Mean Threshold Playbook, OB Dealing Range Playbook]
tags: [synthesis, playbook, order-block, dealing-range, liquidity]
---

# How to Use Order Blocks and Dealing Ranges

This page is the operator guide for the order-block / dealing-range lecture. The source's practical lesson is that an order block is not just a shaded zone: it is a specific delivery-change area inside a dealing range, and the best entries depend on mean threshold, the composite candle structure, and whether a higher-time-frame bias already exists ([[concepts/order-block]], [[sources/2024-04-18-ob-tape-reading]] @ 47:47, @ 1:50:35, @ 2:18:09).

## Core idea

An order block sits inside a dealing range. The dealing range itself must have taken both sides of liquidity on the time frame being traded. Once that structure exists, the midpoint / mean threshold becomes the key execution reference.

## How to read the setup

### 1. Start with the dealing range

Do not call something a dealing range unless price has engaged both buyside and sellside liquidity on that timeframe. If only one side has been touched, the range is incomplete.

### 2. Identify the order block correctly

For a bearish OB, consecutive up-close candles define a composite range. The OB is not automatically the last candle unless the run was interrupted. For a bullish OB, the same composite logic applies on the downside.

### 3. Divide the range

Once the OB is found, divide it:
- in half to locate mean threshold,
- and in quarters if you want finer internal grading.

The source repeatedly says the best bearish entries form below mean threshold, while bullish entries should respect the upper portion of the range.

### 4. Respect the FVG interaction

If a fair value gap exists in the lower half of a bullish OB, do not force the upper down-close candle as the entry. The market will often reprice to the inefficiency first.

### 5. Use mean threshold as strength confirmation

If price does not even reach mean threshold before reversing, that is a sign of strength. Mean threshold is therefore both a quality filter and a diagnostic tool.

## Practical execution map

### A. Bearish OB

Use the full composite range of the up-close run.
- Prefer shorts below mean threshold.
- Treat the lowest open of the consecutive up-closes as the precise bearish OB level.
- If a lower down-close interrupted the run, then the uninterrupted structure changes the definition.

### B. Bullish OB

Use the composite down-close run.
- Prefer longs in the upper portion of the OB's internal range.
- If a lower-half FVG is present, wait for price to reprice there first.

### C. News driver days

On high-impact news days, do not force sub-5-minute precision immediately at release. Wait at least 15 minutes, and sometimes 30 minutes, before dropping lower.

## What to avoid

- Do not confuse an order block with a generic supply or demand zone.
- Do not ignore mean threshold.
- Do not assume the last candle always defines the block.
- Do not buy a bullish OB too low if a lower-half FVG is still open.
- Do not over-refine on a high-impact release candle.

## Fast checklist

Before acting, ask:
1. Has the dealing range taken both sides of liquidity?
2. Is the order block a composite range or a single candle?
3. Where is mean threshold?
4. Is there an FVG that will likely draw price first?
5. Is the time of day / news context appropriate?

## See also

- [[concepts/order-block]]
- [[concepts/dealing-range]]
- [[concepts/mean-threshold]]
- [[concepts/consequent-encroachment]]
- [[concepts/fair-value-gap]]
- [[timing/macros]]
- [[deferred/timing/killzones]]
- [[sources/2024-04-18-ob-tape-reading]]
