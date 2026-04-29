---
type: source
title: "Algorithmic Price Delivery - Live recorded lesson"
source_type: youtube
raw: "[[Clippings/Algorithmic Price Delivery - Live recorded lesson]]"
date_ingested: 2026-04-18
key_concepts: [liquidity, fair-value-gap, consequent-encroachment, order-block, dealing-range, discount-premium, low-resistance-liquidity-run, turtle-soup]
tags: [source, derivative, liquidity]
aliases: ["Algorithmic Price Delivery"]
---

# Algorithmic Price Delivery - Live recorded lesson

## Summary

- The algorithm is framed as doing two things: raiding liquidity or rebalancing inefficiency. When both are nearby, price often targets them together as a single repricing event ([[sources/algorithmic-price-delivery-live-recorded-lesson]] @ 0:28, @ 2:47).
- Relative equal highs/lows are treated as buy-side and sell-side liquidity pools that retail traders place stops around; the move is engineered into the opposing pool rather than being random ([[sources/algorithmic-price-delivery-live-recorded-lesson]] @ 1:02, @ 1:31, @ 5:54).
- The clip repeatedly uses nested PD arrays: FVG, breaker, OB, and consequent encroachment can overlap, and price often respects the CE midpoint before displacement ([[sources/algorithmic-price-delivery-live-recorded-lesson]] @ 4:26, @ 8:15, @ 11:53).
- The working logic is to wait for buyside liquidity to be engaged before shorting and sellside liquidity before longing, then offload into the opposing liquidity pool (@ 16:58).

## Extra linkage

- [[concepts/liquidity]] — algorithm’s two recurring jobs: raid liquidity / rebalance inefficiency
- [[concepts/consequent-encroachment]] — midpoint where the gap or imbalance often stalls
- [[concepts/discount-premium]] — premium / discount filter on the delivery leg
- [[concepts/dealing-range]] — delivery context when a range is already defined
- [[concepts/low-resistance-liquidity-run]] — clean repricing through the next pool
- [[models/turtle-soup]] — sweep-and-reverse logic when liquidity is harvested

## Key quotes

- **@ 0:28** — "the algorithm has two main roles it will repic to areas of liquidity or it will rebalance areas of inefficiency"
- **@ 2:47** — "the algorithm will repic to areas where there are both parameters in close proximity liquidity and inefficient price action"
- **@ 4:26** — "stopping dead at the consequent encroachment or the midpoint of that Gap"
- **@ 10:57** — "anything above that green line is a premium"
- **@ 16:58** — "we always want to wait for price to engage with buy side liquidity before we enter short"

## See also

- [[concepts/liquidity]]
- [[concepts/fair-value-gap]]
- [[concepts/consequent-encroachment]]
- [[concepts/order-block]]
- [[concepts/dealing-range]]
- [[concepts/discount-premium]]
- [[models/turtle-soup]]
- [[concepts/low-resistance-liquidity-run]]
