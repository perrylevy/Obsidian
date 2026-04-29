---
type: concept
aliases: [IR, Immediate Rebalance]
tags: [concept, pd-array, delivery]
---

# Immediate Rebalance

An **immediate rebalance** is a rapid repricing back to a specific reference level after an expansion move, rather than a slow deferred revisit later in the session. In ICT's framing, the market has already "booked" the level and is snapping back to it as part of delivery.

## Core idea

Immediate rebalance is different from a normal fair-value-gap reaction:

- an FVG can remain a deferred draw,
- an immediate rebalance is a fast return to a nearby reference price,
- and the point is the speed and finality of the repricing, not the existence of a blank zone.

The canonical source page on the concept already frames it as a PD array and contrast term for deferred FVG behavior ([[sources/what-is-icts-immediate-rebalance]]). Lecture 21 of the 2024 mentorship sharpens the live execution side: the candle expands, then the next candle trades back to the prior candle's opening price / reference, which is the rebalance signature ([[sources/2024-mentorship-lecture-21]] @ 12:39, @ 13:12). The September 4 tutelage clip shows the same signature after a first-FVG reclaim: the move returns to the prior candle reference and then continues toward the next liquidity draw ([[sources/2024-mentorship-tutelage-september-04-2024]] @ 9:31, @ 10:01).

## Relationship to delivery

Immediate rebalance is best understood as a delivery change:

- the market has moved away,
- it returns quickly to the prior reference,
- and that return is the actionable signature.

The 2025-10-14 PD-array review adds a crisp live example: an old inefficiency can itself become the immediate rebalance when price snaps back to the inefficiency's opening price / high, rather than waiting for a full slow revisit ([[sources/ict-secret-to-selecting-algorithmic-pd-arrays-october-14-2025]] @ 1:27:58, @ 1:28:30).

That is why it sits naturally beside [[concepts/change-in-state-of-delivery]] and [[concepts/price-delivery-continuum]].

## Why it matters

This matters because the trader should not treat every fast revisit as an ordinary FVG trade.

- If the move is immediate and one-sided, the cleaner expectation is often that the rebalance leg completes rather than dithers.
- The lecture material stresses that the target behavior is sharp and complete, not slow and incremental.
- In practice, this helps the trader avoid micromanaging the move with premature partials when the market is clearly delivering to a known reference.

## See also

- [[concepts/change-in-state-of-delivery]]
- [[concepts/price-delivery-continuum]]
- [[concepts/fair-value-gap]]
- [[concepts/new-week-opening-gap]]
- [[concepts/draw-on-liquidity]]
- [[sources/what-is-icts-immediate-rebalance]]
- [[sources/2024-mentorship-lecture-21]]
