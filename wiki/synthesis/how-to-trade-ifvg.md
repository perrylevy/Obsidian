---
type: synthesis
aliases: [IFVG Playbook, How to Trade Inversion FVG]
tags: [synthesis, playbook, ifvg, entry]
---

# How to Trade IFVG

This page is the operator guide for trading **inversion fair value gaps**. The core idea is simple: wait for an FVG to be violated and swiftly closed through, then use the flipped area as a continuation trigger or pullback entry, but only when higher-time-frame context supports the move ([[concepts/inversion-fair-value-gap]], [[sources/how-to-trade-ifvg]] @ 0:38, @ 4:00, @ 7:22).

## Core operating sequence

1. Establish the higher-time-frame bias and swing context first.
2. Identify the relevant FVG or stacked FVG cluster.
3. Make sure the lower-time-frame candle-two sweep supports expansion with a small wick.
4. Wait for the close through the gap to confirm the inversion.
5. Enter on the close-through or the next candle open, depending on the framing.
6. Keep the stop beyond the swing / HTF wick and target the other side of the range or a reasonable R multiple.

## What makes an IFVG valid

- The gap must be not respected and swiftly closed over, not just touched.
- The higher-time-frame structure must still support the reversal or continuation.
- A sweep of candle one's high or low and a small wick on candle two strengthen the setup.
- SMT between candle one and candle two is optional confluence, not a requirement.
- If the opposing move is large, expect the expansion to wait until the next HTF candle.

The January 24, 2026 TTrades clip is a useful supplement to the core rule-set: it treats IFVG as an HTF-aligned continuation / reversal tool, not a raw pattern trade. The practical filter is sweep first, then inversion, then entry only if the candle-two wick and the broader expansion context agree; otherwise wait for the next HTF candle or pass ([[sources/how-to-trade-ifvg]] @ 1:07, @ 1:32, @ 2:03, @ 4:00, @ 5:19, @ 6:45, @ 12:13).

The "This Stupid Simple Strategy Works Everyday" clip is the same IFVG family stripped down to a low-R operating style: HTF FVG tap, 5-minute FVG confirmation, inversion out of the lower gap, then a liquidity target. The management rules are equally plain: stop at the swing that manipulated into the 5-minute gap, move to breakeven at the internal high / low, and only re-enter if the higher-time-frame draw is still intact ([[sources/this-stupid-simple-strategy-works-everyday-stupid-simple-and-proven]]).

## Common execution modes

### Continuation mode

Use IFVG as a continuation trigger when the market is already in the prevailing direction and the inversion confirms the next leg.

### Reversal mode

Use IFVG as a reversal anchor when the source of the move is a clear liquidity sweep and price shows a clean V-shape response.

### Aggressive live-tape mode

Derivative-teacher examples sometimes enter on the first violation inside the FVG rather than waiting for the pullback. Treat that as a more aggressive variant, not the default ICT-direct rule.

The NQ live tape-reading AM review uses this kind of live execution framing on an opening-day review: the morning spike is treated as a Judah swing into the daily OB/NWOG scaffold, then the IFVG is used to time the long rather than chasing the open itself ([[sources/nq-live-tape-reading-am-review]] @ 6:55, @ 10:38, @ 12:20, @ 13:08).

The same review also shows a more aggressive failure-short variant: if price is already above midnight and 8:30 opens, and buy side has been run, the trader can short inside the bullish IFVG as it starts to fail instead of waiting for a full return to the gap ([[sources/nq-live-tape-reading-am-review]] @ 26:32, @ 26:56, @ 27:28).

If the gap is expected to stay open as a breakaway gap, require immediate feedback; do not accept a slow drift into consequent encroachment or the OB below ([[sources/nq-live-tape-reading-am-review]] @ 4:16–4:43).

The Trump-volatility NQ reclaimed-IFVG clip is a cleaner live example of the same family: a Judas-swing lower into bullish context, then an IFVG reclaim back toward buy-side liquidity inside the morning window ([[sources/nq-trade-breakdown-reclaimed-ifvg-entry-with-trump-volatility-live-account-ict-concepts]]).

## What to avoid

- Trading the pattern with no HTF alignment.
- Forcing IFVGs when the chart is consolidating instead of expanding.
- Treating every visible gap as equally important.
- Ignoring candle-two behavior and wick size.
- Ignoring stacked FVG aggregation when the source shows them functioning as one broader imbalance.

## Practical checklist

- [ ] HTF context is clear
- [ ] FVG or stacked FVG is identified
- [ ] Candle-two sweep supports expansion
- [ ] Close-through / inversion is confirmed
- [ ] Entry plan matches the session and candle framing
- [ ] Stop is beyond the invalidation point

## See also

- [[concepts/inversion-fair-value-gap]]
- [[concepts/fair-value-gap]]
- [[concepts/change-in-state-of-delivery]]
- [[concepts/smt]]
- [[deferred/concepts/v-shape-reversal]]
- [[models/fractal-model]]
- [[concepts/time-frame-alignment]]
- [[sources/how-to-trade-ifvg]]
