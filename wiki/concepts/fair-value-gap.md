---
type: concept
aliases: [FVG, Fair Value Gap]
tags: [concept, pd-array, price-action]
---

# Fair Value Gap (FVG)

## Definition

A **3-candle pattern** where the wick of candle 1 and the wick of candle 3 do not overlap, leaving an inefficiency between them ([[sources/how-to-trade-ifvg]] @ 0:18, [[sources/internal-external-liquidity]] @ 0:37, [[sources/2022-ict-mentorship-episode-2]] @ 30:05). The 2022 mentorship Episode 6 provides the most detailed early ICT-direct three-candle formation explanation: Candle 1 = reference high/low, Candle 2 = extended low/high, Candle 3 = continuation candle whose high/low doesn't reach Candle 1's low/high, leaving the gap where only one side of liquidity was offered ([[sources/2022-ict-mentorship-episode-6]]). Episode 7 demonstrates the FVG as the **intraday entry trigger within a daily bias framework**: once daily bias is established (bearish = target old low), the intraday liquidity sweep + MSS produces the FVG where the entry is taken, with stop below the FVG low ([[sources/2022-ict-mentorship-episode-7]]). Episode 8 applies the same FVG concept to **forex markets** (EUR/JPY example), showing the three-candle formation works identically across asset classes ([[sources/2022-ict-mentorship-episode-8]]). Episode 14 shows the same logic in a compact live long: after an upside MSS, ICT looks for a gap fill from Friday's close and uses the FVG as the limit-entry array while targeting buyside liquidity above the short-term highs ([[sources/2022-ict-mentorship-episode-14]]).

Episode 15 provides a live equity-account example of FVG entry under bullish bias: the 680 level FVG is the premium market support array, with a smaller 630 FVG in the last 3 candles as the minimum support level. The entry is taken into the 680 FVG with sell stops resting below the swing low (13,612) rather than a hard stop, allowing the trade to survive opening whipsaw ([[sources/2022-ict-mentorship-episode-15]]).

Episode 16 reaffirms the FVG as the clean imbalance that the market wants to return to, and notes that stacked FVGs should be read as one larger opportunity set, with the upper gap generally taking precedence ([[sources/2022-ict-mentorship-episode-16]]).

Episode 22 adds a compact imbalance example: the gap between candle low and opening price becomes the working trade window, with bodies staying inside the imbalance while wicks probe liquidity ([[sources/2022-ict-mentorship-episode-22]]).

Episode 35 turns the same idea into a live delivery lesson: repeated retracements into the working FVG are part of the compression phase before the expansion leg, and the market can treat the gap as the active intraday array while it builds higher lows toward the larger target ([[sources/2022-ict-mentorship-episode-35-order-block-and-smt-divergence]]).

Episode 36 adds the operational version: the FVG is the working entry/support-resistance array inside the intraday range, and the market can revisit it multiple times before the final expansion run ([[sources/2022-ict-mentorship-episode-36]]). Episode 37 keeps the same idea in a daily/breaker context: price works inside the FVG, then extends through the short-term high once the retracement array has done its job ([[sources/2022-ict-mentorship-episode-37]] @ 0:24, @ 0:31, @ 3:22, @ 7:18).

Classified by the middle candle's direction:

- **Bullish FVG** — middle candle up-closed. Also termed **BISI** (Buy Side Imbalance, Sell Side Inefficiency).
- **Bearish FVG** — middle candle down-closed. Also termed **SIBI** (Sell Side Imbalance, Buy Side Inefficiency). The gap runs between the low of candle 1 and the high of candle 3 ([[sources/2025-price-delivery-continuum]] @ 08:52).

## Status in ICT doctrine

FVG has "taken the throne from [[concepts/optimal-trade-entry|OTE]]" as ICT's flagship entry pattern ([[sources/2023-mentorship-silver-bullet]] @ 5:31). It is the entry trigger for the [[models/silver-bullet|Silver Bullet]] and appears across ICT's 2023–2025 material.

## Where and when FVGs form

- Inside a [[timing/silver-bullet-windows|Silver Bullet 60-minute window]], an FVG that forms becomes the entry trigger ([[sources/2023-mentorship-silver-bullet]] @ 9:38).
- Up to **four potential FVGs per hour** on the working timeframe — one per [[timing/quarters-of-the-hour|quarter of the hour]] (xx:00, xx:15, xx:30, xx:45) ([[sources/2025-price-delivery-continuum]] @ 19:09).
- If no FVGs are forming during a quarter, the market is in a [[concepts/high-resistance-liquidity-run|high-resistance]] state — sit still, wait the next quarter ([[sources/2025-price-delivery-continuum]] @ 21:01).

## Precision rules

- **Include [[concepts/volume-imbalance|volume imbalances]]** inside the range when drawing the FVG boundary ([[sources/mnq-pm-silver-bullet-walkthrough]] @ 0:36).
- **Upper half of a bearish FVG / lower half of a bullish FVG** must not be traded through; violation of this half is disqualifying. Study only that half for entry validity ([[sources/2025-price-delivery-continuum]] @ 15:51, @ 18:29, [[sources/mnq-pm-silver-bullet-walkthrough]] @ 0:58).
- **Bodies tell the story, wicks do the damage** — when price retraces into an FVG, watch whether bodies stay inside the gap ([[sources/2023-mentorship-silver-bullet]] @ 14:48).
- **[[concepts/consequent-encroachment|Consequent encroachment]] (CE)** = the midpoint of the FVG. A bullish FVG that is reclaimed but fails to be traded back down to its CE is the institutional-orderflow entry-drill signature ([[sources/2025-price-delivery-continuum]] @ 04:38, @ 06:36).
- On the NQ review clips, the **first presented FVG** after the 9:30 open is often literally the opening-range gap and the working array; the same rule repeats for the PM session around 1:30–2:00 and for news impulses like CPI once the market validates the move ([[sources/2025-lecture-series-nq-review-when-930am-et-is-1st-presented-fvg-may-18-2025]] @ 8:29, @ 12:46, @ 13:16, @ 43:05, [[sources/2025-lecture-series-nq-review-cpi-no-trade-may-13-2025]] @ 1:23, @ 3:51).
- **Quadrant-straddle qualifier** — a FVG is "smart-money grade" only when any part of its gap range overlaps a quadrant line of the [[concepts/pd-array|PD array matrix]]. A FVG floating entirely between two quadrant lines is "common grade" — 50/50 ([[sources/2025-pd-array-matrix]]).
- **News-driver TF rule** — on high-impact news days at 8:30 NY, only trust **5-minute or higher** FVGs at release. Wait 15–30 min before dropping to sub-5-minute timeframes; sub-5-min FVGs in the spike are unreliable ([[sources/2024-04-18-ob-tape-reading]] @ 14:09, @ 14:34, @ 32:57).

## Institutional-orderflow entry drill variant

One reclaimed-bullish-FVG variant now absorbed here is the **institutional orderflow entry drill**: price reclaims a bullish FVG, but then fails to trade back down to the gap's [[concepts/consequent-encroachment|CE]] on the next pass. In that framing, the key tell is not merely that the gap exists, but that price cannot retrace deeply enough to violate the active midpoint expectation ([[sources/2025-price-delivery-continuum]] @ 04:38, @ 06:36, [[sources/2024-mentorship-lecture-12]]).

## FVG lifecycle

- **Fresh / unmitigated** — not yet revisited. Highest-quality draw.
- **Mitigated** — price has traded into it. One framing argues mitigated FVGs should be deleted from the chart; subsequent reactions come off the swing point left behind, not the FVG ([[sources/how-to-trade-turtle-soups]] @ 16:37, @ 17:52). _Attribution: Arjo / MMC._
- **Reclaimed** — a bullish FVG that failed first-visit but was later retaken can act as support again on the next revisit ([[sources/mnq-pm-silver-bullet-walkthrough]] @ 22:25).
- **Inverted** — violated and closed through swiftly; polarity flips and it becomes an [[concepts/inversion-fair-value-gap|IFVG]] ([[sources/how-to-trade-ifvg]] @ 0:38).

## FVG as a draw on liquidity

FVGs sitting above or below current price can themselves act as the [[concepts/draw-on-liquidity|draw on liquidity]] — where price wants to go ([[sources/2023-mentorship-silver-bullet]] @ 5:55, @ 6:14).

The "Keys To Success In Troubled Markets" lecture treats a daily FVG / inefficiency pocket as exactly that kind of reference: a large hole in the chart that can remain a target or a warning depending on whether price has already traded through its lower-half structure ([[sources/2025-lecture-series-keys-to-success-in-troubled-markets-june-16-2025]] @ 2:10, @ 6:04, @ 16:17).

The breaker-block continuation clip treats an FVG as the fallback when a textbook breaker does not fully form: if the swing has already been swept and price trades back into the gap, the continuation can still be framed through the FVG pocket and the intermediate-term swing that created it ([[sources/trade-continuations-using-breaker-blocks]]).

The 02/13/2025 Telegram execution uses the same idea one step lower: the first presented FVG after the PPI move becomes the working array, and the trader is willing to hold only if the bodies stay in the right half of that gap while price works toward the higher-level buy-side target ([[sources/nq-live-execution-using-analysis-i-shared-in-telegram-02132025]] @ 6:12, @ 9:03, @ 10:06, @ 11:26, @ 14:43, @ 16:55).
The 06/02/2025 and 06/05/2025 storyteller clips show the same thing as a live carry-forward stack: the prior daily inefficiency stays live, the 15-minute FVGs become the working canvas, and the opening-range / first-presented FVG only matters when it aligns with that parent structure ([[sources/2025-storytellers-series-nq-review-june-02-2025]] @ 2:33, @ 5:41, @ 7:31, @ 12:44; [[sources/2025-storytellers-series-nq-futures-june-05-2025]] @ 1:08, @ 5:17, @ 12:44, @ 16:11).

The "This Stupid Simple Strategy Works Everyday" clip uses the same FVG idea as a deliberately sparse scaffold: first tap a higher-time-frame FVG, then wait for a 5-minute FVG to open, and only then look for the inversion. The lesson is to let one HTF gap and one LTF gap do the work instead of stacking more and more arrays ([[sources/this-stupid-simple-strategy-works-everyday-stupid-simple-and-proven]]).

## Stacked FVGs

Adjacent FVGs should be **aggregated and treated as one larger FVG** for inversion / closure purposes ([[sources/how-to-trade-ifvg]] @ 5:08, @ 10:02).

## Multiple FVG strategy

The 2022 mentorship Episode 3 provides the earliest ICT-direct formulation of the multiple-FVG handling rule: when two fair value gaps exist (one lower, one higher), sacrifice the better entry at the lower FVG and wait for price to trade into it and return to the higher FVG. Enter when price accumulates in the higher FVG, expecting the lower FVG won't be retested ([[sources/2022-ict-mentorship-episode-3]]). This is an early formulation of what later becomes the "stacked FVG" handling rule — both are valid; Episode 3 provides the foundational logic.

## Special cases now absorbed here

- **Stacked FVGs** are not treated as a separate top-level doctrine page in this wiki. They are a handling rule inside the broader FVG family: adjacent gaps should be aggregated and read as one larger imbalance when judging inversion, closure, or continuation ([[sources/how-to-trade-ifvg]] @ 5:08, @ 10:02).
- **Reclaimed bullish FVG** is also treated as an FVG lifecycle state rather than a separate doctrine page: a bullish gap can fail on first contact, later be reclaimed, and then behave again as support on the next revisit ([[sources/mnq-pm-silver-bullet-walkthrough]] @ 22:25).

## HTF parent rule

HTF FVGs are "parent" to LTF FVGs — stronger and more important. When an LTF FVG is overlapped, a parent HTF FVG's midpoint can still hold price ([[sources/mnq-pm-silver-bullet-walkthrough]] @ 15:22).

## Nuance & cross-source notes

- **IRL ≡ FVG — multi-source consensus among derivative teachers.** [[sources/internal-external-liquidity|TTrades]] (@ 0:37) and [[sources/game-changer-irl-erl|The MMXM Trader]] (@ 1:32) both equate **internal range liquidity** with FVG as a primitive — independently, with no apparent cross-influence. Neither teacher mentions OBs, breaker blocks, or other PD arrays as IRL components. This appears to be the standard derivative-teacher reading, **not** a TTrades idiosyncrasy. Still pending: ICT-direct confirmation of the strict equivalence (the foundational ICT framing treats IRL more broadly).
- **Algorithm does not forget** — even after an FVG is filled / closed in, the level remains tracked by the algorithmic delivery ([[sources/2025-price-delivery-continuum]] @ 04:18).

## See also

- [[concepts/inversion-fair-value-gap]]
- [[concepts/consequent-encroachment]]
- [[concepts/balanced-price-range]]
- [[concepts/order-block]]
- [[concepts/pd-array]]
- [[concepts/liquidity]]
- [[models/silver-bullet]]
- [[timing/quarters-of-the-hour]]
- [[timing/first-presented-fvg]]
