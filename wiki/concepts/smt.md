---
type: concept
aliases: [SMT, SMT Divergence, Smart Money Tool, Smart Money Technique]
tags: [concept, structure, confluence]
---

# SMT (Smart Money Tool / Divergence)

A divergence between two correlated instruments where one makes a higher high / lower low and the other does **not**. The non-confirming leg is the algorithmic tell.

ICT framing: SMT = **Smart Money Tool**, not "Smart Money Technique" as commonly relayed ([[sources/intro-smt-divergence]]).

## Index-futures triad

The three correlated US index futures used for SMT:

- **ES** (E-mini S&P 500)
- **NQ** (E-mini Nasdaq)
- **YM** (E-mini Dow)

When two of the three sweep a swing point and the third refuses, the third is the divergent leg ([[sources/intro-smt-divergence]]).

## Trade-side rule for MNQ / NQ

When trading [[instruments/MNQ|MNQ]] / [[instruments/NQ|NQ]], **enter on the divergent leg** of the trio:

- If NQ is the leg that fails to confirm a sellside sweep (refuses to make the new low) → NQ is the **preferred long entry instrument** vs ES or YM.
- If NQ is the one that **does** confirm and ES/YM diverge → defer; ES/YM is the better entry ([[sources/intro-smt-divergence]]).

This is the most direct MNQ-trading consequence of SMT. _Attribution: Fearing — derivative teacher relaying ICT material._

## Use as confluence

SMT layered into IFVG / FVG entries: divergence between candle 1's high (or candle 2's high) on one instrument vs the other strengthens the inversion / sweep signature ([[sources/how-to-trade-ifvg]] @ 2:15, @ 12:13).

The "$4,000 In 7 Minutes" trade adds a classic triad example: ES and Q traded above the previous-day high while YM did not, then a lower-time-frame SMT formed again on the 1-minute sequence before the short was validated ([[sources/4000-in-7-minutes-trading-my-ict-30m-po3-model]] @ 14:27, @ 14:45, @ 15:12).

The breaker-block continuation clip adds a stop-placement nuance: if the sweep is paired with SMT, the unbroken swing can be treated as protected and the breaker retest can still be used for continuation instead of waiting for a textbook sweep in the local market ([[sources/trade-continuations-using-breaker-blocks]]).

The "Forever Model" clip uses SMT as optional A++ confirmation inside a larger manipulation / IFVG / CISD sequence, making it additive rather than mandatory when the higher-time-frame draw is already obvious ([[sources/my-forever-model-the-strategy-that-has-made-me-over-half-a-million-insane-value]]).

The 04/26/2025 protected-highs-and-lows lesson adds a stop-placement use case: if the swing carries a valid time-based SMT, it can become the protected high or low that justifies putting the stop beyond the swing instead of at the obvious wick ([[sources/stop-getting-stopped-out-with-this-simple-concept-protected-highs-lows]]).

Episode 22 gives the clean intermarket example: ES fails to match NQ's overnight high, then the afternoon sequence repeats the same divergence logic against the daily bearish read ([[sources/2022-ict-mentorship-episode-22]]).

Episode 35 sharpens the same rule: NQ can make the lower low while ES refuses to confirm the low, and the divergence is only meaningful when the bias is already known and you know what price is reaching for ([[sources/2022-ict-mentorship-episode-35-order-block-and-smt-divergence]]).

A useful open-session variant is the "Beesting at Open" model: treat pre-open SMTs as unreliable, wait for the RTH open, then use the post-open SMT only when it is aligned with the higher-time-frame narrative and the change-in-state-of-delivery trigger ([[synthesis/how-to-trade-the-beesting-at-open-model]], [[sources/this-ict-model-will-change-your-trading-forever-smt-cisd-time]], [[sources/this-ict-model-will-make-you-profitable-forever-stop-paying-for-mentorships-beesting-open-vid-2]]).

## See also

- [[concepts/inversion-fair-value-gap]]
- [[concepts/liquidity-sweep]]
- [[instruments/MNQ]]
- [[instruments/NQ]]
