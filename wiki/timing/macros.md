---
type: timing
aliases: [Macros, ICT Macros, Macro Windows]
tags: [timing]
---

# Macros

Short, time-anchored windows (~10–20 min) inside which the algorithm reliably reprices toward a [[concepts/pd-array|PD array]] / [[concepts/draw-on-liquidity|DOL]]. Macros are the time component of the **time + price agreement** rule from the [[concepts/pd-array|PD array matrix]] ([[sources/2025-pd-array-matrix]]).

## Macros referenced in ingested sources

|| Window (NY time) | Context | Source |
||---|---|---|
|| 2:00–3:00 | PM session best setup window; after lunch consolidation (noon–1:00 PM), the 2:00 PM onward window offers cleaner setups, especially when morning session was invalidated by overnight run; Episode 9 demonstrates the full PM session execution: relative equal lows → liquidity sweep → MSS → FVG entry at 2:34 PM with 3.5:1 risk/reward ([[sources/2022-ict-mentorship-episode-9]])
|| 2:50–3:10 | PM macro shown driving FVG respect | [[sources/2025-pd-array-matrix]], [[sources/mnq-pm-silver-bullet-walkthrough]] @ 3:01 |
|| 9:50–10:10 | opening / news macro; target window for IFVG or opening-range continuation | [[sources/nq-live-tape-reading-am-review]] @ 11:09, [[sources/nq-futures-review-04012025]] @ 7:02, [[sources/2025-lecture-series-ict-gauntlet-nq-am-session-may-07-2025-review]] @ 21:14, [[sources/2025-lecture-series-nq-nfp-algorithmic-price-delivery-04042025]] @ 1:22, [[sources/950-macro-atm-model-ict-tape-read]], [[sources/live-atm-model-trade-ict-tape-read]]
|| 8:30–8:40 | employment-data / morning spooling checkpoint; stacked NDOG / NWOG side tends to matter more; high-impact release days like NFP and news releases are structure-first, not prediction-first; Episode 6 demonstrates the 8:30 employment data release as a live NQ example where displacement creates the morning's directional thesis ([[sources/2022-ict-mentorship-episode-6]]); Episode 10 adds the **economic calendar awareness** context: forexfactory.com color coding (red=high impact), 8:30 AM ET news embargo, and the predictable price buildup/breakdown patterns around high-impact events | [[sources/2024-mentorship-lecture-4]], [[sources/ict-2024-mentorship-october-nfp-nq-october-04-2024]], [[sources/ict-2024-mentorship-news-release-tape-reading-october-17-2024]], [[sources/2022-ict-mentorship-episode-10]]
|| 9:30–10:00 | opening range; first presented FVG after open/news; 30-minute opening range probes buy side then sell side before the real move; Episode 7 notes the 9:30 open is characteristically sloppy and recommends **leader trades** (small single-contract entries) to gather intel before scaling in | [[sources/nq-futures-review-04012025]] @ 5:50, @ 6:21, [[sources/2025-lecture-series-nq-may-01-2025-review]] @ 19:52, [[sources/2025-lecture-series-nq-review-when-930am-et-is-1st-presented-fvg-may-18-2025]] @ 8:29, @ 47:42, [[sources/2025-lecture-series-algorithmic-timing-and-journaling-03222025]] @ 42:01, @ 43:38, @ 48:46, [[sources/2024-mentorship-lecture-1]] @ 1:51:44–1:52:32, [[sources/ict-2026-smart-money-concepts-lecture-february-23-2026]] @ 19:13, [[sources/2022-ict-mentorship-episode-7]]
|| 10:50–11:10 | late-morning continuation / objective window after opening validation | [[sources/ict-2026-market-commentary-march-10-2026]] @ 26:36, [[sources/2025-lecture-series-nq-nfp-algorithmic-price-delivery-04042025]] @ 1:39, @ 10:51 |
||| 1:30–2:00 | PM session first presented FVG / afternoon opening range; 1:30 PM is when macro algorithms activate for the afternoon session per the 2022 mentorship ([[sources/2022-ict-mentorship-episode-5]]) | [[sources/2025-lecture-series-nq-review-when-930am-et-is-1st-presented-fvg-may-18-2025]] @ 12:01, @ 43:48, [[sources/2025-lecture-series-algorithmic-timing-and-journaling-03222025]] @ 1:15:31 |
|| 11:30–1:30 | [[timing/lunch-macro]]; mid-day continuation / lunch-hour shift; in bullish mornings, 11:30 often raids the first low formed after 10:00 before trend resumption; the 04/14/2026 review adds that the lunch macro can begin as early as 10:30 once the 9:30–10:30 first-hour dealing range is complete, and the 03/11/2026 lunch-theory clip adds the carry-forward rule for the inefficiency immediately before the raid; the 03/28/2026 first-hour lesson adds the 10:30–11:30 sweet spot and the projected lower-copy / first-presented-FVG handoff once the range breaks | [[sources/2025-lecture-series-algorithmic-timing-and-journaling-03222025]] @ 58:57, [[sources/2024-mentorship-lecture-12]], [[sources/ict-2026-new-york-lunch-algorithmic-theory]] @ 10:08, @ 27:12, [[sources/ict-2026-futures-review-april-14-2026]] @ 4:37, @ 4:50, @ 5:16, @ 6:08, @ 27:44, [[sources/ict-2026-1st-hour-dealing-range-march-28-2026]] @ 45:37, @ 46:53, @ 50:14, @ 1:10:05, @ 1:12:46, @ 1:14:13 |
|| 3:15–3:45 | last-hour macro; run on unengaged liquidity / final-hour continuation, but can also produce the pullback off the high before market-on-close takes over | [[sources/nq-futures-review-04012025]] @ 12:13, [[sources/nq-nfp-algorithmic-price-delivery-04042025]] @ 3:39, [[sources/ict-explains-how-to-trade-last-hour-macro]] @ 0:00–15:17, [[sources/this-was-my-largest-trade-ever-nq-live-trade-walkthrough-final-hour-macro-ict-concepts]] @ 0:05–10:17, [[sources/2024-mentorship-lecture-12]] |
||| 3:45–4:00 | market-on-close macro; final rip into sellside liquidity / late-session target delivery; 3:50–4:00 PM is the close algorithm acceleration per the 2022 mentorship ([[sources/2022-ict-mentorship-episode-5]]) | [[sources/smc-algorithmic-market-on-close-macro]] @ 28:32, @ 29:23, [[sources/2024-mentorship-lecture-12]] |


The 05/07/2025 ICT Gauntlet review is the cleanest liquidity-first open-to-10:10 example in the vault: ICT explicitly says the 7:00–9:30 ET window is the liquidity map, treats the 9:30 open as a likely draw back into the gap or toward the first relative equal highs, and then uses the 9:50–10:10 macro on the 15-second chart to confirm the move ([[sources/2025-lecture-series-ict-gauntlet-nq-am-session-may-07-2025-review]] @ 6:23, @ 8:06, @ 9:38, @ 11:30, @ 11:40, @ 21:14).

The 04/04/2025 NFP delivery review adds the sharper open-to-11 cadence: the 9:30 open and first presented FVG are the working array, the 10:00 release is a volatility driver rather than a new bias, the 9:50–10:10 macro handles the first drive, and the 10:50–11:10 macro becomes the late-morning continuation / objective window once the opening narrative validates. The 10/04/2024 NFP lecture and the 10/17/2024 news-release tape say the same thing in plainer language: wait for the release, let the first impulse print, and then decide which side actually survived ([[sources/2025-lecture-series-nq-nfp-algorithmic-price-delivery-04042025]] @ 0:33, @ 1:04, @ 1:22, @ 1:39, @ 7:55, @ 9:04, @ 10:51, [[sources/ict-2024-mentorship-october-nfp-nq-october-04-2024]] @ 5:47, @ 6:24, @ 12:57, @ 17:13, [[sources/ict-2024-mentorship-news-release-tape-reading-october-17-2024]] @ 2:27, @ 9:00, @ 10:52, @ 17:13).

The "From Vision To Execution" lecture uses the same 9:50–10:10 window as the confirmation zone after a turtle-soup style sweep and displacement, so the macro is not just a time slot; it is the place where the drawn-to level is supposed to prove itself ([[sources/from-vision-to-execution]]).

The 03/10/2026 market commentary adds a direct open-to-10:10 read: the 9:30 print above prior settlement makes the ORG premium, the 7-minute-after-10 candle becomes the sellside litmus test, and the same morning can still revisit its 10:50–11:10 objective once the opening narrative is validated ([[sources/ict-2026-market-commentary-march-10-2026]] @ 10:02, @ 13:19, @ 18:34–19:06, @ 23:33–23:54, @ 26:36).

The 01/22/2025 GBPUSD London macro shows the same time + price agreement in FX: the 2:50–3:10 window, reclaimed bullish FVG, and immediate rebalance can still produce a clean run when the body stays above consequent encroachment ([[sources/gbpusd-london-macro-live-execution-2025-01-22]] @ 0:40, @ 2:04, @ 2:55, @ 6:14, @ 7:51).

One broad time-and-price lecture frames the whole day as a session-range ladder: the previous-day 1:30–4:00 PM range, the 2:00–5:00 AM London range, the 9:30 AM–noon AM session / opening-range-gap frame, and then the lunch pulse that often revisits the morning low before continuation. It is a clean reminder that macros are nested inside larger session windows ([[sources/understanding-time-price-the-only-thing-you-need]]).

The 01/13/2026 lecture adds that the pre-9:30 tape can sit in time distortion/compression and that 10:00–11:00 is the first profit-taking / offboard window after the open, especially if you are long from the premarket or opening-thrust sequence ([[sources/ict-2026-smart-money-concepts-lecture-january-13-2026]] @ 2:19, @ 4:00, @ 17:17, @ 25:39).

The April 29, 2024 bias lecture adds a useful framing rule for macro selection: if the tape is not aligned, do not force a daily bias just because a time window is open. The calendar and the event week itself are part of the manipulation map, so the macro only matters when seasonal / structural context has already narrowed the likely draw ([[sources/how-to-read-price-with-or-without-a-bias-april-29-2024]] @ 26:52, @ 27:52, @ 1:01:19–1:02:02).

Many other macros exist in ICT material (e.g. 11:50–12:10, 1:50–2:10) but are **not** in the currently-ingested clippings.

## Why macros matter

Without time alignment, a high-quality PD array at a quadrant is **not actionable** — the algorithm only reprices into / out of it during a macro or session open ([[sources/2025-pd-array-matrix]]). PD array selection (price) and macro window (time) must agree.

## Macros vs killzones

- [[deferred/timing/killzones|Killzones]] are **multi-hour** session windows (London / NY AM / NY PM).
- Macros are **~20-minute pulses** inside or adjacent to those sessions.

A killzone defines the broad opportunity set; a macro defines the precise execution window inside it.

## News-driver caveat

On high-impact news days at 8:30 NY, do not use sub-5-minute charts for 15 min (ICT minimum) to 30 min (recommended). Sub-5-min FVGs around the spike are "spottiness" — unreliable ([[sources/2024-04-18-ob-tape-reading]] @ 14:34, @ 32:57). The 10/17/2024 news-release tape and 10/04/2024 NFP lecture reinforce the same release-day rule: let the first impulse happen, then reassess structure instead of trying to front-run the number. The 8:30–9:30 window is expected "time distortion" — price marks time in a range while waiting for the open ([[sources/2024-04-18-ob-tape-reading]] @ 1:46:10). Wait for the 9:30 open to define a fresh dealing range.

The 04/29/2024 bias lecture makes the same warning from a preparation angle: red- and orange-folder weeks are a "minefield," and ICT explicitly does not force a daily bias on FOMC / NFP weeks. He instead treats the calendar as a manipulation map and waits to see whether the early move is only a trap before the real directional leg ([[sources/how-to-read-price-with-or-without-a-bias-april-29-2024]] @ 26:52–29:59, @ 31:39–32:24, @ 1:01:19–1:02:02).

The 09/06/2024 NFP lecture sharpens the same macro rule into a practical bellwether workflow: map the 15-minute highs/lows, let the initial shock print, and only then decide which side survived ([[sources/nonfarm-payroll-september-06-2024]] @ 8:22, @ 8:51, @ 9:23, @ 11:52, @ 22:33).

## See also

- [[deferred/timing/killzones]]
- [[timing/silver-bullet-windows]]
- [[timing/lunch-macro]]
- [[timing/quarters-of-the-hour]]
- [[timing/new-york-local-time]]
- [[timing/first-presented-fvg]]
- [[timing/time-distortion]]
- [[concepts/pd-array]]

