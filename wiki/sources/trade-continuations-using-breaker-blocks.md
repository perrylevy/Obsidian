---
type: source
title: "Trade Continuations Using Breaker Blocks"
source_type: youtube
raw: "[[Clippings/Trade Continuations Using Breaker Blocks.md]]"
date_ingested: 2026-04-22
key_concepts:
  - breaker-block
  - continuation-entry
  - change-in-state-of-delivery
  - fair-value-gap
  - smt
tags: [source, breaker-block, continuation, cisd, fvg, smt, execution]
aliases: ["Trade Continuations Using Breaker Blocks"]
---

# Trade Continuations Using Breaker Blocks

This clip translates the breaker-block reversal idea into a continuation framework: do not chase the first turn, wait for the market to prove the shift, then use the next clean retest to join the move.

The sequence is sweep -> close through the level -> breaker formation -> retest entry. If the sweep is missing, the clip allows an SMT exception: the unbroken low/high can be treated as protected when the correlated market confirms the divergence and the continuation still aligns with the higher-time-frame narrative.

When a textbook breaker does not form, the clip falls back to a fair-value-gap / intermediate-term swing framing. The message stays the same: let the market prove the change in delivery first, then use the retest as the continuation entry rather than guessing the turn.

## See also

- [[concepts/breaker-block]]
- [[synthesis/how-to-use-order-flow-entries]]
- [[concepts/change-in-state-of-delivery]]
- [[concepts/fair-value-gap]]
- [[concepts/smt]]
