---
type: concept
aliases: [OB, Order Block]
tags: [concept, pd-array, order-flow]
---

# Order Block (OB)

A PD array defined by specific opposite-color candles preceding a directional displacement.

## ICT's strict definition

**Bearish order block**: a couple of consecutively **up-closed candles** whose **lowest opening price** marks the OB. The lowest-open price also marks a [[concepts/change-in-state-of-delivery|change in state of delivery (CISD)]] ([[sources/2025-price-delivery-continuum]] @ 32:15). The 2022 mentorship Episode 9 provides an early ICT-direct formulation: "Consecutive down-closed candles right before a price surge that has an imbalance — that's how you find your order blocks" — the consecutive opposite-color candles preceding displacement form the block, and the imbalance (FVG) within it is the entry zone ([[sources/2022-ict-mentorship-episode-9]]).

Episode 12 sharpens the definition further: an order block is a **consecutive series** of same-direction candles (all up-closed for bearish, all down-closed for bullish) that **contains an imbalance within it**. ICT explicitly distinguishes this from the common SMC interpretation: an order block is **NOT** simply "the last candle before a reversal" — it must be a multi-candle series with internal imbalance ([[sources/2022-ict-mentorship-episode-12]]).

Episode 13 adds the **three-part trade-entry filter** — all three must be present for a high-probability OB setup ([[sources/2022-ict-mentorship-episode-13]]):
Episode 18 tightens the practical workflow: start on the daily chart, mark previous-day highs/lows, transpose to the hourly and 15-minute charts, and wait for New York-session displacement before treating the OB as valid for entry ([[sources/2022-ict-mentorship-episode-18]]).

1. **Gap / Imbalance** — an unfilled price area (FVG) inside the candle series.
2. **Directional closed candle** — down-closed for bullish OB; up-closed for bearish OB.
3. **Underlying liquidity narrative** — price is likely to reach for buyside liquidity (bullish) or sellside liquidity (bearish).

> "It must have the imbalance coupled with the down closed candle and the underlying narrative that it's likely to go higher to reach for buy side liquidity — period."

This turns the OB from a structural shape into a tradable setup by requiring the destination to be visible before entry.

Lecture 6 of the 2024 mentorship gives a more execution-oriented restatement of the same rule: once later price closes below the opening price of the up-closed candle, that opening price can be treated as the bearish order-block validation line, and the first uptick back into the opening-price / low portion of the candle becomes the short-entry location ([[sources/2024-mentorship-lecture-6]]).

> [!note] Precision vs common usage
> ICT explicitly defines OB by a **specific price** (lowest open of consecutive up-closes for bearish), **not** as a shaded "supply zone." "A couple of up-close candles consecutively are a bearish order block" — and the OB level is the lowest of their opens ([[sources/2025-price-delivery-continuum]] @ 32:15). This is tighter than the loose "last up-close before a down move" framing common in SMC material.

## Mirror: bullish order block

A **cluster of consecutively down-closed candles** acting as a basing structure before a bullish displacement ([[sources/mnq-pm-silver-bullet-walkthrough]] @ 29:45). A single down-closed candle preceding a buy program also qualifies ([[sources/nq-live-tape-reading-am-review]] @ 4:49).

Episode 16 reinforces the bullish mirror in a higher-timeframe context: the bullish order block is the down-close structure that acts as support in discount markets, and it sits inside a broader premium/discount framework rather than a retail supply/demand story ([[sources/2022-ict-mentorship-episode-16]]).

Episode 35 re-emphasizes the practical read: the low, the open, and the middle of the candle are the sensitive areas, and the middle point / 50% threshold is the main continuation line for the OB ([[sources/2022-ict-mentorship-episode-35-order-block-and-smt-divergence]]). Episode 37 uses the same down-closed candle idea as a journaling anchor: mark the OB, record the target liquidity, and treat the setup as a study object rather than a signal service ([[sources/2022-ict-mentorship-episode-37]] @ 17:49, @ 18:14, @ 21:21).

Recent NQ reviews keep that rule practical: a bullish entry can be framed off the low of a small [[deferred/concepts/gray-pool|gray-pool]] / discount-wick structure, or off a consecutive down-close cluster that serves as the bullish shoulder block before continuation ([[sources/2025-lecture-series-nq-may-01-2025-review]] @ 11:59, @ 18:12). EP8 adds a derivative nuance: after the original bullish order block has already reacted, a later down-closed candle body can become a [[deferred/concepts/propulsion-block|propulsion block]] whose upper quadrant acts as the refined continuation sensitivity zone ([[sources/ep8-the-daily-range]] @ 4:54).

> [!note] Highest-open rule still partially unverified
> By symmetry with the strict bearish definition (lowest open of consecutive up-closes), the bullish OB level should be the **highest opening price** of consecutive down-closes. ICT did **not** state this single-price rule in [[sources/2024-04-18-ob-tape-reading]]. Instead he gave a **positional** rule: the entry candle should sit in the **upper portion** of the OB's internal [[concepts/dealing-range|dealing range]] — above [[concepts/mean-threshold|mean threshold]] (@ 2:20:52, @ 2:21:21). The two rules are compatible but not identical; the strict price-level mirror remains pending an ICT-direct statement.

## Composite range rule (multi-candle OBs)

A bearish OB formed by **multiple consecutive up-closed candles** uses the **entire composite range** of those candles — not just the last one. [[concepts/mean-threshold|Mean threshold]] (midpoint of the composite) is the quality-entry anchor; **best shorts form below mean threshold** ([[sources/2024-04-18-ob-tape-reading]] @ 2:03:51, @ 2:07:30, @ 2:17:38).

The "last candle only" rule applies **only when** a down-closed candle breaks the green run before the final up-close — otherwise the entire run is the OB.

## OB as a micro dealing range

ICT explicitly: **"your order block is what — it's a dealing range — but very specific with this part"** ([[sources/2024-04-18-ob-tape-reading]] @ 2:08:29). The OB's internal range is graded with the same equilibrium / quadrant logic as a HTF [[concepts/dealing-range|dealing range]]. Mean threshold = midpoint = equilibrium. The bullish-OB upper-portion entry rule follows from this.

## Bullish OB precision rule

Ideal long entries inside a bullish OB are in the **upper portion** of the retracement dealing range, **not** the lower half ([[sources/2024-04-18-ob-tape-reading]] @ 2:20:52).

**Exception**: if a [[concepts/fair-value-gap|FVG]] exists in the lower half of the same range, **skip** the upper down-close candle — price will reprice to the FVG+OB confluence in discount first ([[sources/2024-04-18-ob-tape-reading]] @ 2:21:21).

The 09/01/2024 top-down review gives the live weekly version of the same idea: price can trade down into the opening price of a bullish order block, use that opening price as the delivery-change line, and then rally back out once the lower portion of the weekly inefficiency has been worked ([[sources/top-down-trade-review-september-01-2024]] @ 8:46, @ 10:07, @ 25:52, @ 33:43).

The 08/27/2024 premarket NQ clip uses the same framework in a tighter intraday form: the short starts in an order block, the stop sits beyond a rejection block, and the market is expected to work back toward the NDOG rather than simply continue in a vacuum ([[sources/premarket-nq-ob-to-discount-ndog-august-27-2024]]).

## Definition framing

The 2022 mentorship Episode 3 provides the earliest ICT-direct **"change in state of delivery"** framing: the opening price of a consecutive candle series marks where delivery flips from sell-side to buy-side (or vice versa). When that opening price is violated, the market changes its state of delivery — "it was offering sell side, when it goes above that opening now it's offering buy side" ([[sources/2022-ict-mentorship-episode-3]]). This is the precursor to the more formalized OB definitions in later material.

Episode 19 compresses the same stack into a short execution lesson: the order block is the delivery-change level, the Judas swing is the counter-move that engineers the trap, and PO3 is the broader delivery scaffold that explains the sequence ([[sources/2022-ict-mentorship-episode-19]]).

Episode 22 uses the same bearish-order-block idea on the daily chart before the SMT divergence and FVG sequence unfolds ([[sources/2022-ict-mentorship-episode-22]]).

ICT characterises an OB as **"the change in the state of liquidity… where the marketplace changes its delivery… a very specific time, specific elements, a very unambiguous range in price"** ([[sources/2024-04-18-ob-tape-reading]] @ 1:50:35). Not related to DOM / time-and-sales. The "block of time" framing: the OB is the block of time **"that sets and establishes the order in which price will change its state of delivery"** — "order" = ordering / coordinating delivery, not buy/sell orders in the book ([[sources/2025-pd-array-matrix]] @ 1:01:57).

## Relationship to CISD

The OB level (lowest open of consecutive up-closes, for bearish) coincides with the [[concepts/change-in-state-of-delivery|CISD]] — they are two names for the same price level ([[sources/2025-price-delivery-continuum]] @ 32:15).

The 02/23/2026 SMC lecture repeats that live on a Monday chart by naming the "order block opening price" as the change in state of delivery, then using the opening-range / CE check to decide whether the market has really left the high-resistance state ([[sources/ict-2026-smart-money-concepts-lecture-february-23-2026]] @ 17:02, @ 13:00, @ 13:32).

The "$4,000 In 7 Minutes" walkthrough shows the order-block / CISD stack in miniature: after the 1-minute order block appeared, the trader waited for 15-second CISD confirmation before treating the short as valid ([[sources/4000-in-7-minutes-trading-my-ict-30m-po3-model]] @ 16:16, @ 16:42).

The TTrades continuation clip makes the same idea operational: once reversal confirmation exists, the next trade is often a continuation entry into a fresh order block, FVG, or swept level rather than a chase of the original turn. That makes the order block part of a sequence, not a one-shot event ([[sources/trade-continuations-using-order-blocks]]).

The 02/04/2025 Forex review also names a bearish propulsion block on the daily dollar index, while the pound-dollar side shows a bullish order block on the 15-minute chart. That is the live example of an order block acting as a high-time-frame decision level rather than a generic zone ([[sources/2025-lecture-series-smc-forex-review-02042025]] @ 5:40, @ 6:09, @ 16:04, @ 16:31).

## Stop-loss placement in order blocks

ICT specifies a concrete stop-loss rule for OB-based entries ([[sources/2022-ict-mentorship-episode-13]]):

- **Initial stop**: place below the **low of the order block candle**, not inside the OB itself.
- Placing stops inside the OB leads to premature exits — price commonly probes the OB before continuation.
- Once price rallies (bullish context) and forms **new down-closed candles**, stops can be **raised** below the new candle low.
- This trailing-stop logic uses the OB framework for both initial protection and ongoing management.

> "If I put my stop loss inside this area here I'm stopped out prematurely."

The stable **pyramid position sizing** (3-2-1, largest base first) from Episode 13 complements this: the largest position enters at the earliest, best-priced entry near the OB retest, with stop below the OB low ([[sources/2022-ict-mentorship-episode-13]]).

## See also
- [[concepts/change-in-state-of-delivery]]
- [[concepts/breaker-block]]
- [[concepts/fair-value-gap]]
- [[deferred/concepts/gray-pool]]
- [[concepts/pd-array]]
- [[concepts/dealing-range]]
- [[concepts/mean-threshold]]
- [[concepts/discount-premium]]
- [[models/market-maker-buy-model]]
