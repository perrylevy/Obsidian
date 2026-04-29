---
type: source
title: "Stop Losses in Trading: Know When You're Wrong"
source_type: youtube
raw: "[[Clippings/Stop Losses in Trading Know When You're Wrong.md]]"
date_ingested: 2026-04-22
key_concepts:
  - protected-highs-lows
  - fair-value-gap
  - change-in-state-of-delivery
  - order-block
  - breaker-block
  - invalidation
  - continuation-entry
tags: [source, risk-management, stop-loss, protected-swings, trade-management]
aliases: ["Stop Losses in Trading", "Know When You're Wrong"]
---

# Stop Losses in Trading: Know When You're Wrong

This clip is a stop-loss and invalidation lesson built around protected swings. The core idea is that a stop should live beyond a swing that has actually earned protection, not on the nearest obvious wick.

The lesson starts from the protected-swing definition: a swing becomes protected after price reaches into an important level such as a sweep or fair-value gap and then closes back through the relevant candle structure. From there, the trader can place invalidation beyond that protected low or high and use that structure as the anchor for trend continuation or reversal planning.

A second takeaway is that stop placement depends on the model being used. If the chosen PD array is based on change-in-state-of-delivery, order blocks, breaker blocks, or fair-value-gap behavior, the invalidation should be decided relative to that array rather than forced onto a generic candle extreme. The clip also notes that if the risk-to-reward is too tight at the protected swing, a body-based stop or continuation entry may be the cleaner way to make the trade work.

## Extra linkage

- [[concepts/protected-highs-lows]] — the protected swing that justifies the stop
- [[concepts/fair-value-gap]] — one of the important-level triggers for protection
- [[concepts/change-in-state-of-delivery]] — the model family used to frame invalidation
- [[concepts/order-block]] — another PD array family mentioned for invalidation decisions
- [[concepts/breaker-block]] — another invalidation reference the clip explicitly allows
- [[deferred/concepts/holding-trades]] — related trade-management discipline once in the position
- [[sources/stop-getting-stopped-out-with-this-simple-concept-protected-highs-lows]] — nearby derivative lesson on protected swings

## See also

- [[concepts/protected-highs-lows]]
- [[concepts/fair-value-gap]]
- [[concepts/change-in-state-of-delivery]]
- [[concepts/order-block]]
- [[concepts/breaker-block]]
- [[deferred/concepts/holding-trades]]
