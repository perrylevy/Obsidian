---
type: concept
aliases: [Rejection Block, Reject Block]
tags: [concept, order-block, reversal]
---

# Rejection Block

A rejection block is the closing-price boundary of a swing that marks where price was rejected and then reversed. In the sources, ICT treats it as the level the market should not comfortably reclaim if the rejection is valid. The February 11, 2026 NFP Wednesday lecture makes the edge case explicit: after a touch of the wick / half-gap / consequent-encroachment area, a failed reclaim can be treated as the rejection-block entry idea ([[sources/ict-2026-smart-money-concepts-lecture-february-11-2026]] @ 53:27, @ 54:19, @ 55:10).

## Core idea

The rejection block is usually the last up-close candle or the lowest closing price in the swing:

- it defines the rejection boundary,
- price can revisit it as a retest / decision point,
- and if the market fails to reclaim it cleanly, the prior rejection remains in force.

## Why it matters

Rejection blocks show up in Turtle Soup and opening-range execution:

- they help define the working stop / invalidation area,
- they can sit beside an inversion fair value gap,
- and they often act as the level price must stay below or above to keep the narrative intact.

## Practical use

Use a rejection block when you want to know where the market failed to continue and where the reversal boundary really is.

## See also

- [[concepts/order-block]]
- [[concepts/inversion-fair-value-gap]]
- [[concepts/consequent-encroachment]]
- [[models/turtle-soup]]
- [[timing/opening-range]]
- [[sources/june-24-2024-nq-turtle-soup-short]]
- [[sources/2025-lecture-series-turtle-soup-deferred-entry-with-rejection-block]]
- [[sources/ict-2026-1st-hour-dealing-range-march-28-2026]]
