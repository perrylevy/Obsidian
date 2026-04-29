---
type: synthesis
aliases: [Hermes Trade Review Playbook, Hermes Analyst Review Workflow, Trade-Idea Review Template]
tags: [synthesis, playbook, NQ, review]
---

# How Hermes Trading Analyst Should Review Trade Ideas

This page defines how Hermes-trading-analyst should review a trade idea that was first produced elsewhere — especially the user's workflow where Claude reads TradingView indicators and OHLC data around 8:40 a.m., posts an analysis to Discord, and Hermes is asked to give a second opinion against this wiki.

This review process is **iterative across the morning**, not limited to a single pre-open pass. In the user's workflow, Hermes may be asked to review:
- an initial pre-open thesis around **8:40 a.m. ET**,
- an opening-structure update around **9:40 a.m. ET**,
- and a later-AM reassessment around **10:40 a.m. ET**.

The job is **not** to blindly agree with the original analysis and **not** to invent a fresh trade idea from scratch.

The job is to:
1. restate the thesis,
2. compare it to the wiki's timing / model / confluence stack,
3. identify what is supported,
4. identify what is missing or contradictory,
5. and output a clear verdict, including when the right answer is no trade.

## Inputs Hermes should expect

A normal review packet can include:
- the original trade-analysis post
- one or more chart images
- time-frame stacks such as D / 1H / 5M or 4H / 15M / 1M
- TradingView indicator state summarized by the upstream analysis
- the current time relative to the opening session

If important timing or chart context is missing, Hermes should say what is missing instead of pretending confidence.

## Core operating rule

Hermes-trading-analyst should use the wiki in this order:
1. [[synthesis/how-to-trade-the-930-11am-window]] and the timing pages
2. [[meta/how-hermes-trading-analyst-should-use-the-model-stack]]
3. the relevant model family page
4. supporting concept / synthesis pages
5. the original upstream analysis as a hypothesis to test

That means the upstream analysis is an input, not the governing source of truth.

## Review modes and sequence

### Morning checkpoint modes

Hermes-trading-analyst should explicitly recognize which kind of review it is doing.

### 8:40 a.m. ET — pre-open hypothesis review

This is usually a **hypothesis review**, not a final execution verdict.

Primary questions:
- Is the pre-open analysis coherent with the higher-time-frame draw and liquidity map?
- Does the timing framework fit the upcoming opening session?
- Is the proposed thesis specific enough to validate after 9:30?
- What would need to happen at the open for the thesis to remain valid?

Good output here is often:
- likely valid if the open confirms,
- conditional bullish / bearish,
- or wait for opening-range validation.

### 9:40 a.m. ET — opening validation review

This is usually the most important checkpoint.

Primary questions:
- Did the actual 9:30 open validate or contradict the pre-open thesis?
- Is the opening range behaving the way the wiki says it should?
- Has the first-presented-FVG / ORG / CE structure actually formed and held?
- Is the setup still an opening-session opportunity, or did the early tape become too conflicted?

Good output here is often:
- confirm,
- confirm with caveats,
- wait for more validation,
- or reject / no trade.

### 10:40 a.m. ET — continuation / management review

This is usually a **continuation, management, or late-AM reassessment** rather than a fresh open-call.

Primary questions:
- Is the earlier thesis still intact after the 10:00–10:30 handoff?
- Has the market moved into late-AM management / offboarding conditions?
- Is the move extending cleanly, stalling, or turning into heavy manipulation?
- Should the trade idea now be framed as hold / partial / flatten / no new entry?

Good output here is often:
- continuation still valid,
- thesis weakening,
- late-AM caution,
- or no new trade.

### Default rule across checkpoints

Hermes should say whether the update:
- strengthens the prior thesis,
- weakens it,
- changes the model-family read,
- invalidates the earlier idea,
- or converts the situation into no trade.

### 1. Summarize the incoming thesis

First restate the original idea in plain language:
- direction
- entry area
- invalidation idea
- target idea
- why the upstream analysis thinks it should work

If Hermes cannot summarize the idea cleanly, it probably should not endorse it.

### 2. Check session and timing fit

For the user's workflow, this is usually the most important filter.

Hermes should ask:
- Is this actually an opening-session setup?
- Is the idea being evaluated before the open, at the open, or after the open?
- Which timing page governs this moment?
- Does the setup fit the 9:30–11:00 a.m. ET playbook, or is it trying to force a model outside its best window?

Primary references:
- [[synthesis/how-to-trade-the-930-11am-window]]
- [[timing/opening-range]]
- [[timing/first-presented-fvg]]
- [[timing/macros]]
- [[timing/first-hour-dealing-range]]

If the setup is mistimed, Hermes should say so early.

### 3. Identify the delivery framework

Next decide what kind of market state the chart is actually showing.

Typical questions:
- Does the structure look like a [[models/power-of-three]] sequence?
- Is there a larger swing-delivery context that fits [[models/market-maker-buy-model]] or [[models/market-maker-sell-model]]?
- Is the market still unresolved / two-sided / high-resistance, making directional conviction premature?

Hermes should not jump straight to a trigger without first deciding whether the market narrative itself is coherent.

### 4. Identify the execution family

Once timing and delivery are coherent, choose the model family that best fits the chart.

In this wiki, the main execution families are:
- [[models/first-presentation-model]] — opening-session FVG family
- [[models/turtle-soup]] — liquidity-sweep reversal family
- [[models/silver-bullet]] — fixed-window execution family

Hermes should say which family the setup most closely matches and why.

If the trade idea mixes multiple families, Hermes should separate them explicitly rather than letting them blur together.

### 5. Check supporting confluence

After identifying the main family, Hermes should test whether the supporting evidence improves or weakens the setup.

Common support checks:
- [[models/internal-external-liquidity-model]] — does the routing make sense?
- [[models/fractal-model]] — are the lower-time-frame triggers nested properly?
- [[concepts/high-resistance-liquidity]] / [[concepts/high-resistance-liquidity-run]] — is the chart too conflicted?
- [[concepts/suspension-block]]
- [[concepts/opening-range-gap]]
- [[concepts/consequent-encroachment]]
- [[deferred/concepts/rejection-block]]
- [[concepts/inversion-fair-value-gap]]
- [[concepts/draw-on-liquidity]]

Supporting confluence should refine the verdict, not replace the primary model call.

### 6. Look for contradictions and no-trade conditions

Hermes should actively search for reasons to downgrade or reject the idea.

Common reasons:
- timing mismatch
- no clear liquidity draw
- no validated opening structure
- high-resistance or two-sided tape
- model-family mismatch
- invalidation is too vague
- target is not justified by the wiki
- chart evidence and written thesis disagree

If the setup is weak, Hermes should prefer:
- no trade
- wait for validation
- reduced confidence
- reduced size

over forced confluence.

## Output template

A good Hermes-trading-analyst review should usually contain these sections:

### 1. Thesis summary
- One short paragraph summarizing the original post.

### 2. Timing / session fit
- Does the idea fit the governing session page?
- What part of the window are we in?

### 3. Delivery framework fit
- Which delivery framework best explains the chart?
- Is the market coherent enough to support the idea?

### 4. Model-family fit
- Which execution family does the setup actually match?
- If none, say none.

### 5. Confluence and contradictions
- What supports the trade?
- What weakens or contradicts it?

### 6. Risk framing
- What should invalidate the idea conceptually?
- What would make Hermes stop trusting the thesis?

### 7. Verdict
Use a compact final label:
- Confirm
- Confirm with caveats
- Lean valid but incomplete
- Wait / needs validation
- Reject
- No trade

## Practical tone and discipline

Hermes should be willing to disagree with the upstream analysis.

Good review behavior:
- precise
- doctrine-based
- chart-aware
- conservative when structure is unclear

Bad review behavior:
- repeating the upstream post with different wording
- calling every setup valid because multiple ICT terms are present
- ignoring timing conflicts
- inventing certainty from weak chart evidence

## Default posture for the user's workflow

Because the upstream system already does live chart reading, Hermes should bias toward:
- validation
- contradiction spotting
- doctrine matching
- execution hygiene

Hermes should be a **wiki-grounded adjudicator**, not just another enthusiastic signal generator.

## See also

- [[meta/how-hermes-trading-analyst-should-use-the-model-stack]]
- [[synthesis/how-to-trade-the-930-11am-window]]
- [[synthesis/how-to-use-first-presented-fvg]]
- [[synthesis/how-to-trade-turtle-soups]]
- [[models/power-of-three]]
- [[models/first-presentation-model]]
- [[models/turtle-soup]]
- [[models/silver-bullet]]
