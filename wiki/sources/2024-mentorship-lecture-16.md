---
title: "ICT 2024 Mentorship — Lecture #16 (August 24, 2024)"
type: source
tags:
  - source
  - ict-direct
  - 2024-mentorship
aliases:
  - "2024 Mentorship Lecture 16"
raw: "[[Clippings/ICT 2024 Mentorship  Lecture 16  August 24, 2024]]"
date_ingested: 2026-04-20
key_concepts:
  - "[[deferred/concepts/event-horizon]]"
  - "[[concepts/new-day-opening-gap]]"
  - "[[concepts/new-week-opening-gap]]"
  - "[[concepts/opening-range-gap]]"
  - "[[timing/first-presented-fvg]]"
  - "[[concepts/balanced-price-range]]"
  - "[[concepts/inversion-fair-value-gap]]"
  - "[[concepts/order-block]]"
  - "[[concepts/volume-imbalance]]"
  - "[[models/turtle-soup]]"
---

# ICT 2024 Mentorship — Lecture #16 (August 24, 2024)

Lecture 16 is a dense chart-annotation and delivery lecture. ICT shows how to build a daily session journal from screenshots, but the real trading takeaway is that price should be read against a stack of higher-timeframe references: NDOG, NWOG, the opening-range gap, the first presented FVG, balanced price ranges, and the event horizon between adjacent opening gaps. The lecture then uses Friday's NQ action to show how those references line up into a very specific algorithmic narrative.

## Summary

- The lecture is framed as a chart-annotation routine: capture screenshots, log each segment of price action, and use your own charts rather than passively consuming the stream.
- ICT wants the trader to keep a daily record of what was useful on each day, what price did around the key arrays, and how the session behaved relative to higher-timeframe expectations.
- On the daily chart, a bearish order block, a volume-imbalance / buy-side inefficiency, and the corresponding consequent-encroachment line are used as the higher-timeframe delivery map.
- The **event horizon** is introduced as the midpoint between adjacent NDOG / NWOG structures; it behaves like a black-hole draw when those gaps are close together.
- For NWOGs, ICT gives a practical lookback limit of about **60 days** before the gap loses interest for this specific use case.
- The lecture explicitly restates that the **first fair value gap of the morning must form at 9:31 or later**, not on the 9:30 candle, if it is to qualify as the first-presented FVG under RTH rules.
- The 9:30–10:00 opening range is then treated as a live structure: if the first valid FVG and the opening-range gap align, price can draw to the gap midpoint, reject the upper half, and later continue toward the day’s higher-timeframe target.
- ICT uses the live NQ example to show that a seemingly bullish early pump can still be a setup for a Turtle Soup-style failure, an IFVG reclaim, or a move back toward the remaining undelivered half of the opening range gap.

## Practical takeaways

- Use your own screenshot journal to build a repeatable view of what price is doing around the important arrays.
- Treat NDOG/NWOG clusters as a mapped draw; if they are close together, the midpoint between them is a meaningful event horizon.
- Do not accept a 9:30 candle as the first-presented FVG if the RTH toggle would remove it; the earliest valid one is 9:31.
- When the opening-range gap and first-presented FVG are aligned, expect the market to respect the gap structure in a very specific sequence: sweep, partial delivery, rejection, continuation.
- Keep the volume-imbalance / BPR distinction in mind: the worked half is not the live imbalance.

## Key quotes

- **0:17** — "it's a review and it's more or less an exercise on showing my son and all of you ... how to annotate your chart"
- **10:00** — "you want to get that midpoint because you're anticipating it"
- **24:30** — "did you notice that it failed there"
- **30:05** — "that right there is my event horizon"
- **32:27** — "can't be older than 60 days"
- **38:01** — "the fair value gap here that forms minimum 931"
- **42:43** — "carry that fair value gap throughout the entirety of the day until when 345"

## See also

- [[deferred/concepts/event-horizon]]
- [[concepts/new-day-opening-gap]]
- [[concepts/new-week-opening-gap]]
- [[concepts/opening-range-gap]]
- [[timing/first-presented-fvg]]
- [[concepts/balanced-price-range]]
- [[concepts/inversion-fair-value-gap]]
- [[concepts/order-block]]
- [[concepts/volume-imbalance]]
- [[models/turtle-soup]]
- [[timing/macros]]
