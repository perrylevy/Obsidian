---
type: synthesis
aliases: [Hermes Trading Analyst Model Stack, Model Selection Stack, Model Confluence Stack]
tags: [synthesis, models, NQ, playbook]
---

# How Hermes Trading Analyst Should Use the Model Stack

This wiki has enough model pages now that they should not be treated as nine equal competitors.

For Hermes-trading-analyst, the cleanest approach is:
1. choose the session window,
2. choose the delivery framework,
3. choose the execution family,
4. use the remaining pages only as supporting confluence.

## The stack

### 1. Session / timing filter first

Start with the session playbook, not the model list.

For the user's main workflow, the primary timing scaffold is:
- [[synthesis/how-to-trade-the-930-11am-window]]
- [[timing/opening-range]]
- [[timing/first-presented-fvg]]
- [[timing/macros]]

If the time window is wrong, model confluence will not rescue the trade idea.

### 2. Delivery framework second

Use one of these as the higher-order narrative:
- [[models/power-of-three]] — the default delivery lens for accumulation / manipulation / distribution.
- [[models/market-maker-buy-model]] or [[models/market-maker-sell-model]] — use when the chart looks like a larger swing-delivery round trip rather than a short intraday scalp.

In practice, the market-maker models are best treated as expanded bullish / bearish mirrors of the same delivery family, not as two separate everyday model choices.

### 3. Execution family third

Once timing and delivery agree, choose the entry family:

- [[models/first-presentation-model]] — default cash-open execution family for the user's 9:30–11:00 a.m. ET focus.
- [[models/silver-bullet]] — fixed time-window FVG execution family, especially 10:00–11:00 and later session windows.
- [[models/turtle-soup]] — liquidity-sweep reversal family.

These are the pages that should generate most actual trade candidates.

### 4. Supporting confluence last

These pages are still useful, but they should not usually be treated as standalone model calls:
- [[models/internal-external-liquidity-model]] — routing / target path framework.
- [[models/fractal-model]] — time-frame nesting and confirmation framework.
- [[deferred/models/confirmation-model]] — stacked confirmation checklist for a bias that already has HTF FVG / SMT / IFVG support.
- [[deferred/models/camerons-model]] — compact derivative heuristic for draw-on-liquidity + stop raid + FVG entry.

They refine a trade idea; they should not usually originate it.

## Canonical model hierarchy for this wiki

### Primary model families

1. [[models/power-of-three]] — delivery framework
2. [[models/first-presentation-model]] — default opening-session execution model
3. [[models/turtle-soup]] — default liquidity-sweep reversal model
4. [[models/silver-bullet]] — fixed-window continuation / entry model
5. [[models/market-maker-buy-model]] / [[models/market-maker-sell-model]] — larger swing-delivery family

### Supporting frameworks and variants

- [[models/internal-external-liquidity-model]]
- [[models/fractal-model]]
- [[deferred/models/camerons-model]]

## Practical default for Hermes-trading-analyst

If Hermes is reading price and charts to produce trade ideas, the default order should be:

1. Is the setup inside the correct window?
2. Is the market behaving like PO3 / larger delivery, or is it just noisy?
3. Is this an opening-session FVG setup, a Silver Bullet window, or a liquidity-sweep reversal?
4. Do IRL/ERL, fractal nesting, or Cameron-style stop-raid logic improve confidence?
5. If multiple families conflict, do not force a trade idea.

## Recommended simplification for decision-making

For day-to-day use, Hermes-trading-analyst should usually think in only four top-level buckets:

- opening-session FVG family
- liquidity-sweep reversal family
- fixed-window continuation family
- higher-time-frame delivery family

That is a much cleaner decision stack than asking the agent to choose among nine supposedly equal models every time.

## See also

- [[synthesis/how-to-trade-the-930-11am-window]]
- [[synthesis/how-to-use-first-presented-fvg]]
- [[synthesis/how-to-trade-turtle-soups]]
- [[models/power-of-three]]
- [[models/first-presentation-model]]
- [[models/turtle-soup]]
- [[models/silver-bullet]]
- [[models/market-maker-buy-model]]
- [[models/market-maker-sell-model]]
