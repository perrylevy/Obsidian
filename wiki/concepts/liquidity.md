---
type: concept
aliases: [Liquidity]
tags: [concept, liquidity, hub]
---

# Liquidity

In ICT, liquidity is **clustered stop orders** — the fuel algorithmic price delivery seeks to consume before making its intended move.

> "Liquidity = swing points; a swing high and a swing low are both liquidity because breakout buy-stops and protective stop-losses cluster there." ([[sources/how-to-trade-turtle-soups]] @ 3:00, @ 3:17, [[sources/2022-ict-mentorship-episode-2]] @ 18:22).

## Two meta-categories (ERL / IRL)

- **External Range Liquidity (ERL)** — swing highs and swing lows. Visible structure where breakout stops and opposing stop-losses rest ([[sources/internal-external-liquidity]] @ 0:58, @ 1:17).
- **Internal Range Liquidity (IRL)** — inefficiencies inside the range. Two derivative teachers independently equate IRL with [[concepts/fair-value-gap|FVG]] as its primitive: [[sources/internal-external-liquidity|TTrades]] (@ 0:37) and [[sources/game-changer-irl-erl|The MMXM Trader]] (@ 1:32). Multi-source consensus among derivative teachers; ICT-direct confirmation still pending — see [[concepts/fair-value-gap#Nuance & cross-source notes|FVG cross-source notes]].

Price rotates **external → internal → external** — the [[models/internal-external-liquidity-model|Internal-External Liquidity Model]] trades these legs ([[sources/internal-external-liquidity]] @ 1:28).

## Delivery heuristic

The algorithm's two recurring jobs are to raid liquidity and to rebalance inefficiency. When a liquidity pool sits in close proximity to an inefficiency, price often targets both in one move rather than treating them as separate destinations ([[sources/algorithmic-price-delivery-live-recorded-lesson]] @ 0:28, @ 2:47, @ 4:08).

The 11/14/2025 general market commentary says the same thing more bluntly: liquidity is the lifeblood of the marketplace, and supply/demand or classical support/resistance are secondary labels to the real stop-order pools ([[sources/ict-general-market-commentary-november-14-2025]] @ 28:56, @ 29:48).

An [[concepts/immediate-rebalance|immediate rebalance]] is the fast-path version of this behavior: price snaps to the booked level with little or no intermediate discovery, and the move should be treated as a sharp delivery event rather than a slow revisit.

Episode 36 keeps the focus on the same target logic: the morning high is the obvious buyside objective early in the session, then the final run clears sell-side liquidity after price has rotated through premium/discount and consolidated ([[sources/2022-ict-mentorship-episode-36]]). Episode 37 repeats the same logic with a short-term high target, warns that NFP week can be too choppy for normal execution, and ends with a stop-run example that clears the old high after the market has already advertised the target side ([[sources/2022-ict-mentorship-episode-37]] @ 0:43, @ 1:44, @ 4:09, @ 7:18, @ 23:09).

The "This Stupid Simple Strategy Works Everyday" clip keeps the target logic equally simple: once the 5-minute inversion prints, the trade is aimed at the next significant liquidity pool instead of trying to squeeze extra R out of the setup. The whole point is to keep the model low-R, repeatable, and easy to execute ([[sources/this-stupid-simple-strategy-works-everyday-stupid-simple-and-proven]]).

## Sub-types under ERL

- **[[concepts/buyside-liquidity|Buyside liquidity]]** — resting buy-stops above swing highs: breakout buys + short stop-losses ([[sources/internal-external-liquidity]] @ 1:17, [[sources/how-to-trade-turtle-soups]] @ 3:17, @ 6:08).
- **[[concepts/sellside-liquidity|Sellside liquidity]]** — resting sell-stops below swing lows: breakout sells + long stop-losses ([[sources/how-to-trade-turtle-soups]] @ 6:26, @ 7:14).

## Candidate draws (from Silver Bullet doctrine)

Identifying the next most likely **[[concepts/draw-on-liquidity|draw on liquidity]]** is the single most important skill — it's where price is trying to go ([[sources/2023-mentorship-silver-bullet]] @ 7:23, @ 7:48).

Candidates include ([[sources/2023-mentorship-silver-bullet]] @ 3:47–6:41):

- Previous day high / low (PDH, PDL)
- Previous session (London / NY) high / low
- Previous weekly high / low
- Current or old [[concepts/new-week-opening-gap|New Week Opening Gap (NWOG)]]
- [[concepts/optimal-trade-entry|OTE]] zones
- Inefficiencies / [[concepts/fair-value-gap|FVGs]] sitting above or below price

## Quality modifiers

- **Relative equal highs / lows** — equal levels amplify the liquidity pool above / below; frequently explicit targets ([[sources/internal-external-liquidity]] @ 11:16).
- **[[concepts/low-resistance-liquidity|Low-resistance liquidity]]** — lined-up previous-day lows (or highs) form a higher-quality draw ([[sources/internal-external-liquidity]] @ 8:06).
- **Important liquidity levels** — previous candle's high and low at HTF (e.g. previous month's low) ([[sources/internal-external-liquidity]] @ 10:47).

## Sweep vs Run (how liquidity gets consumed)

When price reaches a liquidity pool:

- **Sweep** — price trades through and **immediately reverses**. Synonym for [[models/turtle-soup|Turtle Soup]] / [[concepts/liquidity-sweep|liquidity sweep]] ([[sources/how-to-trade-turtle-soups]] @ 2:35).
- **Run** — price trades through and **continues** in the same direction. What breakout traders want; the opposite outcome of a sweep ([[sources/how-to-trade-turtle-soups]] @ 3:48, @ 4:34).

The NQ review clips repeatedly show the algorithm sweeping obvious sell-side pools — especially London lows and prior daily lows — before continuation or validation of the next array ([[sources/nq-review-april-30-2025]] @ 7:55, @ 9:04, [[sources/nq-heavy-manipulation-review]] @ 13:09).

If the leg into the swing point contains an FVG, **favor a run**. If the leg has no FVG (a "[[deferred/concepts/last-line-of-defense|last line of defense]]"), favor a sweep ([[sources/how-to-trade-turtle-soups]] @ 11:47, @ 12:11, @ 12:29).

## See also

- [[concepts/draw-on-liquidity]]
- [[concepts/liquidity-sweep]]
- [[concepts/internal-liquidity]]
- [[concepts/external-liquidity]]
- [[concepts/buyside-liquidity]]
- [[concepts/sellside-liquidity]]
- [[concepts/relative-equal-highs-lows]]
- [[concepts/low-resistance-liquidity]]
- [[models/turtle-soup]]
- [[models/internal-external-liquidity-model]]
