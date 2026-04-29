---
type: concept
aliases: [HRLR, High Resistance Liquidity Run, High-Resistance Liquidity Run]
tags: [concept, liquidity, order-flow]
---

# High-Resistance Liquidity Run (HRLR)

A run that targets **already-swept** liquidity. The pool ICT's algorithm is reaching for has been visited before — the run faces opposing PD arrays, FVGs, and structure that act as resistance along the way.

## Defining feature

HRLR targets are **post-sweep** pools ([[sources/hrlr-vs-lrlr]]). The sweep has already occurred; the algorithm is now "stop-loss territory" for late participants.

This is the run-state version of [[concepts/high-resistance-liquidity]]: the market is moving through the already-swept side rather than reaching for the clean unswept target.

The 02/23/2026 SMC lecture adds a direct ICT Monday-compression example: the market can stay inside the same previous-candle range, probe around the new week opening gap, and still remain in HRLR / high-resistance conditions until it earns a closing breach below the relevant consequent encroachment ([[sources/ict-2026-smart-money-concepts-lecture-february-23-2026]] @ 4:54, @ 16:20, @ 19:13, @ 21:49, @ 13:32).

## Behavior signatures

- Choppy progress; FVGs get retested / filled during the move.
- Multiple structural reversals along the way.
- Slower expansion candles than [[concepts/low-resistance-liquidity-run|LRLR]].
- More likely to reverse short of the target — many HRLRs become [[concepts/failure-swing|failure swings]].

## When to expect HRLR

After a clean sweep + reversal (e.g. [[models/turtle-soup|Turtle Soup]]), the **pull-back leg in the direction of the prior trend** is HRLR — it's running at protective stops that have already been hunted. Avoid trading these continuations as if they were LRLRs.

In the derivative-teacher framing, high-resistance liquidity is also the stop-loss side of the curve: the target has already been swept, so the market is now working through more structure before it can reverse again ([[sources/hrlr-vs-lrlr]] @ 1:42, @ 1:21).

The lunch-macro commentary is a live HRLR example: price lingers around an inversion FVG / breaker context, partials are needed, and the move never becomes a clean one-shot run ([[sources/trading-high-resistance-liquidity-run-conditions-with-my-lunch-macro]] @ 0:57, @ 1:22, @ 6:53).
The 02/05/2025 forex/NQ review makes the same point from the FX side: when the tape is fuzzy, overlapping, and prone to overshoot, the stops must be wider and the trader has to treat Forex as a high-resistance environment instead of trying to force a tight-stop scalp ([[sources/2025-lecture-series-forex-nq-review-02052025]] @ 6:08, @ 6:23, @ 6:40, @ 7:03, @ 8:12, @ 8:42).
The 10/28/2024 mentorship lecture gives the direct Monday-session version: premarket can be the lower-resistance opportunity, but the 9:30 opening session is often higher resistance and should be treated with smaller expectations and lower leverage when the calendar is quiet ([[sources/ict-2024-mentorship-high-resistance-low-resistance-conditions-october-28-2024]] @ 6:34, @ 8:53, @ 12:38, @ 14:52).
The 03/25/2026 market commentary gives a direct ICT open example: he explicitly labels the morning "high resistance liquidity run conditions", uses 7:00–9:30 ET as the pre-open liquidity map, then lets the 9:30 open / opening-range-gap / first presented FVG decide whether the session is worth trading. When the tape is conflicted, he recommends lower leverage and waiting for the range to validate before treating the move as bullish or bearish ([[sources/ict-2026-market-commentary-march-25-2026]] @ 11:21, @ 12:40, @ 14:01, @ 15:30, @ 17:31, @ 17:47, @ 26:58).

## When [[concepts/fair-value-gap|FVGs]] are not forming

If no FVGs are forming during a [[timing/quarters-of-the-hour|quarter of the hour]], the market is in a HRLR state — sit still, wait the next quarter ([[sources/2025-price-delivery-continuum]] @ 21:01).

## See also

- [[synthesis/how-to-use-resistance-liquidity]]
- [[concepts/low-resistance-liquidity]]
- [[concepts/failure-swing]]
- [[concepts/liquidity-sweep]]
- [[concepts/market-structure-shift]]
- [[sources/hrlr-vs-lrlr]]
- [[sources/trading-high-resistance-liquidity-run-conditions-with-my-lunch-macro]]