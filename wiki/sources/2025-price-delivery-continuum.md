---
type: source
title: "2025 Lecture Series - Algorithmic Price Delivery Continuum"
source_type: youtube
raw: "[[Clippings/2025 Lecture Series - Algorithmic Price Delivery Continuum]]"
date_ingested: 2026-04-15
key_concepts:
  - price-delivery-continuum
  - fair-value-gap
  - inversion-fair-value-gap
  - balanced-price-range
  - consequent-encroachment
  - institutional-orderflow-entry-drill
  - pd-array
  - draw-on-liquidity
  - low-resistance-liquidity-run
  - high-resistance-liquidity-run
  - breakaway-gap
  - measuring-gap
  - order-block
  - change-in-state-of-delivery
  - macros
  - quarters-of-the-hour
---

# 2025 Lecture Series - Algorithmic Price Delivery Continuum

## Summary

- Introduces the **Price Delivery Continuum** theory: instead of top-down analysis, continuously cycle back through HTF → LTF charts (15m at every 15m close, 5m at every 5m close, etc.) while operating primarily on the 1-minute.
- Claims a fair value gap forms every 15-minute quarter of the hour (10:00–10:15, 10:15–10:30, etc.) on whatever timeframe is being traded — four potential FVGs per hour — provided a draw on liquidity exists.
- Distinguishes **low-resistance liquidity run** (FVGs are forming / being respected) vs **high-resistance liquidity run** (no FVGs forming — sit and wait in 15-minute increments, potentially all session).
- When studying a bearish FVG, focus on the **upper half**; for a bullish FVG, the **lower half**. Back-and-forth delivery in the "wrong" half makes it a **Balanced Price Range**; the opposite half becomes the true imbalance to be delivered to.
- Explicitly rejects retail order-flow tools (Level 2, DOM, footprint, VWAP, volume profile, POC, Ichimoku, Heikin-Ashi) — the algorithm only references **time + OHLC**; it does not see contracts or stops.
- Stop-loss placement rule: once price works the upper half of a bearish FVG as a BPR, place stops in the upper quadrant of the shaded area (conservative: just above the high); half-size re-entry if stopped.
- Ties the setup together with a macro window (10:50 a.m. – 11:10 a.m.) and a bearish **order block** (lowest opening of consecutive up-closed candles = change in state of delivery).
- Frames unfilled gaps on the 1m as **breakaway gaps**, with a follow-on **measuring gap** projecting a second equal move.

## Key quotes

- **@ 00:35** — "in this lecture we're going to be covering how to visually read actual order flow without retail gimmicks like level two data depth of Market ladders even footprint"
- **@ 04:38** — "fails to trade down to its consequent encroachment which is the midpoint right here in that line so that's institutional orderflow entry drill"
- **@ 12:33** — "that is my price delivery Continuum theory that means I'm constantly cycling through all those time frames it's not top- down analysis it's cycling through continuously looking for algorithmic PD rise"
- **@ 14:29** — "if you know where the market is likely to go that's the bias the draw and liquidity if you know that open high low and close and the time of the day or the session is all that you need"
- **@ 16:59** — "this back and forth price action in the upper half of that is a balanced price range what makes it balanced the fact that we're in the upper half of a bearish fair value Gap"
- **@ 19:09** — "when do fair value gaps form inside the quarters now that's not quarters Theory okay... what I'm talking about is time so if we were looking at the time of 10:00 in the morning Eastern Standard Time from 10:00 at the top of the hour to 10:15 there's going to be a fair value Gap that forms every time frame"
- **@ 19:38** — "that means there's four potential fair value gaps that form per hour... that's high frequency trading algorithm"
- **@ 21:01** — "if the Market's going to be range bound it might not create that because why we're going to be in a high resistance Li quility run conditions"
- **@ 22:09** — "sell side imbalance buy side inefficiency meaning that it needs to offer price back up to the midpoint that's what you'd be waiting for that's what the algorithm is doing"
- **@ 26:41** — "the only thing it refers back to is number one time and then it works on the Open high low and close it doesn't use high Kashi it doesn't use ichimoku"
- **@ 27:31** — "your stop can be in the upper quadrant of that known area right there because that's not likely to fill more conservative approach would be put your stop loss just above that shaded area"
- **@ 28:04** — "I would reenter the short and place a stop loss again in the upper quadrant of it or just above the high with half the number of contracts that I just took"
- **@ 31:52** — "my macro time 10:50 a.m. to 11:10 macro hello southbound train baby"
- **@ 32:15** — "let Clos candles consecutively are a bearish order block that's not a supply Zone okay it's the change in the state of delivery which is the lowest opening price of these consecutive candlesticks"
- **@ 36:23** — "you have a breakaway Gap that was up here and this is going to be a measuring Gap so half halfway from it starts dropping this is about halfway and you know there have another measure move to that level here"

## See also

- [[concepts/price-delivery-continuum]]
- [[synthesis/how-to-use-price-delivery-continuum]]
- [[concepts/fair-value-gap]]
- [[concepts/inversion-fair-value-gap]]
- [[concepts/balanced-price-range]]
- [[concepts/consequent-encroachment]]
- [[deferred/concepts/institutional-orderflow-entry-drill]]
- [[concepts/pd-array]]
- [[concepts/draw-on-liquidity]]
- [[concepts/low-resistance-liquidity-run]]
- [[concepts/high-resistance-liquidity-run]]
- [[concepts/breakaway-gap]]
- [[concepts/measuring-gap]]
- [[concepts/order-block]]
- [[concepts/change-in-state-of-delivery]]
- [[timing/macros]]
- [[timing/quarters-of-the-hour]]
- [[synthesis/how-to-trade-the-930-11am-window]]
