---
type: concept
aliases: [PDC, Price Continuum Theory]
tags: [concept, delivery, liquidity]
---

# Price Delivery Continuum

Price Delivery Continuum is the doctrine that price should be read as a continuous cycling process across timeframes rather than as a one-shot top-down analysis. The trader keeps moving through HTF → LTF layers, looking for the algorithmic PD array that is currently active ([[sources/2025-price-delivery-continuum]] @ 12:33, @ 14:29, [[sources/mnq-pm-silver-bullet-walkthrough]] @ 15:22).

## Weekly-summary framing

The weekly-summary clip uses the same logic at a larger scale: a weekly holding pattern gives way once one side of the range is taken, the daily gap / volume-imbalance hybrid behaves like a balanced-price-range structure, and the week later resolves into inversion / continuation behavior. That makes the summary a good example of PDC at weekly scope ([[sources/2025-lecture-series-nq-weekly-summary-02282025]] @ 2:07, @ 3:39, @ 5:52, @ 31:59).

The 03/22/2025 timing-and-journaling lecture makes the same continuum explicit on the operator side: the chart should be cycled at each close, the active PD array should be logged with the current time window, and the model is only useful if the trader keeps repeating the scan across 60m / 15m / 5m / 1m layers ([[sources/2025-lecture-series-algorithmic-timing-and-journaling-03222025]] @ 9:16, @ 11:22, @ 12:33, @ 14:29).
The AM Trades weekly-narrative clip extends that same continuum into a full trading week: economic-calendar screening sets the days to watch, the daily chart sets the current phase of price delivery, and the weekly profile decides whether the market is likely to trend, reverse, or stay congested ([[sources/am-trades-blending-the-economic-calendar-daily-chart-weekly-profiles]] @ 4:04, @ 5:08, @ 12:23, @ 15:32).
The "Secret To ICT Daily Bias" clip pushes the same doctrine into a mechanical top-down routine: prior-quarter market profile, quarterly shift, premium/discount, and liquidity lookbacks decide the favored side before any lower-time-frame entry is considered ([[sources/the-secret-to-ict-daily-bias-a-mechanical-approach]] @ 0:33, @ 1:25, @ 3:00, @ 5:52, @ 19:21).
## Core idea

The model’s working assumptions are:

- time and OHLC are the primary inputs,
- the market keeps cycling across timeframes,
- and a parent higher-timeframe inefficiency can dominate a smaller lower-timeframe one.

## Why it matters

PDC is the umbrella that ties together:

- [[concepts/fair-value-gap|FVG]] behavior,
- [[concepts/balanced-price-range|balanced price range]] logic,
- institutional-orderflow entry drill behavior around reclaimed FVG / CE failure,
- and the low-resistance / high-resistance delivery split.

It explains why a lower-timeframe gap can still be subordinate to a higher-timeframe parent gap.

## Practical use

When a setup is forming, keep cycling the chart hierarchy:

- identify the higher-timeframe draw,
- drop down for the active delivery leg,
- then check whether the active lower-timeframe feature is nested inside a stronger parent structure.

If the parent level is still holding, treat the smaller setup as contextual rather than absolute.

A practical example is the institutional-orderflow entry-drill behavior: once a bullish FVG is reclaimed, failure to trade back down to CE shows that the parent delivery remains dominant and that the midpoint is being defended rather than neutralized ([[sources/2025-price-delivery-continuum]] @ 04:38, @ 06:36).

## See also

- [[synthesis/how-to-use-price-delivery-continuum]]
- [[concepts/fair-value-gap]]
- [[concepts/balanced-price-range]]
- [[concepts/low-resistance-liquidity]]
- [[concepts/high-resistance-liquidity-run]]
- [[concepts/draw-on-liquidity]]
