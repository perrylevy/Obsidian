---
type: source
title: "ICT Explains How To Trade Last Hour Macro"
source_type: youtube
raw: "[[Clippings/ICT Explains how to trade last hour macro]]"
date_ingested: 2026-04-20
key_concepts: [macros, draw-on-liquidity, order-block, change-in-state-of-delivery, fair-value-gap, breaker-block, no-trade, new-york-local-time]
tags: [source, macro, timing, ict]
aliases: ["Last Hour Macro", "Final Hour Macro", "Finite Hour Macro"]
---

# ICT Explains How To Trade Last Hour Macro

## Summary

- The last-hour macro is defined as the 3:15–3:45 New York local window, when the algorithm runs on liquidity that has not yet been engaged.
- The narrator describes the move as a spooling / fishing-line effect: price is being pulled toward the next pool of buy-side or sell-side liquidity, not reacting to sentiment.
- In a bullish context, the market can still trade down first, then reprice higher into the next liquidity pool; the same logic applies in reverse for bearish delivery.
- The order block is framed as a change in state of delivery, not as a single candle label, and the opening price can become the new fair-value reference after the shift.
- If there is no obvious setup, the rule is to do nothing and wait; the last 15–20 minutes before 4:00 can produce a clean final run.
- This source is the clearest canonical support in the vault for a reusable late-day macro window.

## Extra linkage

- [[timing/macros]] — canonical late-day macro window
- [[concepts/draw-on-liquidity]] — the macro runs on the next unengaged liquidity pool
- [[concepts/order-block]] — order block as change in state of delivery
- [[concepts/change-in-state-of-delivery]] — same delivery-shift idea, more explicit
- [[concepts/fair-value-gap]] — fair-value / repricing examples inside the macro
- [[concepts/breaker-block]] — broken reference reused in the later delivery leg
- [[concepts/no-trade]] — if no clear setup, do nothing
- [[timing/new-york-local-time]] — all anchors are NY local
- [[synthesis/how-to-use-price-delivery-continuum]] — late-day delivery context
- [[synthesis/how-to-use-order-blocks-and-dealing-ranges]] — OB / delivery-reuse context

## See also

- [[timing/macros]]
- [[concepts/order-block]]
- [[concepts/change-in-state-of-delivery]]
- [[concepts/draw-on-liquidity]]
- [[concepts/no-trade]]
