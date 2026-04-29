---
type: source
title: "2022 ICT Mentorship Episode 5 - Intraday Order Flow & Daily Range"
source_type: youtube
raw: "https://www.youtube.com/watch?v=N29ZJ-o31xs"
date_ingested: 2026-04-27
key_concepts:
  - intraday-order-flow
  - daily-range
  - displacement
  - fair-value-gap
  - swing-high
  - swing-low
  - three-drives-pattern
  - liquidity
  - buy-side-liquidity
  - sell-side-liquidity
  - morning-session
  - afternoon-session
  - lunch-hour
  - pre-market
  - close-algorithm
  - futures-contract
  - roll-timing
  - new-york-local-time
  - measured-move
  - stop-hunt
tags:
  - 2022
  - mentorship
  - direct-ict
  - foundational
  - futures
  - ES
  - NQ
  - YM
aliases:
  - "2022 ICT Mentorship Episode 5"
  - "Intraday Order Flow & Daily Range"
  - "Daily Range Setup"
---

# 2022 ICT Mentorship Episode 5 - Intraday Order Flow & Daily Range

**Video**: [YouTube](https://www.youtube.com/watch?v=N29ZJ-o31xs) | **Duration**: 46:04 | **Channel**: The Inner Circle Trader | **Published**: February 1, 2022

## Summary

This episode teaches the **intraday order flow and daily range setup** for index futures (E-mini S&P 500, NASDAQ, Dow). It introduces the session structure (pre-market, morning, lunch, afternoon, close), the displacement concept, the three-drives pattern, and two core entry patterns: swing-low violation + stop hunt, and fair value gap. This is foundational material for the user's ES/NQ/MNQ trading workflow.

### Core themes

1. **Futures contract basics** — index futures trade March/June/September/December; roll to front month one week before expiration based on open interest.
2. **NY local time is mandatory** — all charts must be calibrated to New York local time.
3. **Daily session structure** — pre-market (before 8:30), morning (8:30–11:00), lunch (12:00–1:00 — no trade), afternoon (1:30–4:00), close algorithm (3:50–4:00).
4. **Swing points as liquidity** — 3-candle swing highs (buy-side liquidity) and swing lows (sell-side liquidity) identified on the 15-minute timeframe before 8:30 AM.
5. **Displacement** — energetic, obvious moves after liquidity raids; weak/anemic moves = no setup.
6. **Three drives pattern** — three presses into an old high, creating accumulation of buy-side liquidity; signals potential short setup when market breaks below.
7. **Two entry patterns** — (a) swing low violation + stop hunt, (b) fair value gap.
8. **Measured move** — afternoon session may duplicate the morning move magnitude.

---

## Key sections

### Futures contract basics

- **Index futures trade 4 months per year**: March (H), June (M), September (U), December (Z).
- **Expiration**: Third Friday of delivery month.
- **Symbol format**: ES2022 = E-mini S&P 500, March 2022 delivery.
- **Roll timing**: One week before expiration, monitor open interest (barchart.com) to identify which contract has larger liquidity.
- **Trade the front month** with highest open interest.

### Time zone requirement

> Set all charts to **New York Local Time** — non-negotiable for proper calibration.

### Daily session structure

| Session | Time (NY) | Purpose |
|---------|-----------|---------|
| **Pre-Market** | Before 8:30 AM | Identify swing highs/lows for stop placement |
| **Morning Session** | 8:30 AM – 11:00 AM | Primary trading window (news events at 8:30) |
| **Lunch Hour** | 12:00 PM – 1:00 PM | **NO TRADING** — avoid entirely |
| **Afternoon Session** | 1:30 PM – 4:00 PM | Secondary trading window |
| **Close Algorithm** | 3:50 PM – 4:00 PM | Aggressive pricing/acceleration into close |

**Key timing notes**:
- 1:30 PM is when macro algorithms activate.
- 20 minutes to 4:00, 10 minutes to 4:00, and 4:00 PM show market-on-close order activity.
- If you get a morning trade, consider squaring positions or taking profits before lunch rather than holding through.

### Pre-8:30 AM analysis: identifying liquidity

**Swing High** (3-candle pattern): candle with lower high to left AND lower high to right. Represents **buy-side liquidity** (buy stops above).

**Swing Low** (3-candle pattern): candle with higher low to left AND higher low to right. Represents **sell-side liquidity** (sell stops below).

### Three drives pattern

> "Three little endings pattern" — Linda Raschke & Larry Connors reference.

- Market presses up 3 times into old high.
- Each swing high is higher than previous.
- Creates accumulation of buy-side liquidity above.
- Signals potential short setup when market breaks below.

### Displacement concept

> "If you have a children's swimming pool and an elephant falls into it, the water is displaced. That's what you're looking for in price."

When price trades above an old high then trades back below it, look for **obvious, energetic displacement** — not weak/anemic moves.
- Weak moves = no setup.
- Energetic moves = valid displacement for entry consideration.

### Entry Pattern 1: Swing low violation + stop hunt

1. Identify swing low after 1:30 PM (afternoon session).
2. Wait for price to trade **below** that swing low (stop hunt).
3. Buy the sell stops resting below.
4. Expect rally through previous resistance.

### Entry Pattern 2: Fair value gap

1. Look for sudden displacement higher.
2. Identify fair value gap (imbalance between candles).
3. If price trades back down into FVG, buy it.
4. Expect continuation higher.

**Note**: Do NOT use order blocks in this methodology; focus on fair value gaps and swing points.

### Morning session strategy

**Objective**: Identify if morning creates bullish or bearish bias.

1. Look for **relative equal highs** = retail resistance = buy-side liquidity above.
2. Look for **higher swing lows forming** = accumulation/uptrend signal.
3. Identify **old highs** from previous days.
4. If three drives pattern forms into old high = short setup potential.
5. Preferably enter before 11:00 AM.

### Afternoon session strategy (1:30 PM+)

**Prerequisite**: Know your daily bias (expect range expansion higher or lower?).

1. Wait for 1:30 PM algorithm activation.
2. Identify first swing high and swing low after 1:30 PM.
3. Apply same stop-hunt logic as morning.
4. Look for buy programs (continuous higher pricing from algorithms).
5. Hold for close acceleration (3:50–4:00 PM).

### Measured move pattern

If morning moved up 200 points, afternoon may duplicate that move:
- Morning: +200 points
- Afternoon: +200 additional points
- Total daily range: +400 points

---

## Key quotes

> "If you have a children's swimming pool and an elephant falls into it, the water is displaced. That's what you're looking for in price."

> "Three little endings pattern"

> "Set all charts to New York Local Time — this is non-negotiable"

> "Lunch hour — no trading"

---

## See also

- [[concepts/fair-value-gap]] — the flagship PD array; Episode 5 teaches FVG as one of two core entry patterns.
- [[concepts/liquidity]] — buy-side and sell-side liquidity pools defined by swing highs/lows.
- [[concepts/liquidity-sweep]] — the stop-hunt pattern before entry.
- [[concepts/market-structure-shift]] — the structural confirmation after displacement.
- [[concepts/displacement]] — energetic moves that validate setups.
- [[timing/new-york-local-time]] — mandatory chart calibration.
- [[timing/first-hour-dealing-range]] — the 9:30–10:30 morning frame.
- [[timing/lunch-macro]] — the 11:30–1:30 midday window (note: Episode 5 says 12:00–1:00 PM no-trade).
- [[timing/macros]] — the ~20-minute pulses that activate at key times.
- [[timing/silver-bullet-windows]] — the 10:00–11:00 AM and 2:00–3:00 PM windows that overlap with Episode 5's session structure.
- [[concepts/swing-high]] — 3-candle pattern defining buy-side liquidity.
- [[concepts/swing-low]] — 3-candle pattern defining sell-side liquidity.
- [[concepts/three-drives-pattern]] — three presses into old highs/lows creating liquidity accumulation.
- [[models/turtle-soup]] — liquidity-sweep reversal model using the same stop-hunt logic.
- [[models/silver-bullet]] — time-window FVG execution model.
- [[sources/2022-ict-mentorship-episode-2]] — foundational setup framework (weekly bias → daily liquidity → entry).
- [[sources/2022-ict-mentorship-episode-3]] — MSS vs break, IRL, killzone boundaries.
- [[sources/2022-ict-mentorship-episode-4]] — practical examples of MSS + FVG + equilibrium.

## Extra linkage

- This episode is **foundational for intraday futures trading** — it provides the earliest ICT-direct session structure (pre-market / morning / lunch / afternoon / close) and defines the daily range setup for index futures specifically.
- The **"no trading at lunch" rule** (12:00–1:00 PM) is a stricter formulation than the later 11:30–1:30 lunch macro window. Both are valid; Episode 5 provides the earliest source.
- The **measured move pattern** (afternoon duplicating morning move) is a precursor to the later [[concepts/daily-profile|daily profile]] concepts and the [[models/power-of-three|PO3]] daily range logic.
- The **three drives pattern** is a classical technical analysis pattern (Linda Raschke / Larry Connors) that ICT incorporates into his liquidity framework. It is not unique to ICT but is taught as a liquidity accumulation signal.
- The **displacement concept** (energetic vs. anemic moves) is a foundational filter that appears across all later ICT material. Episode 5 provides one of the earliest and most memorable formulations.
- The **"trade the front month" rule** based on open interest is practical futures knowledge that supports the user's MNQ/NQ execution.
