---
type: concept
aliases: [CISD, Change in State of Delivery]
tags: [concept, pd-array, structure]
---

# Change in State of Delivery (CISD)

A **change in state of delivery** is the precise price level where the market changes how it is delivering — the point ICT ties directly to the order-block opening price.

## Core idea

ICT's order-block framing is not just a zone story; it is a **delivery-change** story. The 2022 mentorship Episode 3 provides the earliest ICT-direct **"change in state of delivery"** framing: the opening price of a consecutive candle series marks where delivery flips — "the opening on that candle starts this series of delivery on the downside; when that opening price gets violated here it changes its state of delivery" ([[sources/2022-ict-mentorship-episode-3]]). This is the foundational precursor to the more formalized CISD definitions in later material.

The order-block opening price marks the point where price changes how it is being delivered, which is why the order-block level and the CISD are treated as the same price marker in the bearish case ([[sources/2025-price-delivery-continuum]] @ 32:15). Lecture 21 of the 2024 mentorship restates that live by calling the opening price "your change in the state of delivery" while the market is trading a Friday morning example ([[sources/2024-mentorship-lecture-21]] @ 1:33:54). The September 4 tutelage clip uses the same language again and ties it directly to a bearish order-block entry after the first FVG reclaim ([[sources/2024-mentorship-tutelage-september-04-2024]] @ 10:01).

The 02/23/2026 SMC lecture repeats the phrase on a Monday opening-range example: "change in the state of delivery with this order block opening price there" — reinforcing that CISD is the specific price marker, not a vague zone ([[sources/ict-2026-smart-money-concepts-lecture-february-23-2026]] @ 17:02).

The "My Forever Model" clip uses CISD in the same practical way: after manipulation and inversion through an inefficiency, the actual short or long is validated only when price closes through the delivery-change level and then pulls back to it ([[sources/my-forever-model-the-strategy-that-has-made-me-over-half-a-million-insane-value]]).

The breaker-block continuation clip uses that same rule in live form: first wait for the sweep, then wait for the close through the level, and only then treat the breaker retest as a valid continuation reference ([[sources/trade-continuations-using-breaker-blocks]]).

The TTrades clip "Why You're Failing with ICT Concepts" makes CISD even more practical by treating it as the one PD array a trader may choose to focus on. In that framing, the rest of the chart is not a set of equal candidates; highs, lows, and liquidity simply provide the structure around the delivery-change trigger ([[sources/why-youre-failing-with-ict-concepts]]).

## Bearish expression

For a bearish order block, the CISD is the **lowest opening price of the consecutive up-closed candles** that form the bearish order block ([[sources/2025-price-delivery-continuum]] @ 32:15).

That is why the bearish order-block level is not merely an area; it is a specific opening price that can act as the repricing point for the short idea.

## Relationship to order blocks

- [[concepts/order-block|Order Block]] is the PD-array container.
- CISD is the **specific delivery-change level** inside that framing.
- In practice, a market can trade back to the OB opening price / CISD, respect it, and then continue in the new direction ([[sources/2025-price-delivery-continuum]] @ 32:15).

## Relationship to IFVG continuation

Derivative-teacher IFVG material treats CISD as a continuation confirmation that can pair with or be substituted by an inversion FVG. In that framing, once the inversion and delivery change are present, continuation lower / higher becomes valid to anticipate ([[sources/how-to-trade-ifvg]] @ 4:00, @ 7:22).

The "$4,000 In 7 Minutes" clip shows CISD doing micro-execution duty: the one-minute order block was the setup, but the actual validation came from the 15-second CISD check before the short was treated as live ([[sources/4000-in-7-minutes-trading-my-ict-30m-po3-model]] @ 16:16, @ 16:42).

Because that equivalence comes from derivative-teacher material rather than ICT-direct doctrine, keep the distinction explicit.

## 9 AM CRT usage

The 9 AM CRT model uses the lower-timeframe purge / Turtle Soup plus **MSS or CISD** as the confirmation that the morning CRT has changed state and is ready for the order-block entry ([[sources/why-the-9-am-crt-model-could-change-your-life]] @ 3:11, @ 4:48, @ 7:45).

## Relationship to MSS

[[concepts/market-structure-shift|Market Structure Shift]] is the broader structural confirmation that the prior direction has broken down.

CISD is the sharper, level-based expression of where price changed how it was delivering. MSS and CISD often appear together, but CISD is the more precise price marker.

## See also

- [[concepts/order-block]]
- [[concepts/market-structure-shift]]
- [[concepts/fair-value-gap]]
- [[concepts/inversion-fair-value-gap]]
- [[concepts/pd-array]]
- [[timing/9-am-crt]]
