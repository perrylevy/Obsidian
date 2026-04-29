---
type: concept
aliases: [Draw on Liquidity, DOL]
tags: [concept, liquidity, bias]
---

# Draw on Liquidity (DOL)

The **next liquidity pool the algorithm is reaching for** — where price wants to go.

Identifying the next most likely DOL is "the single most important skill" in ICT's framework ([[sources/2023-mentorship-silver-bullet]] @ 7:23, @ 7:48).

## Candidates

DOL candidates include ([[sources/2023-mentorship-silver-bullet]] @ 3:47–6:41):

- Previous day high / low (PDH / PDL)
- Previous session (London / NY) high / low
- Previous weekly high / low
- Current or old [[concepts/new-week-opening-gap|New Week Opening Gap (NWOG)]]
- [[concepts/optimal-trade-entry|OTE]] zones
- Inefficiencies / [[concepts/fair-value-gap|FVGs]] sitting above or below price
- Relative-equal highs / lows ([[sources/internal-external-liquidity]] @ 11:16)
- The premium/discount 50% midpoint of the daily range as a structural target for algorithmic delivery ([[sources/2022-ict-mentorship-episode-2]] @ 35:22)
- In NQ review clips, the current daily premium wick high / daily volume imbalance and the London sell-side pool are also repeated draws ([[sources/nq-review-april-30-2025]] @ 5:56, @ 6:42, [[sources/2025-lecture-series-nq-may-01-2025-review]] @ 5:56).
- In the Trump-volatility NQ trade breakdown, buy-side liquidity / relative-equal-high style objectives remain the target after the reclaimed IFVG and Judas swing sequence ([[sources/nq-trade-breakdown-reclaimed-ifvg-entry-with-trump-volatility-live-account-ict-concepts]]).

## Quality filters

- **Smoothness** — a too-clean swing high / quadruple top is a louder DOL signal than a ragged one ([[sources/nq-live-tape-reading-am-review]] @ 5:21, @ 7:03).
- **HTF alignment** — DOLs that line up with HTF FVGs / OBs are higher conviction ([[sources/internal-external-liquidity]] @ 10:47).
- **Low-resistance setup** — when the path to a DOL is unobstructed, expect a [[concepts/low-resistance-liquidity-run|LRLR]] into it.

## DOL ↔ bias

DOL is the operational form of **directional bias**. "Bias = bullish" means nothing actionable; "DOL = previous week high" tells you both direction and target.

The January 27, 2025 GBP/USD NWOG lecture is a clean live example of that logic: the weekly gap is the frame, the 10:00 Silver Bullet pocket is the timing filter, and the next liquidity draw is the sell-side target after the IFVG / CE confirmation holds ([[sources/2025-lecture-series-smc-new-york-nwog-with-forex-01272025]]).

Episode 34 of the 2022 mentorship gives the same DOL logic a weekly-gap twist: the Sunday gap can be extended through the week, can be left behind for a time, and then becomes the draw / reference that price returns to as support or resistance once the market revisits it ([[sources/2022-ict-mentorship-episode-34-using-the-sunday-gap-opening]]).

Lecture 3 of the 2024 mentorship adds the new-day variant: a clustered NDOG can become the larger draw on liquidity, with the morning relative equal highs/lows acting as the local sweep path on the way to that gap ([[sources/2024-mentorship-lecture-3]]).

The "$4,000 In 7 Minutes" PO3 walkthrough gives a practical low-hanging-fruit version of the same idea: the 2-day open, the daily open, and the 25% mark were the immediate draws the trader wanted price to deliver into after the morning manipulation completed ([[sources/4000-in-7-minutes-trading-my-ict-30m-po3-model]] @ 5:53, @ 8:45, @ 10:51, @ 17:44).

The 02/13/2025 Telegram execution gives a similar intraday draw map: once the morning buy-side liquidity is overhead, the market works back through the first presented FVG and opening-range structure before pushing toward the relative equal highs target ([[sources/nq-live-execution-using-analysis-i-shared-in-telegram-02132025]] @ 0:58, @ 1:17, @ 3:17, @ 4:01, @ 4:25, @ 8:28).

The 11/14/2025 general market commentary makes the same point operationally: keep the daily draw in view, because that context tells you whether the current tape is a tradable expansion or a gap-risk environment where short-term trading should be reduced rather than forced ([[sources/ict-general-market-commentary-november-14-2025]] @ 11:27, @ 11:59, @ 13:26).

The "From Vision To Execution" lecture adds the mental step: cast forth a vision of where price is likely to draw and how it gets there, then let the market prove that picture in the execution window. In that framing, DOL is not only a target; it is the path you are anticipating before the chart finishes telling the story ([[sources/from-vision-to-execution]]).

The "This Stupid Simple Strategy Works Everyday" clip uses DOL in the most stripped-down way possible: after the 5-minute inversion, the target is simply the next significant liquidity pool. That keeps the model low-R and prevents the trader from overcomplicating the draw with extra arrays or oversized expectations ([[sources/this-stupid-simple-strategy-works-everyday-stupid-simple-and-proven]]).

## See also

- [[concepts/liquidity]]
- [[concepts/low-resistance-liquidity-run]]
- [[concepts/buyside-liquidity]]
- [[concepts/sellside-liquidity]]
- [[concepts/relative-equal-highs-lows]]
- [[sources/950-macro-atm-model-ict-tape-read]]
- [[sources/live-atm-model-trade-ict-tape-read]]
- [[sources/old-daily-lows-breaker-entry-and-ifvg-reentry-after-profitable-stop-out]]
- [[models/internal-external-liquidity-model]]
