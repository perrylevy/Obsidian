---
type: model
aliases: [MMSM, Market Maker Sell Model]
tags: [model, market-maker, swing]
---

# Market Maker Sell Model (MMSM)

A **swing-trading model** describing the full algorithmic round-trip from a premium accumulation down to a discount target. Bearish mirror of the [[models/market-maker-buy-model|MMBM]] ([[sources/2023-mentorship-market-maker-models]]).

## Status in this wiki

For Hermes-trading-analyst, the market-maker sell-model is the **bearish swing-delivery mirror** of MMBM. Treat it as higher-time-frame context, not as a separate everyday scalp trigger.

## Stages

| # | Stage | Role |
|---|---|---|
| 1 | Original consolidation | Accumulation at discount ahead of the leg up |
| 2 | Buy side delivery | Run buyside liquidity, reach premium |
| 3 | [[concepts/smart-money-reversal|Smart money reversal]] | Apex at premium — bodies inside the PD array, only wicks exceed |
| 4 | First-stage distribution | Bearish topping inside the premium range |
| 5 | Sell side delivery | Drop down through the prior range |
| 6 | Second-stage redistribution | Pause / redistribute at a [[concepts/pd-array|matrix]] quadrant |
| 7 | Target | Original consolidation low (or beyond, into HTF sellside) |

## Curve metaphor

ICT teaches the MMSM as a **curve** — accumulation on the left, distribution at the apex, delivery on the right. The smart money reversal is the apex; the second-stage distribution is the right shoulder. Same logic in reverse for [[models/market-maker-buy-model|MMBM]] ([[sources/2023-mentorship-market-maker-models]]). The 2022 mentorship Episode 2 demonstrates this curve live in a bearish session: premium accumulation, sell-side delivery to discount (123 handles), then smart-money reversal and rally back — the full MMSM round-trip from a live account ([[sources/2022-ict-mentorship-episode-2]] @ 1:40, @ 35:22).

The 11/14/2025 general market commentary keeps the mirror logic alive in live tape form: if the higher-time-frame dollar thesis fails and price loses the key level, the bearish side of the round trip becomes the operative model. Treat the sell-model as the bearish companion to the buy-model, not as a separate intraday trigger ([[sources/ict-general-market-commentary-november-14-2025]]).

The "$4,000 In 7 Minutes" walkthrough is a clean PO3-style sell-model example: price expanded up first, then the morning manipulation / sweep above all-time highs set up the short, and only after that did the tape qualify for the bearish delivery leg back toward the 2-day open / daily-open targets ([[sources/4000-in-7-minutes-trading-my-ict-30m-po3-model]] @ 6:47, @ 7:46, @ 8:45, @ 10:51).

The 09/06/2024 OSOK execution and the 08/30/2024 PM-session turtle-soup clip are live sell-model mirrors: the market runs a stop raid, the trader waits for the larger bearish delivery context to assert itself, and the exit / add logic is then organized around the daily FVG midpoint rather than the initial spike ([[sources/ict-nq-live-execution-september-6-2024-100k-osok]] @ 1:15, @ 3:34, @ 8:14; [[sources/nq-pm-session-turtle-soup-long-full-pull-august-30-2024]] @ 1:15, @ 3:34, @ 8:14).

## PD-array role flip

PD arrays acting as **support** on the way up flip to **resistance** on the way down ([[sources/2023-mentorship-market-maker-models]] @ 51:43). On the redistribution / second-stage leg back to a prior PD array, expect price to reject — the algorithm is using the same level for the opposite role.

## Where it nests inside the matrix

The second-stage redistribution "will always lay on one of these quadrants" — referring to the [[concepts/pd-array|PD array matrix]] quadrants ([[sources/2025-pd-array-matrix]] @ 1:24:03). The MMSM doesn't float free; it walks across matrix quadrants.

## Relationship to PO3

See [[models/market-maker-buy-model#Relationship to PO3 (AMD)]] — the same applies in mirror form.

## Risk & stop placement

- **Entry trigger**: at the distribution high or on the redistribution leg back to a prior PD array that is flipping from support to resistance ([[sources/2023-mentorship-market-maker-models]] @ 51:43). The array must land in the correct [[concepts/pd-array|PD array matrix]] quadrant ([[sources/2025-pd-array-matrix]] @ 1:24:03).
- **Stop placement**: above the distribution high (for the primary short) or above the premium PD array being rejected (for the redistribution-leg short). The flipped PD array itself is the invalidation level — if price closes back above it, the role-flip failed.
- **Target**: the accumulation zone that the model is designed to reach on the way down. Scale at the midline and again at the first relative-equal-lows cluster before the accumulation extreme.
- **Invalidation**: full-body close back above the distribution high or the role-flipped array.

## See also
