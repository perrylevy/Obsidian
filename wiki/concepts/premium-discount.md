---
type: concept
aliases: [Premium Discount, Premium/Discount, Premium and Discount, PD Array Matrix]
tags: [concept, pd-array, price-action, bias]
---

# Premium / Discount

In ICT, **premium** and **discount** describe the position of price relative to the **50% midpoint** of a reference range (typically the daily range). The algorithm treats this midpoint as a structural dividing line: above it is "expensive" (premium), below it is "cheap" (discount).

## Definition

- **Premium market** = price trading above the 50% midpoint of the reference range. Algorithms favor selling from premium ([[sources/2022-ict-mentorship-episode-2]] @ 35:22).
- **Discount market** = price trading below the 50% midpoint of the reference range. Algorithms favor buying from discount ([[sources/2022-ict-mentorship-episode-2]] @ 35:22).

The 50% level is found using Fibonacci retracement from the daily high to the daily low. Episode 4 demonstrates this in live ES and NQ examples: the equilibrium (50%) level is applied to the day's range, and the target sits beyond that midpoint at the old low or high ([[sources/2022-ict-mentorship-episode-4]]). Episode 7 identifies the equilibrium midpoint as the **consolidation hurdle zone**: when price stalls near 50%, daily bias becomes unclear and the trader must shift to intraday charts for "surgical strikes" rather than forcing directional trades ([[sources/2022-ict-mentorship-episode-7]]).

Episode 16 reiterates the same split in stronger terms: price is framed as moving from discount to premium and back again, with the daily midpoint acting as the key divider for whether the market is cheap or expensive ([[sources/2022-ict-mentorship-episode-16]]).

Episode 36 puts the same split into a live intraday frame: equilibrium is drawn across the active swing, no indicator is needed to read whether price is in premium or discount, and the trade is built from that visual midpoint rather than a lagging tool ([[sources/2022-ict-mentorship-episode-36]]).

## Trading logic

- **Bearish trades** (shorts): look for entries from premium, targeting discount. The algorithm reprices lower in sell programs regardless of temporary buying pressure ([[sources/2022-ict-mentorship-episode-2]] @ 35:22).
- **Bullish trades** (longs): look for entries from discount, targeting premium.
- **Target selection**: prefer "low-hanging fruit" targets (the 50% midpoint or nearby liquidity) rather than chasing extreme highs/lows.

## Relationship to PD Array Matrix

The 2022 mentorship Episode 2 uses a **simple 2-zone split** (premium above, discount below) as the foundational logic. Later ICT material (2025+) expands this into the **4-quadrant PD Array Matrix**:

- Premium + Premium (deep premium)
- Premium + Discount (near the 50% line from above)
- Discount + Premium (near the 50% line from below)
- Discount + Discount (deep discount)

Both formulations are valid. The 2-zone version from Episode 2 provides the foundational logic; the 4-quadrant version from 2025 provides finer granularity for array selection. See [[concepts/pd-array]] for the full matrix system.

## Relationship to other concepts

- **Consequent encroachment (CE)** — the midpoint of an FVG. When price trades into an FVG from premium/discount, the CE acts as a precision target or invalidation level ([[sources/2025-price-delivery-continuum]] @ 04:38).
- **Mean threshold** — the midpoint of an order block, analogous to CE but for OBs ([[concepts/mean-threshold]]).
- **Draw on liquidity (DOL)** — the 50% midpoint itself can act as a DOL when price is extended to one side of the range ([[sources/2022-ict-mentorship-episode-2]] @ 35:22).

## Historical note

The premium/discount concept appears in Episode 2 (January 2022) as one of ICT's early formulations. The terminology and the 50% midpoint logic remain consistent through 2025-2026 material, though the quadrant system was added later. This makes Episode 2 a high-weight foundational source for the concept.

## See also

- [[concepts/pd-array]] — the hub page for PD array selection and the 4-quadrant matrix.
- [[concepts/discount-premium]] — upper/lower half of a reference range (synonymous terminology).
- [[concepts/consequent-encroachment]] — the FVG midpoint.
- [[concepts/draw-on-liquidity]] — the next pool the algorithm targets.
- [[concepts/fair-value-gap]] — the flagship PD array that often forms at premium/discount transitions.
