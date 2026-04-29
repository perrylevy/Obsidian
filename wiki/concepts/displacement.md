---
type: concept
aliases: [Displacement, Aggressive Displacement, Displacement Move]
tags: [concept, price-delivery, confirmation]
---

# Displacement

**Displacement** is aggressive, full-bodied price delivery in one direction that signals the algorithm is actively repricing — not rotating. It is the delivery signature that validates whether a liquidity event was a real turn versus noise, and it is what leaves behind the [[concepts/fair-value-gap|fair value gaps]] and [[concepts/order-block|order blocks]] that subsequent entries reference.

## Working definition

- Displacement is **an aggressive move with full-bodied candles** ([[sources/market-structure-shift-ict-concepts]] @ 0:20). The 2022 mentorship Episode 5 provides one of the earliest and most memorable formulations: "If you have a children's swimming pool and an elephant falls into it, the water is displaced. That's what you're looking for in price." Energetic, obvious moves validate setups; weak/anemic moves = no setup ([[sources/2022-ict-mentorship-episode-5]]). Episode 6 adds the **"beefy candle"** formulation: displacement must be energetic with "a lot of movement, big beefy bearish candle that closes low below this level" — the range between the displacement high and displacement low is the FVG zone ([[sources/2022-ict-mentorship-episode-6]]).
- It frequently prints as a [[concepts/fair-value-gap|FVG]] — a three-candle sequence whose outer wicks do not overlap ([[sources/internal-external-liquidity]] @ 0:37).
- The clip framing treats displacement and FVG as tightly coupled: the FVG is the visible footprint of displacement ([[sources/market-structure-shift-ict-concepts]]).

## Role in sequencing

Displacement is not the entry — it is the **validation event** that qualifies the prior sweep or draw and justifies using the array it leaves behind.

The canonical sequences in the wiki all route through displacement:

1. **Killzone + sweep + MSS + FVG entry.** The [[concepts/market-structure-shift|MSS]] is only meaningful when the move away from the sweep is aggressive enough to count as displacement; otherwise it is just a retrace ([[sources/internal-external-liquidity]] @ 1:56, [[sources/market-structure-shift-ict-concepts]]).
2. **Opening range + first-presented FVG.** The first FVG inside the opening window is only tradeable **after displacement and liquidity context make it meaningful** ([[sources/ict-opening-range-theory-1st-presented-fvg-logic]], [[sources/ict-the-first-presented-fvg-in-the-opening-range]]).
3. **Post-8:30 order block.** The 2024 mentorship lecture 1 is explicit: a down-closed candle becomes an order block because *"we have displacement. It took liquidity. And the market has been one-directional"* ([[sources/2024-mentorship-lecture-1]]).
4. **Asian-range / NDOG continuation.** After the initial pool is taken, wait for **displacement away from the NDOG** and only then look for continuation ([[sources/2024-mentorship-lecture-5]]).
5. **Silver bullet entries.** Entries require confirmation such as displacement back into the range, breaker blocks, order blocks, or FVGs ([[sources/am-silver-bullet-strategy-on-nq]]).
6. **Venom / time-distortion days.** Run the stop pool, validate the bullish displacement, then use the first presentable array or [[concepts/inversion-fair-value-gap|IFVG]] for continuation ([[sources/2025-lecture-series-ict-venom-example-may-12-2025]]).

## Relationship to related concepts

- [[concepts/fair-value-gap]] — the visible footprint of displacement; the gap is the array displacement creates.
- [[concepts/market-structure-shift]] — MSS is confirmed *by* a displacement leg; without displacement the break is suspect.
- [[concepts/change-in-state-of-delivery|CISD]] — the precise delivery-state flip that often coincides with the displacement candle's close.
- [[concepts/order-block]] — the last opposing candle before displacement becomes the OB.
- [[concepts/inversion-fair-value-gap]] — the post-displacement flip state when a prior FVG is violated.
- [[concepts/liquidity-sweep]] — the event displacement is meant to validate as a real turn.
- [[concepts/breakaway-gap]] — a displacement-scale gap that tends not to fill in the near term ([[sources/ict-forex-futures-market-review-october-4-2025]]).

## Operator use

- Treat a sweep without displacement as incomplete — wait, do not chase.
- Use displacement strength as a **quality filter**: failure to pull back to [[concepts/mean-threshold|mean threshold]] or [[concepts/consequent-encroachment|consequent encroachment]] after displacement is a strength signature in the displacement direction ([[sources/2024-04-18-ob-tape-reading]] @ 1:51:22).
- The array you trade after displacement (FVG, OB, breaker, IFVG) is selected by the [[concepts/pd-array|PD array matrix]], not by the displacement candle itself.

## See also

- [[concepts/fair-value-gap]]
- [[concepts/market-structure-shift]]
- [[concepts/change-in-state-of-delivery]]
- [[concepts/order-block]]
- [[concepts/inversion-fair-value-gap]]
- [[concepts/liquidity-sweep]]
- [[concepts/price-delivery-continuum]]
