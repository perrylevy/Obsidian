---
type: timing
aliases: [Silver Bullet, Silver Bullet Windows, SB]
tags: [timing, session, silver-bullet]
---

# Silver Bullet Windows

Silver Bullet is a time-based intraday model that uses specific New York local-time windows rather than all-day discretion. The model is framed around recurring 60-minute opportunity windows that repeat every trading day ([[sources/2023-mentorship-silver-bullet]], [[sources/am-silver-bullet-strategy-on-nq]], [[sources/nq-pm-session-silver-bullet-august-26-2024]]).

## Core idea

The recurring windows are:

- London Silver Bullet: 3:00–4:00 a.m. NY
- AM Silver Bullet: 10:00–11:00 a.m. NY
- PM Silver Bullet: 2:00–3:00 p.m. NY

The 2022 mentorship Episode 3 provides the earliest ICT-direct source for these time preferences, defining the **optimal trading hours** as 8:30 AM – 11:00 AM (can extend to noon) and the **best afternoon setup** as 2:00 PM – 3:00 PM NY local time ([[sources/2022-ict-mentorship-episode-3]]). The Silver Bullet windows (10:00–11:00 AM and 2:00–3:00 PM) align precisely with these optimal periods. Episode 7 reinforces the **daily bias → intraday execution** sequence: daily bias is established pre-market (old high or old low target), and the Silver Bullet window is where the intraday MSS + FVG setup confirms and executes that bias ([[sources/2022-ict-mentorship-episode-7]]).

Within each window, the model looks for:

- a draw on liquidity,
- a sweep or raid of prior highs/lows or session liquidity,
- a confirming fair value gap / order block / breaker block setup,
- and a target on the opposite side of the relevant range.

A direct Forex example on 2025-01-27 uses the 10:00 AM Silver Bullet pocket to short a NWOG-based IFVG, with bodies staying in the lower half / at CE before the drop resolves into the next liquidity draw ([[sources/2025-lecture-series-smc-new-york-nwog-with-forex-01272025]] @ 6:25, @ 6:58, @ 10:52). Episode 8 confirms the Silver Bullet framework applies to **forex markets** (EUR/JPY example): the NY session 7:00–10:00 AM window is where the FVG setups form, and the same MSS + FVG sequence executes identically across asset classes ([[sources/2022-ict-mentorship-episode-8]]).

## Why it matters

Silver Bullet is one of the clearest examples of ICT-style time-and-price precision:

- the market does not need to trade all day,
- the same rule set repeats in fixed windows,
- and the setup is only valid when the time filter and liquidity logic align.

The January 27, 2025 GBP/USD NWOG lecture is a direct example of the 10:00 AM pocket in use: the NWOG / IFVG / CE stack is traded inside the Silver Bullet window, not outside it ([[sources/2025-lecture-series-smc-new-york-nwog-with-forex-01272025]]).

## Practical use

Use Silver Bullet as a timing filter, not a standalone trigger:

- if the window is not active, ignore the setup,
- if liquidity has not been taken, no trade,
- if confirmation does not appear, no trade,
- if the target does not offer enough framework, pass.

The 2022 mentorship Episode 5 provides the earliest ICT-direct **session structure** that contextualizes these windows within the full trading day: pre-market (before 8:30), morning (8:30–11:00), lunch (12:00–1:00, no-trade), afternoon (1:30–4:00), and close algorithm (3:50–4:00). The Silver Bullet windows (10:00–11:00 AM and 2:00–3:00 PM) align with the morning and afternoon sessions respectively ([[sources/2022-ict-mentorship-episode-5]]).

## See also

- [[timing/new-york-local-time]]
- [[timing/opening-range]]
- [[timing/first-hour-dealing-range]]
- [[concepts/fair-value-gap]]
- [[concepts/order-block]]
- [[concepts/breaker-block]]
- [[concepts/change-in-state-of-delivery]]
- [[concepts/market-structure-shift]]
- [[concepts/consequent-encroachment]]
