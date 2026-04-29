---
type: source
title: "2022 ICT Mentorship Episode 2 - Elements To A Trade Setup"
source_type: youtube
raw: "https://www.youtube.com/watch?v=tmeCWULSTHc"
date_ingested: 2026-04-26
key_concepts:
  - fair-value-gap
  - market-structure-break
  - liquidity
  - premium-discount
  - weekly-bias
  - seasonality
  - auction-theory
  - imbalance
  - draw-on-liquidity
  - stop-hunt
tags:
  - 2022
  - mentorship
  - direct-ict
  - foundational
  - futures
  - NQ
  - MNQ
aliases:
  - "2022 ICT Mentorship Episode 2"
  - "Elements To A Trade Setup"
---

# 2022 ICT Mentorship Episode 2 - Elements To A Trade Setup

**Video**: [YouTube](https://www.youtube.com/watch?v=tmeCWULSTHc) | **Duration**: 49:35 | **Channel**: The Inner Circle Trader | **Published**: January 21, 2022

## Summary

This is the foundational setup episode of the 2022 ICT Mentorship. ICT introduces the complete trade setup framework: weekly bias → daily liquidity → hourly framework transposition → 15-minute liquidity pool identification → 2-minute/1-minute entry execution. He demonstrates live executions from his own account and emphasizes finding larger intraday moves rather than scalping small handle counts.

### Core themes

1. **Weekly bias as foundation** — analyze weekly candles on weekends; determine if the week will expand higher or lower.
2. **Seasonality and macro context** — Fed policy, earnings season, and market tone inform weekly directional bias.
3. **Liquidity hunting** — algorithms run stops before major moves; buy stops above highs, sell stops below lows.
4. **Break in market structure** — the key signature: market breaks below a short-term low after consolidation and liquidity engineering.
5. **Fair value gap (imbalance)** — ICT's 2016-introduced concept: a single candle passes with no overlap, creating an inefficiency the algorithm must correct.
6. **Premium/Discount matrix** — the 50% midpoint of the daily range; bearish trades target discount, bullish trades target premium.
7. **Independence** — the goal is skill-based trading where you need only the chart, not signals or handholding.

---

## Key sections

### Markets and leverage (1:40)

**Three main index futures**:
- E-mini S&P 500 (ES) — $50/handle, ~$12,500 margin
- E-mini NASDAQ (NQ) — $20/handle, ~$177,000 margin (faster, more aggressive)
- E-mini Dow (YM)

**Micro contracts** reduce tick multiplier and margin requirements, making them accessible for learning.

**Handle definition**: One handle = 4 ticks (minimum fluctuation).

### Weekly analysis — the foundation (13:49)

Before each trading week:
1. Analyze the weekly candle on the weekend.
2. Determine bias: will the week expand **higher or lower**?
3. Don't predict the exact close — just anticipate direction.
4. Use **seasonality**, Fed policy, earnings season, and overall market tone to inform the bias.

> "The market draws to specific levels like a paperclip to a magnet."

**Example from the episode**: Looking for lower prices based on:
- Seasonal tendencies (market tends to go down around this time)
- Fed interest rate increases
- Earnings season volatility
- Overall market weakness

### Daily chart — liquidity and swing points

- Identify **swing highs and swing lows** for liquidity.
- Majority of trading analysis should focus on this timeframe.
- Understand where the market sits within the weekly range expansion.

### Hourly chart — framework transposition (18:22)

- Transpose daily levels (old highs/lows) to the hourly chart.
- Watch for **liquidity runs** and **stop hunts**:
  - Sell stops rest below swing lows.
  - Buy stops rest above swing highs.
- **Pattern**: Market often drops to trigger sell stops, then runs up to trigger buy stops before the main move.

> "Anytime a significant price move lower is expected, always anticipate some measure of a stop hunt on buy stops or a short-term high being taken out."

### 15-minute chart — liquidity pool identification

- Identify **relative equal highs/lows**.
- Watch for **break in market structure** — the key signature.
- Prepare for entry setup on lower timeframes.

### 2-minute to 1-minute charts — entry execution

- Best timeframes for finding **imbalances** (fair value gaps).
- **Imbalance definition**: A single candle passes higher/lower with no overlap from adjacent candles.
- Look for **break in market structure** after liquidity run.
- **Entry trigger**: Market trades into the imbalance.

### The setup pattern — bearish example

**Sequence**:
1. **Liquidity run**: Market runs above old highs (triggers buy stops).
2. **Break in market structure**: Market breaks below recent swing low.
3. **Imbalance formation**: Gap created between candles (fair value gap).
4. **Entry trigger**: Market trades up into the imbalance → **sell short**.

**Stop loss**: Place above the high of entry candle or above the imbalance high.

### The liquidity matrix — premium and discount (35:22)

- Calculate range: daily high to daily low.
- Find 50% midpoint using Fibonacci.
- **Premium market** = above 50% level (expensive).
- **Discount market** = below 50% level (cheap).

**Trading logic**:
- If bearish (going short), look for market to move from premium to discount.
- Algorithms reprice lower in sell programs regardless of buying pressure.
- Target: below the 50% level where sell stops reside.
- Bonus: often an imbalance (fair value gap) near the old low.

> "Prefer low-hanging fruit targets rather than chasing extreme lows."

### Fair value gap — the imbalance (30:05)

ICT's unique framework introduced in 2016:
- A single candle passes in one direction.
- Previous and next candles do not overlap.
- Creates an unfilled area in price.
- The algorithm will eventually return to "efficiently price" the gap.

**Visual**:
```
Candle 1: High at X
Candle 2: Opens higher, trades higher, stops
Candle 3: Low is higher than Candle 1's high
= Fair Value Gap (imbalance between Candle 1 high and Candle 3 low)
```

### Live trade example (from thinkorswim live account)

- Entry 1: 14,720 → Exit: 14,732 = **12 handles**
- Entry 2: 14,756 → Exit: 14,784 = **28 handles**
- Entry 3: 14,798 → Exit: 14,675 = **123 handles** ← primary teaching example

All entries shown from a **live account**, not demo.

---

## Key quotes

> "I'm going to teach you skill sets that focus primarily on this... you want to find a nice price leg intraday." (@ 0:49)

> "Take notes, we dive deeper each new episode and build on the previous episode." (@ opening)

> "Anytime a significant price move lower is expected, always anticipate some measure of a stop hunt on buy stops or a short-term high being taken out." (@ 18:22)

> "There absolutely is an algorithm and it's manipulating the markets every single day, every single tick — it's completely controlled." (@ algorithmic price delivery)

> "The market draws to specific levels like a paperclip to a magnet." (@ weekly bias)

> "Prefer low-hanging fruit targets rather than chasing extreme lows." (@ target selection)

---

## See also

- [[concepts/fair-value-gap]] — the 3-candle inefficiency pattern; ICT's flagship entry concept.
- [[concepts/liquidity]] — buy-side and sell-side liquidity pools.
- [[concepts/liquidity-sweep]] — the stop-hunt pattern before major moves.
- [[concepts/market-structure-shift]] — the break in structure signature.
- [[concepts/premium-discount]] — the 50% midpoint matrix for target selection.
- [[concepts/draw-on-liquidity]] — targeting the next liquidity pool.
- [[models/power-of-three]] — the weekly accumulation/manipulation/distribution frame.
- [[models/market-maker-buy-model]] — the bullish swing-delivery round-trip.
- [[models/market-maker-sell-model]] — the bearish mirror.
- [[timing/weekly-open]] — the Monday open reference.
- [[sources/2022-ict-mentorship-no-rant-expectations]] — the orientation episode.

## Extra linkage

- This episode is **foundational ICT doctrine** — it defines the complete setup framework that later episodes build on. Every concept here (FVG, liquidity, market structure break, premium/discount) appears repeatedly across the wiki but this is one of the earliest ICT-direct sources that ties them together as a system.
- The **weekly bias** framing here is the precursor to the weekly profile concept. ICT does not yet use the term "weekly profile" in this episode, but the weekend analysis routine (weekly candle → directional bias → daily liquidity → hourly transposition) is the same logic.
- The **seasonality** reference here is brief but significant: "tends to go down around this time." This is the seed of the seasonal tendencies concept that gets expanded in later mentorship months. One source is insufficient for a standalone seasonal-tendencies page; wait for Month 03-04 content.
- The **premium/discount matrix** (50% midpoint of daily range) is an early formulation of what later becomes the PD Array Matrix quadrant system. This episode uses a simpler 2-zone split (premium above, discount below) rather than the 4-quadrant version from 2025. Both are valid; this source provides the foundational 2-zone logic.
- This episode does **not** define killzone clock boundaries. The killzone timing gates (London 02:00-05:00, NY 07:00-10:00) are introduced in later episodes (likely Episode 3-5). This source should be ingested for its framework content, but the killzone boundary gap remains open until a later episode is sourced.
- The **live account executions** are significant because they demonstrate ICT trading his own framework in real-time, not hindsight. This gives the episode higher doctrinal weight than derivative-teacher explanations.
