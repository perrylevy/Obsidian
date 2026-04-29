---
type: instrument
aliases: [MNQ, Micro Nasdaq, Micro E-mini Nasdaq]
tags: [instrument, futures]
---

# MNQ

Micro E-mini Nasdaq-100 futures. Flagship instrument for this wiki. 1/10 the size of NQ; same price action.

## Contract facts

- **Product**: Micro E-mini Nasdaq-100 futures (CME Globex symbol: MNQ).
- **Underlying**: Nasdaq-100 index; tracks the same price action as [[instruments/NQ|NQ]] at 1/10 notional.
- **Tick size**: 0.25 index points.
- **Tick value**: $0.50 per tick (so 1 point = $2.00 per contract). NQ is 10× this: 1 point = $20.00 per NQ contract.
- **Contract months**: quarterly (March / June / September / December), like NQ.
- **Session (CME)**: Sunday 6:00 p.m. ET – Friday 5:00 p.m. ET, with a daily 5:00–6:00 p.m. ET break. Regular Trading Hours reference for the 9:30 a.m. open is New York local time.
- **Rollover**: second Thursday of the contract month (8 days before third-Friday expiry).

_These are static industry facts, not source-backed claims; they are stated here once so risk-per-contract questions resolve inside the wiki without external lookup._

## ICT doctrine applied to MNQ

ICT doctrine (FVG, Silver Bullet, PO3, Turtle Soup, liquidity sweeps) applies to **index futures** generally — the 10-handle / 40-tick minimum framework scopes to index futures as a category ([[sources/2023-mentorship-silver-bullet]] @ 0:22). No MNQ-only doctrine has been stated in ingested sources yet.

## Cross-instrument selection rule (SMT)

When trading [[concepts/smt|SMT]] divergence on the ES / NQ / YM trio, **enter on the divergent leg**. If NQ is the leg that refuses to confirm a sweep, NQ (and therefore MNQ) is the **preferred entry instrument** vs. ES or YM — because the algorithmic non-confirmation is happening on Nasdaq ([[sources/intro-smt-divergence]]). _Attribution: Fearing — derivative teacher relaying ICT material._

Conversely: if NQ **does** confirm the sweep and ES or YM diverges, defer the MNQ trade and take the divergent index instead. This rule directly governs whether MNQ is the right instrument on a given setup.

## Observed behavior (single observations)

Each entry here is a **single observation** — one trade or one session. Patterns require multiple observations before being treated as recurring MNQ behavior.

### 2025-02-13 — PM Silver Bullet, long

- Setup: [[models/silver-bullet|PM Silver Bullet]] window + 2:50–3:10 NY [[timing/macros|PM macro]] ([[sources/mnq-pm-silver-bullet-walkthrough]] @ 3:01).
- Entry FVG: 1m FVG nested inside upper half of 5m FVG; volume imbalance included in FVG boundary per the trader's rule ([[sources/mnq-pm-silver-bullet-walkthrough]] @ 0:36, @ 6:46).
- Draw on liquidity: buyside ~22,100 ([[sources/mnq-pm-silver-bullet-walkthrough]] @ 8:02).
- Outcome: -2 SD projection paid ~$1,000 on ~15 MNQ contracts, ~$350 risk ([[sources/mnq-pm-silver-bullet-walkthrough]] @ 30:59).
- Doctrine used: [[concepts/low-resistance-liquidity-run|low-resistance liquidity]] signatures — speed through highs, FVGs staying open, fluid one-directional delivery ([[sources/mnq-pm-silver-bullet-walkthrough]] @ 13:42).

**Pattern candidates to watch in future journal entries** (too early to call recurring):

- 1m-inside-5m FVG nesting as an MNQ PM SB edge.
- Reliable delivery of the 2:50–3:10 NY macro during PM SB on MNQ.
- HTF parent FVG midpoint holding when LTF FVG is overlapped ([[sources/mnq-pm-silver-bullet-walkthrough]] @ 15:22).

## See also

- [[instruments/NQ]] — parent contract, same price action
- [[models/silver-bullet]]
- [[concepts/fair-value-gap]]
- [[concepts/low-resistance-liquidity-run]]
- [[concepts/smt]]
- [[concepts/judas-swing]]
- [[index]]
