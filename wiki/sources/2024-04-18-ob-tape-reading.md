---
title: "Lecture On ICT Order Blocks & Tape Reading April 18, 2024"
type: source
raw: "[[Clippings/Lecture On ICT Order Blocks & Tape Reading April 18, 2024]]"
date_ingested: 2026-04-16
key_concepts:
  - concepts/order-block
  - concepts/fair-value-gap
  - concepts/dealing-range
  - concepts/change-in-state-of-delivery
  - concepts/volume-imbalance
  - concepts/consequent-encroachment
  - concepts/mean-threshold
  - concepts/breaker-block
  - concepts/optimal-trade-entry
  - concepts/judas-swing
  - concepts/liquidity
  - concepts/buyside-liquidity
  - concepts/sellside-liquidity
  - concepts/balanced-price-range
  - timing/macros
  - timing/killzones
tags: [source, order-block, tape-reading, live-stream, direct-ict]
---

# Lecture On ICT Order Blocks & Tape Reading April 18, 2024

Live stream on NQ / NASDAQ futures (April 18, 2024 — employment data day). ICT walks through a live bearish session setup and then delivers an extended lecture on order block identification, volume imbalances, and dealing ranges. Direct ICT source.

---

## Summary

- **Dealing range definition**: A dealing range requires that price takes **both sides of liquidity** — buy side AND sell side — on the time frame being traded. A range that only touches one side is not a dealing range. The midpoint of the dealing range is the equilibrium price point; the algorithm retraces to it before continuing the directional move.
- **Bearish OB — multiple consecutive up-closes**: When several consecutive up-closed candles precede the directional drop, the entire range of those candles defines the OB — not just the last candle. Divide that range in half (mean threshold) and in quarters; the best entries form **below mean threshold** (lower half of the composite range).
- **Last up-close shortcut**: The "last up-closed candle" rule is only valid when there is no preceding run of consecutive up-closes. If a single down-close breaks the green run and is immediately followed by the final up-close, that final candle alone is the OB. If the run is uninterrupted, the entire composite range applies.
- **Bullish OB and where to look**: For a bullish OB (consecutive down-closed candles), the ideal long entries are in the **upper portion** of the dealing range (premium side is where down-closed candles appear in an uptrend — this is not a contradiction; the OB itself is in the upper half of a retracement range). If a fair value gap exists in the **lower half** of that range, do not buy the down-close candle in the upper portion — price will reprice to the FVG+OB confluence in discount first.
- **Volume imbalance**: The gap between the bodies (not wicks) of two immediately adjacent candles. Weaker than an FVG. Price can pass through it multiple times. Stop losses must be placed above (for shorts) or below (for longs) the candle that creates the volume imbalance — not inside it.
- **Mean threshold**: The midpoint of a candle or candle group acting as an order block. Equivalent to consequent encroachment for a gap. A price that fails to reach mean threshold before reversing signals extra directional strength.
- **High-impact news driver rule**: On high-impact news driver days, do not trade below the 5-minute chart at the time of release. Wait a minimum of 15 minutes (ICT) or 30 minutes (students) before dropping to sub-5-minute charts. The algorithm seeks wider stops and premium/discount arrays on these days.
- **Bias framework**: Weekly → daily → intraday. Once you have a directional bias from weekly/daily, expect a Judas swing (fake counter-move) at 8:30 / session open before the true move. If bearish, buy side is taken first, then sell side — that sequence confirms the directional intent.

---

## Key quotes

> "You do have all of these consecutive up-closed candles which makes that a what an ICT bearish order block… these up-closed candles if you take the body or the opening price of that lowest one and draw that out." — @ 25:05

> "If you're looking for a bearish order block… up-closed candles that are in succession here one after the other that entire range has to be defined." — @ 2:03:51

> "The best setups are going to form below mean threshold which is the middle of the entirety of the multiple candlesticks that make up my IC bearish order block." — @ 2:18:09

> "If you ever have a series of immediate consecutive candles you have to define the range that all of those candles make, divide it in half, divide it in quarters and the best setups are going to form below mean threshold." — @ 2:18:09

> "When do you use the last up-close candle before the down move… if there is a break in this — for instance let's say this candlestick right here was a down-closed candle — then I would have used that candle as my bearish order block and none of this down here would have been a factor." — @ 2:17:38

> "What is an order block what is it… it's the change in the state of liquidity… it's where you are in the marketplace and how it changes its delivery where it pinpoints a very specific time it's specific in elements that provide you a very unambiguous range in price." — @ 1:50:35

> "For a bullish OB — the ideal entry points are not in the lower half… if you're bullish [an inefficiency] won't want to come back down here that's what you really want that's a signature in price delivery… the best buys will form between [the midpoint] and [the high of the inefficiency]." — @ 1:01:38

> "You want to see a down-closed candle in the upper portion of this range… caveat: if there is a fair value gap on the time frame you're looking at in the lower half, you do not buy a down-closed candle in the upper portion because it won't hold — it will drop down and reprice to the inefficiency." — @ 2:21:21

> "A dealing range is a high that has engaged buy side and a low that has engaged sell side… it must be on the time frame you're looking for in terms of the analysis." — @ 47:47

> "If you're bearish you want to see buy side taken first then drop down here — you don't want to see the market trade down, take out that low, and then take out buy side." — @ 1:09:43

> "A volume imbalance is any time frame where you have two candles immediately right next to each other… the difference between the bodies — not the wicks." — @ 1:54:54

> "Volume imbalances — you have to be flexible — they can pass through them and be used multiple times." — @ 1:59:08

> "The midpoint of that inefficiency is consequent encroachment… if it's a candlestick that makes an order block the midpoint is mean threshold." — @ 1:51:22

> "When price fails to even get to mean threshold that's a signature of strength of the move." — @ 1:52:16 (paraphrased from the passage; exact: "if it can go to just half of it or fall short of half of it when you're bearish… it indicates a signature in terms of strength of the move")

> "On high impact news drivers… at least refer to the 5-minute chart and try not to place so much emphasis on anything less than that… 15 minutes minimum up to 30 minutes." — @ 14:34 / 32:57

---

## See also

- [[concepts/order-block]]
- [[synthesis/how-to-use-order-blocks-and-dealing-ranges]]
- [[concepts/fair-value-gap]]
- [[concepts/volume-imbalance]]
- [[concepts/mean-threshold]]
- [[concepts/consequent-encroachment]]
- [[concepts/dealing-range]]
- [[concepts/judas-swing]]
- [[concepts/change-in-state-of-delivery]]
- [[concepts/breaker-block]]
- [[concepts/optimal-trade-entry]]
- [[concepts/price-delivery-continuum]]
- [[synthesis/how-to-use-price-delivery-continuum]]
- [[timing/macros]]
- [[timing/new-york-local-time]]
