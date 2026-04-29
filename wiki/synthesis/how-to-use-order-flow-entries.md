---
type: synthesis
aliases: [Order Flow Entry Playbook, Orderflow Entries Playbook, FVG Entry Playbook]
tags: [synthesis, playbook, entries, order-flow]
---

# How to Use Order Flow Entries

This page is the operator guide for the **entries using order flow** source. The practical rule is that entries are the easy part only after higher-time-frame context, session timing, and the fair value gap family have already set up the move ([[sources/entries-using-order-flow]] @ 1:34, @ 2:29, @ 5:13).

## Core idea

The source reduces execution to two families:
- sharp turns, and
- lower-time-frame orderflow lags.

Both are just ways of expressing where an FVG-based entry becomes tradable inside a larger context area.

In cleanup terms, this page now absorbs several low-level labels that were creating terminology sprawl: **sharp turn**, **orderflow lag**, **continuation entry**, and **order-flow sweep** are treated as operator-language variants inside one order-flow-entry family rather than as separate top-level doctrines.

The August 28, 2024 speed clip adds a useful continuation check: once the draw is already established, the market should show immediate speed through intermediate highs/lows after a retracement into an FVG, order block, or breakaway gap. If the gap or retracement just stalls, the move is not behaving like a clean continuation.

## How to read the setup

### 1. Define the context area first

Start on the higher time frame and identify the area where the market is expected to react. The source explicitly says entries are easier once daily / weekly / monthly context is known.

### 2. Decide whether this is a sharp turn or an orderflow lag

A sharp turn is the cleaner "FVG in, FVG out" style reaction inside context. An orderflow entry is the lower-time-frame continuation / lag version, usually based on stacked FVGs or a directional imbalance that is already in motion.

### 3. Check the time window

The source stresses New York local time and volatility windows. The same chart setup can be far better or far worse depending on whether the market is inside an active killzone / news window.

### 4. Use the fair value gap family as the trigger family

The source's main claim is that entries are all about fair value gaps. That means the question is not whether there is a random candle pattern; the question is whether the FVG is being used as a valid reaction / continuation structure inside the correct context.

### 5. Keep the risk small

The lesson closes by emphasizing baseline entries, small risk, and stopping after one trade unless the data justifies more. That is part of the method, not just a side note.

## Practical execution map

### A. Sharp-turn entry

Use when:
- higher-time-frame context is clear,
- price reaches the context area,
- and the chart gives an FVG in / FVG out style reversal.

This is the cleaner of the two families.

### B. Orderflow-lag entry

Use when:
- the move is already underway,
- the lower time frame is producing stacked FVGs / lags,
- and you are entering with the direction rather than fading it.

### C. Do not force an entry outside the window

If the time-of-day context is wrong, a good-looking chart setup can still fail. The source makes timing part of the entry logic, not an afterthought.

## What to avoid

- Do not start with the entry before the higher-time-frame context.
- Do not trade an FVG without knowing whether it is a sharp turn or a lag.
- Do not ignore NY local time and volatility windows.
- Do not overtrade once one clean baseline entry has already worked.

## Fast checklist

Before entering, ask:
1. Is the higher-time-frame context defined?
2. Is this a sharp turn or an orderflow lag?
3. Is the FVG acting as trigger structure?
4. Is the time window active?
5. Is the risk sized conservatively enough?

## See also

- [[concepts/fair-value-gap]]
- [[concepts/time-frame-alignment]]
- [[deferred/timing/killzones]]
- [[timing/macros]]
- [[timing/new-york-local-time]]
- [[concepts/liquidity]]
- [[concepts/order-block]]
- [[sources/when-do-i-expect-speed-in-my-trades-advanced-order-flow-teaching-ict-concepts]]
- [[sources/entries-using-order-flow]]
