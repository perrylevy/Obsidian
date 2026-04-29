---
type: synthesis
aliases: [PDC Playbook, Price Delivery Continuum Playbook, Continuum Playbook]
tags: [synthesis, playbook, delivery, liquidity]
---

# How to Use Price Delivery Continuum

This page is the operator guide for the **Price Delivery Continuum** framework. The practical rule is to keep cycling through the higher-time-frame and lower-time-frame layers, then decide whether the current quarter-of-the-hour is producing a tradable PD array or a high-resistance wait state ([[concepts/price-delivery-continuum]], [[sources/2025-price-delivery-continuum]] @ 12:33, @ 19:09, @ 21:01).

## Weekly-summary anchoring

The weekly summary clip shows the same continuum logic at a larger scale: the market is held in a weekly range until one side is taken, then the later expansion and inversion behavior map the delivery path across the rest of the week ([[sources/2025-lecture-series-nq-weekly-summary-02282025]] @ 3:39, @ 7:37, @ 31:59).

## News-driven opening example

The April 4 NQ NFP review shows the same continuum on a news-driven day: the first post-open FVG after the buyside sweep, the 9:50–10:10 macro, and the 3:15–3:45 PM continuation all behave like quarter-hour delivery checkpoints ([[sources/nq-nfp-algorithmic-price-delivery-04042025]] @ 0:33, @ 1:22, @ 3:39).

## Core idea

Price delivery is not a one-shot top-down read. It is a continuous scan across:
- the active higher-time-frame draw,
- the current lower-time-frame delivery leg,
- and the time window that gives the array permission to act.

The source treats time + OHLC as the only real inputs. That means the operator is always asking three questions:
1. Where is the current draw on liquidity?
2. Which half of the current imbalance is already efficient?
3. Is this quarter-of-the-hour producing a valid structure, or is the market in a high-resistance wait condition?

## How to read the continuum

### 1. Start with the active range

Define the relevant working range first. On the source framing, the range might be the current higher-time-frame band, the active session leg, or a dominant candle range that overrides smaller structure ([[concepts/price-delivery-continuum]], [[concepts/pd-array]], [[sources/2025-price-delivery-continuum]] @ 14:29).

### 2. Classify the move state

Ask whether the market is in:
- a low-resistance liquidity run,
- a high-resistance liquidity run,
- or a balanced-price-range condition inside part of an FVG.

If the market is not forming useful FVGs during the quarter, treat it as high resistance and wait for the next quarter instead of forcing execution.

### 3. Separate worked half from live half

When studying a bearish FVG, the upper half is the worked / balanced side and the lower half is the remaining imbalance. For a bullish FVG, reverse that logic.

This is the key operational filter:
- the worked half is not the remaining objective,
- the live half is the side still being delivered to,
- and the consequent encroachment is the midpoint reference that tells you when the market has already started balancing the structure.

### 4. Use time as a trigger filter

The lecture explicitly ties valid delivery to the quarter of the hour. If the setup is structurally valid but the timing window is dead, sit still. If the timing window is live and the array is clean, then the setup has permission to execute.

## Practical execution map

### A. When the market is low resistance

Use the current quarter to:
- confirm the active draw on liquidity,
- identify the live imbalance,
- and align with the session window before taking the trade.

This is the environment where FVGs are forming or being respected and the move can expand cleanly.

### B. When the market is high resistance

Do not invent a setup. If the quarter is producing no usable FVG structure, the source’s instruction is to wait in 15-minute increments and reassess.

High resistance is a pause state, not a failure state.

### C. When an FVG becomes a balanced price range

If price back-and-forths through the wrong half of the gap, that half has become balanced price range. The opposite half is the part still worth targeting.

This is where the operator stops treating the entire gap as equally actionable.

### D. When a breakaway gap or measuring gap appears

If the market launches with an unfilled breakaway gap, treat that as leg initiation. If a later gap functions as the midpoint projection, treat it as the measuring gap for the next measured move.

These are not interchangeable labels; they describe different points in the delivery sequence.

## What to avoid

- Do not use retail order-flow tools as the primary lens when the source is explicitly framing time + OHLC as sufficient.
- Do not assume every quarter will produce a trade.
- Do not treat the balanced half of a gap as the remaining imbalance.
- Do not force a low-resistance interpretation in a high-resistance tape.
- Do not skip the time filter just because the structure looks familiar.

## Fast checklist

Before trading this framework, ask:
1. What is the current draw on liquidity?
2. Is the market in low-resistance or high-resistance delivery?
3. Which half of the current gap is already balanced?
4. Is the current quarter of the hour actually producing structure?
5. Is there a clear breakaway / measuring / OB context around the move?

## See also

- [[concepts/price-delivery-continuum]]
- [[concepts/balanced-price-range]]
- [[concepts/high-resistance-liquidity-run]]
- [[concepts/low-resistance-liquidity-run]]
- [[concepts/breakaway-gap]]
- [[concepts/measuring-gap]]
- [[concepts/consequent-encroachment]]
- [[concepts/order-block]]
- [[timing/quarters-of-the-hour]]
- [[sources/2025-price-delivery-continuum]]
- [[sources/nq-nfp-algorithmic-price-delivery-04042025]]
- [[sources/smc-algorithmic-market-on-close-macro]]
- [[sources/nq-futures-review-04012025]]
