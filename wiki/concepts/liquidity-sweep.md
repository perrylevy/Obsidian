---
type: concept
aliases: [Liquidity Sweep, Sweep, Stop Run]
tags: [concept, liquidity, reversal]
---

# Liquidity Sweep

A **liquidity sweep** is price trading through a visible liquidity pool and then reversing. In ICT / derivative-teacher language this is the same basic idea as a **Turtle Soup** / false breakout ([[sources/how-to-trade-turtle-soups]] @ 2:35, [[sources/nq-review-april-30-2025]] @ 7:55, @ 9:04, [[sources/nq-heavy-manipulation-review]] @ 13:09, [[sources/2022-ict-mentorship-episode-2]] @ 18:22). Episode 4 demonstrates the sweep in live ES and NQ examples: price runs above old highs (liquidity rest), then breaks down with market structure shift and FVG entry ([[sources/2022-ict-mentorship-episode-4]]). Episode 7 frames the sweep as the **daily bias validation trigger**: on a bearish daily bias, price must first take out sell-side liquidity (sweep below old low) before the MSS confirms the bias and the FVG entry is taken ([[sources/2022-ict-mentorship-episode-7]]).

The key distinction is that a sweep alone is only the raid; it becomes an MSS only when price then trades away with structural confirmation. Faiz SMC's March 2023 video makes that separation explicit and uses it to define a high-probability MSS setup ([[sources/secret-way-to-identify-high-probability-market-structure-shifts]] @ 1:49, @ 3:33, @ 5:29, @ 6:24).

The 08/27/2024 premarket NQ clip is a simple intraday example: the market tests the order block, then the trailing logic expects price to run toward the NDOG and other sellside pools rather than hold the original short-sweep direction ([[sources/premarket-nq-ob-to-discount-ndog-august-27-2024]]).

Lecture 5 of the 2024 mentorship adds a session-structure version: after the 6:00 p.m. reopen, ICT wants to see the market take a short-term high or low, then return to the NDOG, then go after the opposite side once the Asian window is active ([[sources/2024-mentorship-lecture-5]]).


## Working definition

- Price runs through a prior high or low where stops are resting.
- The move immediately rejects or reverses instead of cleanly continuing.
- The sweep often exists to clear one side of the market before price rebalances in the opposite direction ([[sources/nq-review-april-30-2025]] @ 7:55, [[sources/nq-heavy-manipulation-review]] @ 13:09).

## Overlapping labels absorbed here

- **Stop raid / stop run** is treated as a synonym for liquidity sweep unless a source makes a stricter distinction.
- **Swing failure pattern (SFP)** is treated as the structural close-back-through-the-level version of the same event.
- **Turtle Soup** remains the named trade model built on top of this sweep event, not a separate primitive from it ([[models/turtle-soup]], [[sources/simple-power-of-three]] @ 6:22).
- **Inducement** (SMC term) is the engineered pool being swept — same mechanism as a liquidity sweep viewed from the execution side. In PO3 language it maps to the Manipulation phase; the session-timed instance is the [[concepts/judas-swing]]. Do not fork a separate page.

## NQ examples in this batch

- **London low sweep** on April 30: price went below the 3:00 a.m. London sell-side pool, then validated the long and ran higher ([[sources/nq-review-april-30-2025]] @ 7:55, @ 9:04).
- **Turtle Soup false breakout** on the heavy-manipulation review: the market ran sell-side liquidity, then reversed after the short entry was framed as a false breakout environment ([[sources/nq-heavy-manipulation-review]] @ 12:49, @ 13:09).
- **Old daily low / buy-side pool re-uses** on May 1 show that once a sweep has occurred, the level can still be relevant for later re-tests and continuation ([[sources/2025-lecture-series-nq-may-01-2025-review]] @ 16:31, @ 22:29).

## See also

- [[models/turtle-soup]]
- [[concepts/liquidity]]
- [[concepts/draw-on-liquidity]]
- [[concepts/inversion-fair-value-gap]]
- [[concepts/order-block]]
- [[sources/secret-way-to-identify-high-probability-market-structure-shifts]]
