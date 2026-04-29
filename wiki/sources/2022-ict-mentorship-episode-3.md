---
type: source
title: "2022 ICT Mentorship Episode 3 - Internal Range Liquidity & Market Structure Shifts"
source_type: youtube
raw: "https://www.youtube.com/watch?v=nQfHZ2DEJ8c"
date_ingested: 2026-04-26
key_concepts:
  - internal-range-liquidity
  - market-structure-shift
  - market-structure-break
  - fair-value-gap
  - order-block
  - change-in-state-of-delivery
  - buyside-liquidity
  - sellside-liquidity
  - killzone
  - london-killzone
  - new-york-killzone
  - asian-session
  - liquidity-sweep
  - relative-equal-highs-lows
  - premium-discount
  - time-frame-alignment
tags:
  - 2022
  - mentorship
  - direct-ict
  - foundational
  - killzone
  - market-structure
aliases:
  - "2022 ICT Mentorship Episode 3"
  - "Internal Range Liquidity & Market Structure Shifts"
  - "IRL & MSS"
---

# 2022 ICT Mentorship Episode 3 - Internal Range Liquidity & Market Structure Shifts

**Video**: [YouTube](https://www.youtube.com/watch?v=nQfHZ2DEJ8c) | **Duration**: 52:27 | **Channel**: The Inner Circle Trader | **Published**: January 25, 2022

## Summary

This episode defines the critical distinction between **market structure shifts** (intraday legs) and **market structure breaks** (longer-term moves), introduces **internal range liquidity** as a precision entry concept, provides the canonical **killzone time boundaries**, and explains order blocks as "change in state of delivery." It is one of the highest-impact foundational episodes in the 2022 mentorship.

### Core themes

1. **Market Structure Shift vs. Break** — intraday shifts can reverse same-day; breaks are multi-day.
2. **Internal Range Liquidity (IRL)** — short-term highs/lows inside a retracing price leg, used for precision entries.
3. **Killzone boundaries** — canonical clock times for London (2:00–5:00 AM NY) and New York (7:00–10:00 AM NY) sessions.
4. **Order Blocks as Change in State of Delivery** — the opening price of a consecutive series marks where delivery flips from sell-side to buy-side or vice versa.
5. **Fair Value Gaps** — single-candle imbalance gaps used for entry and target zones.
6. **Algorithmic behavior** — HFT algorithms operate on sub-1-minute timeframes and "offer price" rather than respond to volume.

---

## Key sections

### Market Structure Shift vs. Market Structure Break

**Critical distinction**:
- **Market Structure Shift** = Intraday price leg. May reverse the same day. The signature is a liquidity run above/below relative equal highs/lows that then fails to continue.
- **Market Structure Break** = More significant, longer-term movement that confirms a sustained directional change.

> "for intraday i want you to think about intraday market structure shifts because it's not necessarily a break in market structure that leads to prolonged multi-day movement"

**The sequence**:
1. Market trades into liquidity (old lows/highs).
2. Market runs above/below relative equal highs or old highs.
3. This creates a **fake run** that signals a potential shift.
4. Evidence: When short-term highs are taken out with liquidity below them.

### Liquidity pools — where stops rest

**Buy-Side Liquidity (Buy Stops)**:
- Above old highs
- Above relative equal highs

**Sell-Side Liquidity (Sell Stops)**:
- Below old lows
- Below relative equal lows

> "it's just logic it's simple look at the chart everybody's trying to do something based on some kind of theory logic whatever some system there's buyers and sellers coming in at all times"

### The algorithm's behavior

**High-frequency trading algorithms** operate on:
- 3-minute, 2-minute, 1-minute charts
- Sub-one-minute intervals (45-second, 30-second, 15-second)

**What algorithms actually do**:
- They don't respond to "buying/selling pressure."
- They constantly **offer price at higher levels** (when rallying).
- They constantly **offer price at lower levels** (when declining).
- This is a **change in state of delivery**, not volume-driven movement.

> "if high frequency algorithms are operating every single day then these signatures will be in the chart"

### Order blocks — change in state of delivery

**Bearish Order Block**:
- Series of consecutive down-close candles.
- Opening price of the series extended in time.
- Significant only if it has taken liquidity and created a market structure shift.

**Bullish Order Block**:
- Series of consecutive up-close candles.
- Opening price of the series extended in time.
- Marks a change from sell-side to buy-side delivery.

**Key insight**:
> "the opening on that candle starts this series of delivery on the downside when that opening price gets violated here it changes its state of delivery now it was offering sell side when it goes above that opening now it's offering buy side"

This is the earliest ICT-direct source for the **change in state of delivery** framing that later becomes the canonical order-block definition.

### Fair Value Gaps (FVG)

**Definition**: A candle with a high that doesn't completely overlap the next candle's low, creating a gap.

**Characteristics**:
- Single candle pass up, next candle has a low that doesn't overlap.
- Represents imbalance in the market.
- Used as entry/target zones.

**Multiple FVG Strategy**:
When two fair value gaps exist (one lower, one higher):
- Sacrifice the better entry (lower FVG).
- Wait for price to trade into lower FVG and return to higher FVG.
- Enter when price accumulates in the higher FVG.
- Expect the lower FVG won't be retested.

### Killzone boundaries — canonical time windows

This episode provides the **definitive clock boundaries** for ICT killzones:

| Session | Time (New York local) | Notes |
|---------|----------------------|-------|
| **London Killzone** | **2:00 AM – 5:00 AM** | Track session highs and lows; market often sweeps above/below these levels |
| **New York Killzone** | **7:00 AM – 10:00 AM** | Primary execution window |
| **Asia Session** | **7:00 PM – 9:00 PM** | Evening session; less emphasized for intraday futures |

**Optimal trading hours**:
- **8:30 AM – 11:00 AM** (can extend to noon)
- **Avoid**: Noon hour (problematic)
- **Resume**: 1:30 PM – 4:00 PM (afternoon trend)
- **Best afternoon setup**: 2:00 PM – 3:00 PM

> "8:30 to 11:00 is the sweet spot... the noon hour is problematic... 1:30 to 4:00 you can get afternoon trend"

### Internal Range Liquidity (IRL)

> "internal range liquidity is looking for short-term lows or short-term highs inside a price leg that we're retracing back into"

**Components**:
- Short-term higher lows with stops above/below.
- Imbalances within the same range of price action.
- Used for precision entries when price retraces into a leg rather than sweeping external liquidity.

### Live trading example (Nasdaq E-Mini)

**Setup identified**:
- Fair value gap in premium (green shaded area).
- Smaller FVG below it (pink rectangle).
- Market structure shift bullish.

**Trade execution**:
- Entry: Buy at market when price accumulates in green FVG.
- Stop: Set to preserve 3.25% risk (personal preference).
- Target: Low end of pink rectangle (low-hanging fruit).
- Result: +$1,190 profit.

> "i'm not suggesting that every trade you take forward from this day on is going to be like this it doesn't mean it guarantees profit"

### Homework assignment

1. Go through e-mini futures intraday charts (15-min, 3-min, 2-min, 1-min).
2. Identify **stop hunts that lead to market structure shifts**.
3. Log examples with your own annotations in a study journal.
4. Focus on **8:30 AM – 12:00 PM NY local time**.

---

## Key quotes

> "for intraday i want you to think about intraday market structure shifts because it's not necessarily a break in market structure that leads to prolonged multi-day movement"

> "if high frequency algorithms are operating every single day then these signatures will be in the chart"

> "the opening on that candle starts this series of delivery on the downside when that opening price gets violated here it changes its state of delivery"

> "internal range liquidity is looking for short-term lows or short-term highs inside a price leg that we're retracing back into"

> "8:30 to 11:00 is the sweet spot"

---

## See also

- [[concepts/market-structure-shift]] — the canonical home for MSS; Episode 3 provides the intraday vs. break distinction.
- [[concepts/order-block]] — the strict definition; Episode 3 provides the "change in state of delivery" framing.
- [[concepts/change-in-state-of-delivery]] — the precise OB delivery-change level.
- [[concepts/fair-value-gap]] — the flagship PD array; Episode 3 adds the multiple-FVG strategy.
- [[concepts/liquidity]] — buy-side and sell-side liquidity pools.
- [[concepts/liquidity-sweep]] — the stop-hunt pattern before MSS.
- [[concepts/internal-liquidity]] — the range-internal inefficiency concept.
- [[concepts/external-liquidity]] — swing highs/lows at range edges.
- [[concepts/premium-discount]] — the 50% midpoint matrix.
- [[timing/killzones]] — the deferred page that this episode now validates.
- [[timing/london-killzone]] — London 2:00–5:00 AM NY.
- [[timing/new-york-killzone]] — New York 7:00–10:00 AM NY.
- [[timing/asian-range]] — Asian session 7:00–9:00 PM NY.
- [[timing/silver-bullet-windows]] — the 10:00–11:00 AM and 2:00–3:00 PM windows that overlap with the NY killzone.
- [[models/internal-external-liquidity-model]] — the IRL/ERL framework that Episode 3 directly defines.
- [[sources/2022-ict-mentorship-episode-2]] — the prior episode that established the foundational setup framework.

## Extra linkage

- This episode is **foundational ICT doctrine** — it provides the earliest direct-ICT definitions for market structure shift (vs. break), internal range liquidity, order blocks as "change in state of delivery," and the canonical killzone clock boundaries. These concepts appear across the entire wiki but this is one of the primary sources.
- The **killzone boundaries** (London 2:00–5:00 AM, NY 7:00–10:00 AM) from this episode are the definitive citation that resolves the `[!note] Uncited` warning on [[timing/killzones]]. This is a major gap closure.
- The **order block as "change in state of delivery"** framing in this episode is the precursor to the more formalized OB definition in later material. Episode 3 should be cited alongside later sources for the complete OB doctrine.
- The **multiple FVG strategy** (sacrifice lower FVG, enter at higher FVG) is an early formulation of what later becomes the "stacked FVG" handling rule. Both are valid; Episode 3 provides the foundational logic.
- The **8:30 AM – 11:00 AM "sweet spot"** and **2:00 PM – 3:00 PM afternoon window** align with the later Silver Bullet window definitions (10:00–11:00 AM and 2:00–3:00 PM). Episode 3 provides the earliest ICT-direct source for these time preferences.
- The **HFT algorithm description** (operating on sub-1-minute timeframes, "offering price" rather than responding to volume) is unique to this episode and provides important context for why ICT emphasizes 1-minute and sub-1-minute entry timeframes.
