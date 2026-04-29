---
type: source
title: "How To Predict Daily Highs and Lows"
source_type: youtube
raw: "[[Clippings/How To Predict Daily Highs and Lows.md]]"
date_ingested: 2026-04-20
key_concepts:
  - midnight-opening-range
  - standard-deviation
  - daily-high
  - daily-low
  - power-of-three
  - fair-value-gap
  - order-block
  - volatility
  - london-session
tags: [source, review, midnight-opening-range]
aliases: ["Predict Daily Highs and Lows", "Midnight Opening Range Levels"]
---

# How To Predict Daily Highs and Lows

## Summary

- The clip uses the midnight opening range, not the New York open, as the working frame for projecting daily highs and lows.
- The range is measured from 00:00 to 00:30 New York time, then projected with standard-deviation levels to estimate where the day may reverse or expand.
- The method is explicitly probabilistic: it works best when volatility is normal and the market has a clear narrative; high-impact news days can distort the levels.
- The level map is meant to be used with power-of-three structure, session context, and other PD arrays rather than as a standalone signal.
- The main practical value is having a repeatable guide for where the market may print the daily extreme.

## Extra linkage

- [[timing/midnight-opening-range]] — the 00:00–00:30 frame used in the clip
- [[concepts/midnight-opening-price]] — the exact 00:00 anchor inside the range
- [[models/power-of-three]] — the daily accumulation / manipulation / distribution scaffold
- [[concepts/fair-value-gap]] — useful confluence on the route to the extreme
- [[concepts/order-block]] — another confluence tool mentioned in the explanation
- [[timing/new-york-local-time]] — all levels are plotted in NY-local time
- [[timing/macros]] — best treated as a session-window tool, not a blind all-day rule

## Key quotes

- **@ 0:18** — "the midnight opening range is literally just a 30 minute window at the start of the day"
- **@ 0:58** — "we are going to use that range and measure it and do standard deviations"
- **@ 2:38** — "we want to see the daily low ... form at those two standard deviation levels"
- **@ 3:04** — "on days with a lot of volatility ... those days going to bring a lot of volatility into the market"
- **@ 5:37** — "I'd absolutely recommend this"

## See also

- [[timing/midnight-opening-range]]
- [[models/power-of-three]]
- [[concepts/fair-value-gap]]
- [[concepts/order-block]]
- [[timing/new-york-local-time]]
