---
type: timing
aliases: [First Presented FVG, Opening Range FVG]
tags: [timing, fair-value-gap]
---

# First Presented FVG

The **first presented FVG** is the first 1-minute fair value gap that appears inside the active session window the trader is working from. In the May 18 ICT review, the flagship case is the **9:30–10:00 AM opening range**: the first usable 1-minute FVG after 9:30 becomes the working array for the morning session ([[sources/2025-lecture-series-nq-review-when-930am-et-is-1st-presented-fvg-may-18-2025]] @ 8:29, @ 9:12, @ 47:42). The ICT opening-range lecture later restates the same idea from the London side of the day ([[sources/ict-opening-range-theory-1st-presented-fvg-logic]]).

The 03/27/2026 market commentary gives a live NQ example of the same rule: once the 9:30 open is in place, the first valid 1-minute FVG becomes the first presented FVG and the opening-range gap / consequent encroachment stay tied to that same morning frame ([[sources/ict-2026-market-commentary-march-27-2026]]).

The 03/09/2026 market commentary adds a premium-open variant: the 9:30 print above prior settlement still keeps the first presented FVG anchored to the opening sequence, but ICT is explicit that the 7-minute-after-10 candle tells you whether sellside is actually the draw or whether the open is still just noise ([[sources/ict-2026-market-commentary-march-09-2026]] @ 10:02, @ 32:26, @ 36:43).

The 03/08/2026 market commentary sharpens the same AM logic from the other side of the frame: once the RTH opening-range gap is established, ICT treats the first valid 1-minute FVG inside that window as the morning's working array and keeps ETH only as context around the RTH anchor ([[sources/ict-2026-market-commentary-march-08-2026]] @ 10:02, @ 13:19–13:43, @ 15:30, @ 17:29–18:26).

The 10/01/2025 NQ market review adds a layered live example: the opening-range-gap is read together with premium wick levels, a 9:31 first-presented FVG, inversion FVGs, and relative equal highs so the session can be handled as one integrated map rather than as isolated patterns ([[sources/ict-nq-futures-market-review-october-1-2025]] @ 0:44, @ 1:34, @ 4:20, @ 5:09, @ 5:45, @ 12:58, @ 13:08).
The May 12, 2025 Venom example is the bullish deferred-entry version of the same opening logic: after a sellside raid below the opening low, ICT wants the opening-price-or-lower buy and then lets the first presented FVG / inversion FVG validate the turn ([[sources/2025-lecture-series-ict-venom-example-may-12-2025]]).
The "NQ May 01, 2025 Review" clip gives a direct live example: the morning opening-range first-presented FVG is used only after the 10:00 news pulse validates the inversion, not before ([[sources/2025-lecture-series-nq-may-01-2025-review]] @ 5:35, @ 7:24, @ 9:04).
The 06/02/2025 and 06/05/2025 NQ reviews keep the same pattern alive in live tape: the first valid morning 1-minute FVG is only useful when it agrees with the prior daily inefficiency, the opening-range gap, and the carried-forward 15-minute canvas ([[sources/2025-storytellers-series-nq-review-june-02-2025]] @ 12:44, @ 15:00; [[sources/2025-storytellers-series-nq-futures-june-05-2025]] @ 12:44, @ 15:00).
- The 01/13/2026 lecture broadens the same logic backward into the premarket lead-in: ICT treats the 7:00–9:30 window as the build-up to the open, then hands off to the 9:30 RTH opening-range probe once the session opens ([[sources/ict-2026-smart-money-concepts-lecture-january-13-2026]] @ 17:17, @ 18:17, @ 19:13, @ 25:39).
- A derivative scalping example from 2026 reinforces the same patience rule from the other side of the tape: wait through the first noisy part of the session, often until 9:45–9:50, then use the first meaningful FVG after the open with the correct swing high/low context instead of trying to scalp every early fluctuation ([[sources/this-very-simple-fvg-scalping-strategy-is-all-you-need-to-be-profitable-in-2026]] @ 11:32, @ 12:00, @ 20:17).

## Working rule

- At the 9:30 open, use the **very first valid 1-minute FVG between 9:31 and 10:00 ET** as the primary morning array ([[sources/2025-lecture-series-nq-review-when-930am-et-is-1st-presented-fvg-may-18-2025]] @ 8:29, @ 47:42; [[sources/2025-lecture-series-algorithmic-timing-and-journaling-03222025]] @ 42:01, @ 43:38, @ 48:46).
- Lecture 16 of the 2024 mentorship sharpens the session filter: the 9:30 candle itself does not qualify, so the first-presented FVG must be the first valid RTH imbalance that still survives a regular-trading-hours view, which in practice means 9:31 or later ([[sources/2024-mentorship-lecture-16]] @ 38:01, @ 38:22, @ 38:38, @ 38:55).
- The 09/27/2024 high-resistance-liquidity lecture says the 9:30 candle is still useful for context, but the model should wait for the 9:31 candle before seeking the FVG, and it frames the opening-range gap as the active morning reference ([[sources/ict-2024-mentorship-how-to-identify-high-resistance-liquidity-conditions-september-27-2024]] @ 7:11, @ 7:36, @ 8:31, @ 12:46).
- In the PM session, the same logic repeats inside the **1:30–2:00 ET** opening window, where the PM session gets its own first presented FVG ([[sources/2025-lecture-series-nq-review-when-930am-et-is-1st-presented-fvg-may-18-2025]] @ 12:01, @ 43:48; [[sources/2025-lecture-series-algorithmic-timing-and-journaling-03222025]] @ 1:15:31).
- On news or impulse days, the first presented FVG after the driver move can replace an earlier idea, but only if price validates it rather than immediately violating it. If the validation is weak, stand down rather than forcing the move ([[sources/2025-lecture-series-nq-review-cpi-no-trade-may-13-2025]] @ 1:23, @ 3:51).
- The 04/04/2025 NFP delivery review is the clean open-to-news case: the 9:30 open’s first presented FVG remains the working array through the 10:00 release, and the 10:50–11:10 window becomes the later-morning continuation objective once the array validates ([[sources/2025-lecture-series-nq-nfp-algorithmic-price-delivery-04042025]] @ 0:33, @ 1:04, @ 1:22, @ 1:39, @ 7:55, @ 9:04, @ 10:51).

## Relationship to the opening-range gap

In the May 18 review, the first presented FVG is not just "another FVG." It is explicitly blended with the [[concepts/opening-range-gap|opening-range gap]] measured from prior settlement to the new regular-trading-hours open. ICT treats the opening-range gap and the first presented FVG as the same operational frame, then measures the consequent encroachment of that opening gap as the expected pullback target ([[sources/2025-lecture-series-nq-review-when-930am-et-is-1st-presented-fvg-may-18-2025]] @ 10:06, @ 12:46, @ 13:16, @ 14:03). The February 03, 2025 Monday review extends that same reclaim logic into a new-week-opening-gap plus opening-range-gap overlap, where the first valid 1-minute FVG after the open becomes the trigger inside the merged scaffold ([[sources/2025-lecture-review-february-03-2025]] @ 0:44–3:31).

## RTH and ETH nuance

The setup is clearest when regular trading hours and electronic trading hours are both understood together. The review treats RTH as the true opening structure while still incorporating overnight liquidity from Asia, London, and premarket as the pools price may reach for ([[sources/2025-lecture-series-nq-review-when-930am-et-is-1st-presented-fvg-may-18-2025]] @ 9:42, @ 10:39, @ 18:42, @ 19:18).

The 03/11/2026 lunch algorithmic-theory clip repeats the same logic in a midday carry-forward form: the first fair value gap immediately before the lunch liquidity raid becomes the reference carried into the next day ([[sources/ict-2026-new-york-lunch-algorithmic-theory]] @ 10:08, @ 27:12).

## Why it matters

The first presented FVG reduces chart clutter and narrows attention to the session’s first true displacement. Later FVGs may still matter, but they are secondary unless the first one has already been mitigated, flipped, or clearly lost relevance. The point is not to plot every FVG; it is to identify the session's first trustworthy one and let that anchor the setup ([[sources/2025-lecture-series-nq-review-when-930am-et-is-1st-presented-fvg-may-18-2025]] @ 20:46, @ 21:19, @ 43:48, @ 48:11).

The "From Vision To Execution" lecture sharpens the post-sweep variant: after a turtle-soup selloff or sellside raid, the first presented FVG becomes the standout array to project forward. The level can stay relevant for many sessions because you are not just marking a gap; you are marking the first clear displacement that proves the draw is active ([[sources/from-vision-to-execution]]).

## Monday carry-forward variant

The **Monday first presented FVG** is treated here as a specialized carry-forward use case rather than its own top-level concept page. Under the PD-array-matrix framing, Monday's first valid presented FVG can stay on the chart as a high-priority reference during the active 20-day look-back cycle, especially when price later starts using it as a draw on liquidity ([[sources/2025-pd-array-matrix]] @ 11:30–15:30, @ 24:02–25:15, @ 38:09–38:34, @ 2:12:32–2:17:01).

## See also

- [[concepts/fair-value-gap]]
- [[timing/macros]]
- [[concepts/new-day-opening-gap]]
- [[concepts/new-week-opening-gap]]
- [[concepts/consequent-encroachment]]
- [[instruments/NQ]]
- [[sources/ict-opening-range-theory-1st-presented-fvg-logic]]
- [[sources/ict-the-first-presented-fvg-in-the-opening-range]]
- [[sources/nq-futures-review-04012025]]
- [[timing/first-presented-fvg]] — Monday carry-forward PFVG use case
- [[sources/nq-trade-breakdown-how-to-pick-the-right-first-presented-fvg-ict-concepts]] — first-presented FVG selection and opening-price filter example
- [[timing/time-distortion]]
