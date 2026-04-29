---
title: "ICT 2024 Mentorship — Lecture #5 (August 9, 2024)"
type: source
tags:
  - source
  - ict-direct
  - 2024-mentorship
aliases:
  - "2024 Mentorship Lecture 5"
raw: "[[Clippings/ICT 2024 Mentorship  Lecture 5    August 9, 2024]]"
date_ingested: 2026-04-20
key_concepts:
  - "[[timing/asian-range]]"
  - "[[timing/new-york-local-time]]"
  - "[[concepts/new-day-opening-gap]]"
  - "[[concepts/breakaway-gap]]"
  - "[[concepts/liquidity-sweep]]"
  - "[[concepts/relative-equal-highs-lows]]"
  - "[[concepts/relative-equal-highs-lows]]"
  - "[[concepts/draw-on-liquidity]]"
  - "[[concepts/consequent-encroachment]]"
  - "[[concepts/fair-value-gap]]"
---

# ICT 2024 Mentorship — Lecture #5 (August 9, 2024)

Lecture 5 pushes the mentorship into the Asian-session workflow. ICT uses the 6:00 p.m. NY reopen, the 7:00–9:00 p.m. Asian window, and the new day opening gap as a live reference scaffold for how the market engineers initial liquidity, then seeks the opposite side once time comes online.

## Summary

- The **6:00 p.m. reopen** marks the new day opening gap. ICT immediately looks for price to move away from that gap, create a short-term buy-side / sell-side pool, and then return to the opposite side.
- If the market is lethargic at 6:00 p.m. and does not expand, that is a caution flag for the Asian session.
- The **Asian session begins at 7:00 p.m. NY local time** and is effectively a 7:00–9:00 p.m. window for the working trader.
- Once the 7:00 candle arrives, ICT wants to see the market trade back to the NDOG, then displace in the direction of the more obvious local liquidity draw.
- If price takes the short-term high, then the short-term low, and returns to the gap, that sequence is read as the algorithm calibrating and engineering liquidity rather than random chop.
- A clean **breakaway gap** is not simply a filled gap; it is a gap that starts to act like a launch point once time confirms the direction.
- The lecture closes by treating speed, distance, and relative equal highs as the telltale signs that the run has genuine intent.

## Practical takeaways

- Mark the 6:00 p.m. open and keep the most recent NDOG visible.
- Treat 7:00 p.m. NY as the Asian-session activation point.
- If the market is flat and unconvincing at 6:00 p.m., be willing to pass.
- After the initial pool is taken, wait for displacement away from the NDOG and only then look for continuation / entry.

## Extra linkage

- [[timing/asian-range]] — the 7:00–9:00 p.m. Asian window and its session-bias role
- [[timing/new-york-local-time]] — all of the timestamps are NY-local
- [[concepts/new-day-opening-gap]] — 6:00 p.m. reopen as the session anchor
- [[concepts/breakaway-gap]] — when the NDOG starts acting like launch fuel
- [[concepts/liquidity-sweep]] — the short-term high/low grabs that precede displacement
- [[concepts/relative-equal-highs-lows]] — the local high target after the initial pool is set
- [[concepts/relative-equal-highs-lows]] — the local low target if the market needs to reverse first
- [[concepts/draw-on-liquidity]] — the larger directional pull beyond the local chop
- [[concepts/consequent-encroachment]] — midpoint logic for any larger gap or inefficiency
- [[concepts/fair-value-gap]] — the displacement / inefficiency context around the run
