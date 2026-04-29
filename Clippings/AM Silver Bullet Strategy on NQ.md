---
title: "AM Silver Bullet Strategy on NQ"
source: "https://ttrades.com/the-am-silver-bullet-strategy-on-nq/"
author:
  - "[[TTrades]]"
published: 2025-06-19
created: 2026-04-15
description: "Learn the AM Silver Bullet strategy for NQ, including liquidity sweeps, entries, risk management, and FX Replay backtest results."
tags:
  - "clippings"
---
![](https://ttrades.com/wp-content/uploads/2026/01/ict-silver-bullet-thumbnail.png)

## at

## 11:00 am

This blog breaks down the New York AM Session Silver Bullet strategy on NQ, focusing on the 10 to 11 a.m. window.

![](https://ttrades.com/wp-content/uploads/2026/01/ict-silver-bullet-thumbnail.png)

#### Introduction

In this post, we’re breaking down the AM Silver Bullet strategy, focusing specifically on the 10:00 to 11:00 a.m. New York session and using NASDAQ (NQ / NAS100) as the ticker. We’ll walk through the model, the exact framework rules, and how entries are identified.

#### What the AM Silver Bullet Is

The Silver Bullet is a time based reversal model. Rather than trading all day, it narrows your focus to a very specific window where liquidity and volatility tend to align.

For this strategy, trading is restricted to the 10:00 to 11:00 a.m. New York time window. Trades are only considered after liquidity is taken, and all targets are set at the opposite side of the previous hour’s range. If those conditions are not met, no trade is taken.

[![](https://ttrades.com/wp-content/uploads/2025/06/Time-SB.png)](https://ttrades.com/wp-content/uploads/2025/06/Time-SB.png)

#### The Core Framework

Everything starts with the 9:00 a.m. hourly candle.

Once 10:00 a.m. hits, the high and low of the 9:00 a.m. candle are marked. This range becomes the framework for the session. Price must take one side of this range before a trade setup is even considered.

If price sweeps the 9:00 a.m. high, the focus shifts to shorts targeting the 9:00 a.m. low. If price sweeps the 9:00 a.m. low, the focus shifts to longs targeting the 9:00 a.m. high. Any setup that appears outside of the 10:00 to 11:00 a.m. window is ignored, regardless of how clean it looks.

[![](https://ttrades.com/wp-content/uploads/2025/06/framework.png)](https://ttrades.com/wp-content/uploads/2025/06/framework.png)

#### Entry Requirements

A sweep by itself is not enough. After liquidity is taken, confirmation is required before entering a trade.

Valid entry models include displacement back into the range, breaker blocks, order blocks, and fair value gaps used within structure. Stops are placed beyond the swing high or low that caused the displacement, and targets are always set at the opposite side of the 9:00 a.m. range.

[![](https://ttrades.com/wp-content/uploads/2025/06/Framework-1.png)](https://ttrades.com/wp-content/uploads/2025/06/Framework-1.png)

#### When There Is No Trade

Some sessions simply do not provide an opportunity.

If price does not sweep either side of the 9:00 a.m. range during the Silver Bullet window, no trade is taken.

#### Key Takeaways

The AM Silver Bullet is built around precision rather than frequency. Time discipline is non negotiable, liquidity sweeps and displacement are required, and risk to reward is what drives performance over time. The strategy is designed to participate only when specific conditions align, not to trade every move.

#### Final Thoughts

The AM Silver Bullet offers a clean and structured approach to intraday trading on NQ. While it does not produce trades every day, the consistency in framework and execution makes it well suited for traders who value patience and rules. A PM Silver Bullet session could be explored in the future, but the AM model stands solidly on its own.