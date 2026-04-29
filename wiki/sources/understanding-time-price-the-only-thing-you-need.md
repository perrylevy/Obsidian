---
title: "Understanding Time & Price - The Only Thing You Need"
type: source
source_type: youtube
raw: "[[Clippings/Understanding Time & Price - The Only Thing You Need.md]]"
date_ingested: 2026-04-21
key_concepts:
  - "[[timing/new-york-local-time]]"
  - "[[timing/macros]]"
  - "[[timing/lunch-macro]]"
  - "[[timing/opening-range]]"
  - "[[timing/first-presented-fvg]]"
  - "[[concepts/opening-range-gap]]"
  - "[[concepts/inversion-fair-value-gap]]"
  - "[[concepts/order-block]]"
  - "[[concepts/draw-on-liquidity]]"
  - "[[deferred/concepts/rejection-block]]"
tags: [source, ict-direct, lecture, time-price]
aliases: ["Understanding Time & Price"]
---

# Understanding Time & Price - The Only Thing You Need

## Summary

This clip frames ICT's full routine as a time-and-price map: the previous day's PM session range, the London session range, the AM session opening / opening-range-gap behavior, and the lunch pulse all matter because the algorithm repeatedly revisits specific liquidity pools at specific times.

- The PM session range is defined as the previous-day 1:30 p.m. to 4:00 p.m. New York local time range; its high/low become a reference for the next session.
- The London session range is treated as 2:00 a.m. to 5:00 a.m. New York local time and is used the same way: define the high/low, then look for a raid and delivery leg.
- The AM session / opening range is the 9:30 a.m. open through noon, with opening-range-gap behavior and the first valid liquidity draw in regular trading hours.
- The lecture emphasizes that RTH and ETH can both matter, but the execution frame should stay tied to the time-based chart, not noise on an arbitrary bar type.
- Lunch is another delivery pulse: once the morning has established structure, price often revisits the morning low or opening-range gap before continuing toward buy-side liquidity.
- The example trade shows an inversion fair value gap acting as dynamic support after reclamation, with the order block and stop placement managed around the gap rather than on top of it.

## Key quotes

- **0:09** — "the PM session ranges... 1:30 p.m. to 4 p.m"
- **1:54** — "if it's not that I'm looking at the London session raid"
- **2:56** — "opening range gaps takes place when you're utilizing regular trading hours"
- **4:20** — "the algorithm doesn't take lunch but it runs on that liquidity"
- **4:45** — "you have every advantage using a Time based chart"
- **7:04** — "that's an inversion fair value Gap ... it's going to go above it treat it as support"
- **9:18** — "everything that I've outlined here is shown to you on a Time based chart"

## Extra linkage

- [[timing/macros]] — the clip is basically a broad macro / session-rhythm lecture
- [[timing/lunch-macro]] — the lunch pulse is part of the routine
- [[timing/opening-range]] — AM open and opening-range-gap behavior
- [[concepts/opening-range-gap]] — regular-trading-hours gap behavior
- [[concepts/inversion-fair-value-gap]] — reclaimed IFVG acting as support
- [[concepts/order-block]] — stop placement and reclaimed OB behavior
- [[concepts/draw-on-liquidity]] — each session range defines the next draw map
- [[deferred/concepts/rejection-block]] — lunch retracement / raid-and-reverse logic
- [[timing/new-york-local-time]] — all windows are explicitly New York local time
- [[timing/first-presented-fvg]] — the AM opening logic still feeds into the first working array
