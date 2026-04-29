---
type: concept
aliases: [Consequent Encroachment, CE]
tags: [concept, pd-array, midpoint]
---

# Consequent Encroachment

Consequent encroachment is the 50% midpoint of a relevant range or candle body/wick structure. In ICT usage, it is the level price often revisits when the market is interacting with a range, a fair value gap, or another PD array.

## Core idea

The midpoint is not arbitrary:

- it is the mechanical half of the range,
- it often acts as the balance point inside a structure,
- and it can function as a decision reference for continuation, rejection, or failed acceptance.

## Why it matters

Consequent encroachment shows up repeatedly in session and delivery work:
- as the midpoint of an opening structure,
- as the midpoint of a dealing range,
- and as a practical target or reaction point during retracements.

The Trump-volatility NQ trade breakdown uses CE as the line that keeps a bullish daily discount-wick frame honest: bodies must stay in the upper half / around CE or the reclaim thesis weakens ([[sources/nq-trade-breakdown-reclaimed-ifvg-entry-with-trump-volatility-live-account-ict-concepts]]).
The "holding through the 9:30 open" NQ walkthrough makes the same level operational: once price closes back above CE / the IFVG midpoint, the trader reduces risk before the opening bell and lets the remainder work only if the market stays accepted above the midpoint ([[sources/nq-live-trade-walkthrough-holding-through-the-930-open-ict-concepts]]).
Lecture 3 of the 2024 mentorship adds a more literal gap-based use: CE is the midpoint of the new-day opening gap, and if the gap is small enough ICT will eyeball the upper/lower quadrants instead of over-annotating the chart ([[sources/2024-mentorship-lecture-3]]).

The 03/11/2026 lunch algorithmic-theory clip applies the same midpoint logic to yesterday's opening-range gap and to the lunch carry-forward setup, treating CE as the reference line that the next session can be measured against ([[sources/ict-2026-new-york-lunch-algorithmic-theory]] @ 11:01, @ 27:12).

The "Keys To Success In Troubled Markets" lecture leans on the same idea when it grades the daily structure and says the market is working in the lower half of the range; the lower-quadrant / midpoint logic is what lets the chart stay objective when price is chaotic ([[sources/2025-lecture-series-keys-to-success-in-troubled-markets-june-16-2025]] @ 6:04, @ 8:48, @ 15:20).

The 02/13/2025 Telegram execution makes the same CE idea practical: the first presented FVG is managed from its consequent encroachment, and the stop / re-entry logic stays anchored to that midpoint while the market tests the opening-range frame and PPI volatility unfolds ([[sources/nq-live-execution-using-analysis-i-shared-in-telegram-02132025]] @ 6:12, @ 10:06, @ 13:09, @ 14:43, @ 15:30).

The 02/23/2026 SMC lecture makes the CE test explicit on a Monday inside-day / discount-wick example: a close below CE generally favors continuation lower, while failure to close below CE keeps the market in high-resistance liquidity and defers the low ([[sources/ict-2026-smart-money-concepts-lecture-february-23-2026]] @ 13:00, @ 13:32). Later in the same clip ICT uses CE again as the body-vs-wick acceptance check for FVG work: wicks may probe through the midpoint, but bodies failing to reclaim the upper half preserve the directional thesis ([[sources/ict-2026-smart-money-concepts-lecture-february-23-2026]] @ 37:04, @ 37:21, @ 37:58, @ 43:43).

The 02/04/2025 Forex review uses the same midpoint logic on a weekly wick, and the 03/28/2025 weekly-option intro treats the same wick midpoint as the control line for a week-long high/low thesis ([[sources/2025-lecture-series-smc-forex-review-02042025]] @ 1:21, @ 2:26, @ 4:38; [[sources/2025-lecture-series-weekly-option-strategy-intro-03282025]] @ 2:26, @ 6:01, @ 10:25).

The 09/06/2024 OSOK execution and the 08/30/2024 Turtle Soup long both use CE as the daily FVG midpoint that keeps the larger swing map honest while the lower-time-frame sweep works itself out ([[sources/ict-nq-live-execution-september-6-2024-100k-osok]] @ 1:15, @ 3:34, @ 8:14; [[sources/nq-pm-session-turtle-soup-long-full-pull-august-30-2024]] @ 1:15, @ 3:34).

The 04/24/2026 futures review makes CE operational on the opening-range gap and the daily structure simultaneously: the 27,080 CE of the gap and the 27,063 pre-posted level are the decision zone for whether price accepts into the gap or rejects back toward the relative equal lows beneath. Bodies staying in the lower half after touching the midpoint, and bodies staying outside the midpoint by the low, are the two tape-reading confirmations that preserve the short thesis ([[sources/ict-2026-futures-review-april-24-2026]] @ opening setup, @ order-flow confirmation).

## Practical use

Use CE when you want to know whether price has merely touched a structure or actually accepted through its center.

## See also

- [[concepts/fair-value-gap]]
- [[concepts/order-block]]
- [[timing/opening-range]]
- [[timing/first-hour-dealing-range]]
- [[timing/9-am-crt]]
- [[sources/why-the-9-am-crt-model-could-change-your-life]]
- [[sources/ict-2026-1st-hour-dealing-range-march-28-2026]]
