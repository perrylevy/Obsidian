---
title: "ICT Mentorship 2023 – Market Maker Models"
type: source
raw: "[[Clippings/ICT Mentorship 2023 - Market Maker Models]]"
url: "https://www.youtube.com/watch?v=iKsIbUblSWM"
author: The Inner Circle Trader
published: 2023-11-01
date_ingested: 2026-04-16
key_concepts:
  - market-maker-buy-model
  - market-maker-sell-model
  - power-of-three
  - accumulation
  - manipulation
  - distribution
  - fair-value-gap
  - order-block
  - breaker-block
  - balanced-price-range
  - liquidity
  - buyside-liquidity
  - sellside-liquidity
  - draw-on-liquidity
  - smart-money-reversal
  - low-resistance-liquidity-run
  - killzones
---

# ICT Mentorship 2023 – Market Maker Models

ICT's final public teaching lecture before leaving the YouTube mentorship format. Presented as the most advanced framework he teaches — one that presupposes fluency with all PD arrays.

---

## Summary

- The **Market Maker Buy Model (MMBM)** and **Market Maker Sell Model (MMSM)** are ICT's name for the full algorithmic swing structure that underlies *all* price delivery — from the lowest discount to the highest premium and back. ICT states that "swing trading is all on the basis of a market maker sell model or a market maker buy model whether you realize it or not" (@ 28:16). The MMBM and MMSM are *distinct from and larger than* PO3/AMD: PO3 (Accumulation / Manipulation / Distribution) describes the three phases of a single swing *within* the model, while the MM model names and sequences the full arc including the buy/sell curve, accumulation stages, redistribution stages, and the smart money reversal at the apex.

- Price during a swing is divided into a **buy side of the curve** (price moving higher — buy side delivery) and a **sell side of the curve** (price moving lower — sell side delivery). The invisible dividing line is the highest high where reversal is anticipated (@ 46:53).

- The MMSM phases, in sequence (@ 23:04–53:48):
  1. **Original Consolidation** — price consolidates; smart money accumulates shorts in context; framed by a repeated level on the high side and the lowest low of the range.
  2. **Buy Side Delivery (buy side of the curve)** — price rallies, targeting buy side liquidity above relative equal highs and/or an overhead inefficiency (FVG).
  3. **Smart Money Reversal** — at the apex (inside a premium PD array on a higher time frame, e.g., a 60-min SIBI/FVG), price rejects. ICT labels this the hardest skill; it requires bodies staying within the PD array with only wicks exceeding it (@ 43:20).
  4. **First Stage Distribution** — first bearish entry after the reversal; price drops into a breaker or fair value gap, then retraces (@ 48:12–48:47).
  5. **Sell Side Delivery (sell side of the curve)** — price moves lower. PD arrays that served as support on the buy side *flip* and act as resistance on the sell side (@ 51:43–52:40).
  6. **Second Stage Redistribution** — the highest-velocity leg down; ICT calls it "the fastest elevator ride of the move" (@ 49:57). For students who classified the first distribution as the entry, this is the "unicorn" — second stage, everything in alignment, low-resistance liquidity run (@ 40:57–41:52).
  7. **Target: Original Consolidation Low** — sell side delivery aims to reprice *below* the original accumulation low to tag stop-losses of trapped longs (@ 47:19).

- The **MMBM** is the exact mirror (@ 3:22–3:49). ICT states: "for the sake of brevity everything I disclose in this teaching just reverse it for a market maker buy model." Phases: original consolidation (distribution of longs by smart money) → sell side delivery → smart money reversal at a discount PD array → first stage accumulation → reaccumulation → buy side delivery → second stage reaccumulation (unicorn long) → target: original consolidation high.

- **Re-accumulation / Redistribution** are mid-curve corrections back into a PD array that offer secondary entries. A return to the original consolidation boundary after price has already left it is called "return to original consolidation" and is the preferred low-risk entry (@ 31:51–32:21). If no return is offered, a second-stage re-entry inside a PD array (FVG consequent encroachment or order block) is the alternative (@ 41:52–42:25).

- **Time** locks in the model: consolidation near London open, buy side delivery into NY open (7:00 AM), smart money reversal inside the NY open killzone (7:00–9:00 AM), sell side delivery targeting the original consolidation low arriving at London close / NY AM session end (10:00 AM–12:00 PM NY) (@ 54:33–57:04).

- Prerequisite: "A market maker model is relying on your understanding of every PD array I've made available" (@ 0:35). Students who can see MM models quickly have fluency across breakers, mitigation blocks, inversion FVGs, BPR — not just order blocks (@ 1:09).

## Extra linkage

- [[models/market-maker-buy-model]] — bullish half of the full model pair
- [[models/market-maker-sell-model]] — bearish half of the full model pair
- [[models/power-of-three]] — the three-phase swing label nested inside the model
- [[concepts/accumulation]] — original accumulation stage of the round trip
- [[concepts/manipulation]] — stop-raid / manipulation leg of the round trip
- [[concepts/distribution]] — expansion / delivery leg of the round trip
- [[concepts/pd-array]] — the model walks across PD arrays and quadrant levels
- [[concepts/fair-value-gap]] — one of the core arrays used in the model
- [[concepts/order-block]] — the delivery-change block used in the model
- [[concepts/breaker-block]] — the mirror / return-entry structure
- [[concepts/balanced-price-range]] — the midpoint / balance behavior inside the curve
- [[concepts/smart-money-reversal]] — the apex turn at premium / discount
- [[concepts/draw-on-liquidity]] — the market is always running toward the next pool
- [[deferred/timing/killzones]] — the London / NY timing scaffold
- [[synthesis/how-to-use-pd-array-matrix]] — the matrix spine beneath the model family
- [[synthesis/how-to-use-price-delivery-continuum]] — the cycling delivery framework that complements the model

---

## Key Quotes

| Timestamp | Quote |
|-----------|-------|
| @ 0:35 | "A market maker model is relying on your understanding of every PD array I've made available." |
| @ 3:22 | "For the sake of brevity, everything I disclose in this teaching just reverse it for a market maker buy model." |
| @ 5:20 | "When I say swing trading — if I'm bullish I'm trading from discount to premium riding the coattails of buy side delivery; if I'm bearish I'm trading from premium to discount riding the coattails of sell side delivery." |
| @ 10:33 | "When price is running higher it's offering buy side; it's giving the marketplace buy side delivery as it's running higher." |
| @ 11:27 | "Buy side delivery is the actual animated movement of price moving higher. Liquidity is a stagnant price level or levels where stops would reside." |
| @ 23:04 | "Does the market offer a consolidation? That's what we would be expecting here — is it consolidating, is it offering a small little pause in price where it goes sideways for a little while, which would be accumulating long positions — that's allowing smart money to accumulate longs." |
| @ 27:26 | "When I call an original consolidation, that is where the market is accumulating." |
| @ 28:16 | "My premise behind swing trading is it's all on the basis of a market maker sell model or a market maker buy model — that's what swing trading is whether you realize it or not." |
| @ 31:51 | "When you understand it — when the market leaves the original consolidation and then comes back down in — if it trades back to that level, what's it doing? It's returning back to the original consolidation. That's how I teach my market maker sell model and buy model." |
| @ 40:57 | "Unicorn is second stage redistribution in a sell model — Market Maker Sell Model. When I say unicorn — everything's in your favor, you got everything behind you, it's so one-sided." |
| @ 41:20 | "The most qualifying factors in my trading is to find the easiest, highest-speed, low-resistance liquidity runs — they're going to always be the second stage redistribution in a market maker sell model." |
| @ 43:20 | "This is what I refer to as a smart money reversal. You are years away from ever being able to do that consistently." |
| @ 46:53 | "The highest high where we anticipate the likelihood of a reversal — to the left of that is the buy side of the curve… now on the left side is the sell side of the curve — that means we're in sell side delivery." |
| @ 47:19 | "Sell side delivery going to be aiming for the original consolidation low — why? Because it wants to reprice under the original accumulation for sell side liquidity — the stops resting below here for traders that rode this up." |
| @ 48:12 | "That bearish breaker — that is your first stage distribution." |
| @ 49:57 | "That bearish order block is your second stage redistribution — this is going to be the fastest elevator ride of the move going down." |
| @ 51:43 | "The buy side of the curve used in reverse in the sell side of the curve — meaning this down closed candle is a bullish order block. So while we were going up, when it drops back down into this it should be offering support. So when we get to the right side of the curve… anything offered as support or as a discount array needs to start acting as a premium array or resistance." |
| @ 54:33 | "One of the wonderful elements not been discussed so far — when everything with price is in agreement with time. Because time sets the stage, then price does the act of precision." |
| @ 57:04 | "London close, 10 o'clock to noon New York local time — friends and neighbors, that's not random." |

---

## Structural Notes

### Buy/Sell Curve
ICT uses the metaphor of a **curve** — an invisible arc dividing the bullish leg (buy side of the curve) from the bearish leg (sell side of the curve). The apex is the smart money reversal point. Everything to the left of the apex is buy side delivery; everything to the right is sell side delivery (@ 46:53).

### PD Arrays Flip Role at the Apex
On the buy side of the curve, a down-closed candle (bullish OB) acts as support. Once price crosses to the sell side of the curve, that same candle's body becomes *resistance* — price retraces to it and rejects lower (@ 51:43–52:59). This is a precise ICT doctrine point: the same PD array changes classification depending on which side of the curve price is on.

### MMSM Phase Map (condensed)

```
SELL SIDE OF THE CURVE (right of apex) ←—————— APEX (Smart Money Reversal) ——————→ BUY SIDE OF THE CURVE (left of apex)
                                                 ↑ 60-min FVG / Premium PD Array
[2nd Stage Redistribution]  [1st Stage Distribution]            [Original Consolidation] → BSL taken → Smart Money Reversal
      ↓ (fastest leg)              ↓
[Original Consolidation Low / SSL target]
```

### MMBM is Mirror
Everything above applies in reverse: original consolidation distributes shorts → sell side delivery → smart money reversal at a discount PD array → 1st stage accumulation → (re-accumulation) → 2nd stage reaccumulation (unicorn long) → original consolidation high (@ 3:22).

### Instrument
ICT reveals at @ 53:48 that the example chart was GBP/USD (British Pound vs. US Dollar Forex pair), but states the concepts are universal across all asset classes.

---

## See also

- [[models/market-maker-buy-model]]
- [[models/market-maker-sell-model]]
- [[models/power-of-three]]
- [[concepts/accumulation]]
- [[concepts/manipulation]]
- [[concepts/distribution]]
- [[concepts/fair-value-gap]]
- [[concepts/order-block]]
- [[concepts/breaker-block]]
- [[concepts/balanced-price-range]]
- [[concepts/liquidity]]
- [[concepts/buyside-liquidity]]
- [[concepts/sellside-liquidity]]
- [[concepts/draw-on-liquidity]]
- [[concepts/low-resistance-liquidity-run]]
- [[deferred/timing/killzones]]
