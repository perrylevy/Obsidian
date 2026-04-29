---
type: model
aliases: [MMBM, Market Maker Buy Model]
tags: [model, market-maker, swing]
---

# Market Maker Buy Model (MMBM)

A **swing-trading model** describing the full algorithmic round-trip ICT's "market maker" walks price through to deliver from a discount accumulation back up to a premium target.

## Status in this wiki

For Hermes-trading-analyst, the market-maker buy-model is best treated as a **larger swing-delivery framework** rather than one of many competing intraday triggers. Use it when the chart is clearly describing a bigger bullish round-trip, then let smaller execution models handle actual entries.

The MMBM is the bullish mirror of the [[models/market-maker-sell-model|MMSM]]. Both are taught together as a pair; the structure is symmetric ([[sources/2023-mentorship-market-maker-models]]). The 2022 mentorship Episode 2 demonstrates the bearish mirror (sell-model) live: accumulation at premium, sell-side delivery to discount, smart-money reversal, then rally back to premium — the full round-trip in a single session ([[sources/2022-ict-mentorship-episode-2]] @ 1:40, @ 35:22).

## Stages (mirror of MMSM)

| # | Stage | Role |
|---|---|---|
| 1 | Original consolidation | Distribution at premium ahead of the leg down |
| 2 | Sell side delivery | Run sellside liquidity, reach discount |
| 3 | [[concepts/smart-money-reversal|Smart money reversal]] | Apex at discount — bodies inside the PD array, only wicks exceed |
| 4 | First-stage accumulation | Bullish base inside the discount range |
| 5 | Buy side delivery | Rally up through the prior range |
| 6 | Second-stage reaccumulation | Pause / re-accumulate at a [[concepts/pd-array|matrix]] quadrant |
| 7 | Target | Original consolidation high (or beyond, into HTF buyside) |

## Derivative execution variant

A later derivative "conceptually" variant turns the buy model into a tightly-scoped intraday routine built around three elements:

- the **Asian session range** after the 2:00 a.m. New York close,
- the **first 30 minutes** of each hour between **7:00 and 11:00 a.m. ET**,
- and a bullish [[concepts/fair-value-gap|FVG]] retest as the actual entry mechanism ([[sources/calubs-model-conceptually-variant-1]] @ 2:25, @ 3:29, @ 4:02, @ 9:05).

In that framing:
- one side of the range is taken first,
- then the opposite side is taken,
- then price must accept back into the range or print a double-sweep retest before the long is valid ([[sources/calubs-model-conceptually-variant-1]] @ 2:43, @ 5:54, @ 6:46, @ 7:19).

Execution is explicitly mechanical:
- buy limit = **one tick above the FVG high**,
- stop = **one tick below the low**,
- stop rolls to cover costs once price trades halfway to first partial,
- first partial / terminus use the **lowest-hanging** NDOG / NWOG overlapping the Fibonacci extension rather than demanding a perfect projection ([[sources/calubs-model-conceptually-variant-1]] @ 4:02, @ 4:58, @ 6:31, @ 7:50, @ 8:23).

> [!note] Derivative source
> This variant is a derivative-teacher interpretation, not ICT-direct doctrine. It is useful as an execution heuristic layered on top of the model, but it should not be conflated with the direct ICT buy-model sources.
## Relationship to PO3 (AMD)

[[models/power-of-three|PO3]] (Accumulation / Manipulation / Distribution) can describe the internal delivery of a swing, but MMBM is the broader round-trip framework. PO3 nests inside MMBM as one way the leg unfolds, not the other way around.

The clearest mapping:

- Original consolidation ≈ PO3 **Accumulation**
- Sell-side delivery (manipulation leg down to take sellside) ≈ PO3 **Manipulation**
- Buy-side delivery rally back up ≈ PO3 **Distribution** (in the bullish sense — distributing accumulated longs into premium)

But MMBM names sub-stages within each (first-stage / second-stage accumulation, smart money reversal, role-flipping PD arrays) that PO3 does not. They are complementary, not synonymous ([[sources/2023-mentorship-market-maker-models]]).

## PD-array role flip at the apex

PD arrays passed during sell-side delivery (acting as **resistance** on the way down) become **support** on the way back up — same level, opposite role ([[sources/2023-mentorship-market-maker-models]] @ 51:43). This is the algorithmic logic for why a HTF FVG often holds first-test on the rally leg.

## Simpler models nest inside

[[models/silver-bullet|Silver Bullet]] and OTE / Model 2022 setups can occur **within** the MMBM at the first-stage accumulation, smart money reversal, or second-stage reaccumulation points ([[sources/2023-mentorship-market-maker-models]] @ 55:33–55:59). MMBM gives the macro context; SB / OTE are the entry tactics.

## Review-clip caution

The NQ heavy-manipulation review is consistent with the idea that a market-maker-style framework can still be present while the tape remains unusually noisy and difficult to execute. In that environment, the framework alone is not enough — stop discipline and macro timing matter more than assuming a clean, graceful round-trip ([[sources/nq-heavy-manipulation-review]] @ 8:16, @ 11:57, @ 15:16).

The 11/14/2025 general market commentary uses the buy-model language on the dollar index: once the pre-identified inversion FVG held and price reclaimed the opening price, the tape was effectively in a buy program. That is a reminder that MMBM is a higher-time-frame delivery framework, not an intraday reaction cue ([[sources/ict-general-market-commentary-november-14-2025]]).

The "$4,000 In 7 Minutes" clip uses the same family logic in mirror form: the morning sell-side sweep above all-time highs was treated as manipulation inside a larger bullish weekly profile, and only after the daily open / 2-day open had not been raided did the sell-model leg become the operative short read before the tape could rotate back into the buy-model framework ([[sources/4000-in-7-minutes-trading-my-ict-30m-po3-model]] @ 6:47, @ 7:46, @ 11:19).

## Risk & stop placement

- **Entry trigger**: inside the accumulation zone or at the smart-money-reversal apex, entered via a confluent PD array — discount FVG, breaker block, or OB within the accumulation ([[sources/internal-external-liquidity]] @ 10:47, @ 14:38). In live form, [[models/silver-bullet|Silver Bullet]] / OTE setups nested inside the MMBM give the tactical entry ([[sources/2023-mentorship-market-maker-models]] @ 55:33).
- **Stop placement**: below the accumulation-zone low (for the stage-one entry) or below the smart-money-reversal low (for the mid-model entry). Protecting beyond the structural low that defines the accumulation is non-negotiable; the MMBM is a higher-time-frame delivery framework, not an intraday reaction cue ([[sources/ict-general-market-commentary-november-14-2025]]).
- **Target**: distribution — the prior external buy-side liquidity the model is designed to reach. Scale at the midline / consequent encroachment on the way up and again at the first relative-equal-highs cluster before the final distribution extreme.
- **Invalidation**: a close below the accumulation zone after the reversal has been declared; on review-clip / heavy-manipulation days, execute smaller and tighter rather than defending a wider stop ([[sources/nq-heavy-manipulation-review]] @ 11:57, @ 15:16).

## See also
