---
type: index
---

# Wiki Index

Catalog of wiki pages. Updated at the end of each ingest batch.

**Legend**: `⭐` = flagship page · `(N)` = number of ingested sources citing this concept · `_pending_` = concept has been captured in source pages but no dedicated wiki page exists yet — see the source pages in the meantime.

---

## Intraday setup index (start here for live NQ / MNQ reads)

Top-level entry point for live tape work. Each row: model, active window, manipulation cue, entry array, stop reference.

- **[[synthesis/intraday-nq-mnq-playbook]]** ⭐ — full end-to-end operator checklist (HTF → session → window → model → entry → stop → target → invalidation → instrument → journal).
- [[models/power-of-three]] · session/day/week · Judas swing · FVG/OB from Distribution displacement · stop beyond Manipulation extreme.
- [[models/silver-bullet]] · 10–11 AM / 2–3 PM NY · sweep into draw inside window · displacement FVG (1m nested in 5m) · stop beyond sweep or 5m parent.
- [[models/turtle-soup]] · Asian-range / session high-low raid · sweep + SFP close back · IFVG or candle-close entry · stop above/below working candle of the sweep.
- [[models/first-presentation-model]] · opening range · first displacement after cash open · first valid FVG in opening range · stop beyond first-presentation swing.
- [[models/market-maker-buy-model]] · HTF accumulation · sweep into discount · discount FVG / breaker / OB · stop below accumulation low or SMR low.
- [[models/market-maker-sell-model]] · HTF distribution · role-flipped PD array · premium FVG / breaker rejecting array · stop above distribution high or flipped array.
- [[models/internal-external-liquidity-model]] · killzone · external-liquidity raid · FVG inside internal-liquidity zone after [[concepts/market-structure-shift|MSS]] · stop beyond raided wick.
- [[models/fractal-model]] · nested HTF→LTF · LTF sweep confirming HTF · IFVG / displacement FVG on LTF · stop beyond sweeping-candle extreme.

See each model page's **Risk & stop placement** section for the full entry/stop/target specification.

---

## Instruments

- [[instruments/MNQ]] ⭐ — ICT doctrine + observed MNQ trades; SMT-based NQ entry rule (2)
- [[instruments/NQ]] — parent Nasdaq futures contract; recurring review instrument for 2025 lecture-series clips (5)

## Models

Use these as a hierarchy, not nine equal choices. Start with [[meta/how-hermes-trading-analyst-should-use-the-model-stack]].

### Primary execution families

- [[models/first-presentation-model]] — default opening-session execution model for the user's 9:30–11:00 ET workflow (2)
- [[models/turtle-soup]] — default liquidity-sweep reversal model; Asian-range variant and SFP equivalence noted (8)
- [[models/silver-bullet]] — fixed time-window FVG execution model, especially 10:00–11:00 and later session windows (2)
- [[models/unicorn-model]] — high-confluence daily-bias + killzone + MSS + OB/FVG stack

### Delivery frameworks

- [[models/power-of-three]] — canonical accumulation / manipulation / distribution delivery scaffold (10)
- [[models/market-maker-buy-model]] — bullish swing-delivery round-trip; best treated as a larger HTF framework, not an everyday scalp trigger (5)
- [[models/market-maker-sell-model]] — bearish mirror of the market-maker buy-model family (5)

### Supporting frameworks

- [[models/internal-external-liquidity-model]] — liquidity-routing framework; strongest as confluence rather than a standalone trigger (1)
- [[models/fractal-model]] — HTF/LTF nesting framework for IFVG / sweep-and-invert structure (1)

Lower-weight model variants were moved out of the main doctrine lane; see [[deferred/index]].

## Concepts — PD arrays & inefficiencies

- [[concepts/pd-array]] — hub; the matrix that selects which array the algorithm uses (5)
- [[concepts/fair-value-gap]] — the flagship PD array (37)
- [[timing/first-presented-fvg]] — canonical home for first-presented-FVG variants, including the Monday carry-forward use case (11)
- [[concepts/inversion-fair-value-gap]] — polarity flip; live-tape entry variants (19)
- [[concepts/suspension-block]] — candle body suspended between an upper and lower volume imbalance; ICT-specific PD array (promoted from deferred after the September 30, 2025 public definition)
- [[concepts/consequent-encroachment]] — midpoint of an FVG (17)
- [[concepts/mean-threshold]] — midpoint of an OB (1)
- [[concepts/order-block]] — strict definition; composite range; three-part trade-entry filter; bullish-OB upper-portion rule; stop-loss placement (23)
- [[concepts/dealing-range]] — both-sides-swept range; DRT 25 / 50 / 75 grading (2)
- [[concepts/volume-imbalance]] — body-to-body gap; weaker than FVG (10)
- [[concepts/balanced-price-range]] — efficient half of an FVG; BPR / worked half (2)
- [[concepts/breaker-block]] — violated OB / structure reused in the opposite direction (5)
- [[concepts/breakaway-gap]] — first FVG of a new leg; immediate-rejection rule (6)
- [[concepts/immediate-rebalance]] — rapid same-session repricing to a booked level / gap (2)
- [[concepts/measuring-gap]] — midpoint / 50 DRT gap inside the dealing range (1)

Source-specific or lower-weight PD-array variants were moved out of the main doctrine lane; see [[deferred/index]].

## Concepts — Liquidity

- [[concepts/liquidity]] — hub page; ERL / IRL taxonomy (12)
- [[concepts/draw-on-liquidity]] — DOL = next pool the algorithm targets (28)
- [[concepts/liquidity-void]] — empty price zone / gap pocket that can later rebalance (1)
- [[concepts/buyside-liquidity]] — resting buy-stops above swing highs; breakout buys + short stop-losses (3)
- [[concepts/sellside-liquidity]] — resting sell-stops below swing lows; breakout sells + long stop-losses (3)
- [[concepts/internal-liquidity]] — in-range liquidity / imbalance inside the dealing range (3)
- [[concepts/external-liquidity]] — swing highs/lows at the range edges; ERL boundary liquidity (3)
- [[concepts/liquidity-sweep]] — canonical home for stop raids, sweep/reject events, and SFP-style reversals (7)
- [[concepts/low-resistance-liquidity-run]] — fluid run targeting unsweep liquidity (4)
- [[concepts/high-resistance-liquidity-run]] — choppy run targeting post-sweep liquidity (5)
- [[concepts/high-resistance-liquidity]] — already-swept side of the resistance-liquidity curve (3)
- [[concepts/low-resistance-liquidity]] — unswept failure-swing target side; clean draw (2)
- [[concepts/relative-equal-highs-lows]] — mirrored smooth-side liquidity clusters; canonical home for equal-high / equal-low variants
- [[concepts/failure-swing]] — swing that aborts before reaching its target (1)

Niche liquidity subtypes and protective edge-case labels now live in [[deferred/index]].

## Concepts — Structure & orderflow

- [[concepts/smt]] — Smart Money Tool; ES/NQ/YM divergence (11)
- [[concepts/judas-swing]] — bias-counter spike at session open / 8:30 (5)
- [[concepts/smart-money-reversal]] — apex of MM model curve (2)
- [[concepts/market-structure-shift]] — structure confirms the directional thesis after the sweep / raid (18)
- [[concepts/displacement]] — aggressive full-bodied delivery that validates sweeps and leaves behind FVGs / OBs
- [[concepts/change-in-state-of-delivery]] — precise order-block delivery-change level (11)
- [[concepts/discount-premium]] — upper/lower half of a reference range (9)
- [[concepts/premium-discount]] — the 50% midpoint matrix for target selection and PD array grading (2)
- [[synthesis/how-to-use-order-flow-entries]] — canonical home for sharp-turn, orderflow-lag, and continuation-entry execution variants
- [[concepts/candle-science]] — canonical home for candle-level sweep logic, previous-candle high/low, and candle-behavior heuristics (3)
- [[concepts/candle-range-theory]] — single-candle high-to-low range read (1)

Additional edge-case structure labels were moved out of the main doctrine lane; see [[deferred/index]].

## Concepts — Opening gaps

- [[concepts/new-week-opening-gap]] — weekly gap that repeatedly acts as a draw and retest level (10)
- [[concepts/new-day-opening-gap]] — session opening gap between prior settlement and the new open (6)
- [[concepts/opening-range-gap]] — RTH opening gap between prior settlement and the 9:30 open; first-session frame (6)

Secondary opening-gap abstractions now live in [[deferred/index]].

## Concepts — Other

- [[concepts/optimal-trade-entry]] — legacy Fibonacci-style entry concept; dethroned by FVG (2)
- [[concepts/price-delivery-continuum]] — cyclical HTF-to-LTF reading of active algorithmic delivery (4)
- [[concepts/daily-bias]] — directional thesis: will price draw to old high or old low? Maintain bias until target is reached (8)
- [[concepts/opening-range]] — the span from open to high (bearish) or open to low (bullish); defines where premium/discount arrays form (1)
- [[concepts/daily-profile]] — session-profile filter for seek-and-destroy and New York reversal days (7)
- [[models/power-of-three]] — canonical home for accumulation / manipulation / distribution delivery phases (9)
- [[concepts/rule-adherence]] — following a trading system exactly as written instead of improvising (6)
- [[concepts/trading-consistency]] — staying with one system long enough for edge to compound (9)
- [[concepts/money-psychology]] — beliefs about money, status, safety, and control under live risk (9)
- [[concepts/self-sabotage]] — destructive trading behavior used to cope with anxiety or drawdown (6)
- [[concepts/protected-highs-lows]] — SMT-backed stop-placement rule for avoiding obvious wick stops (3)
- [[concepts/weekly-open]] — weekly accumulation reference around the weekly open (1)

Lower-priority psychology and edge-case operator concepts now live in [[deferred/index]].

## Timing

- [[timing/silver-bullet-windows]] — three 60-minute NY windows (1)
- [[timing/macros]] — ~20-minute pulses; time-side of time+price agreement (17)
- [[timing/lunch-macro]] — 11:30–1:30 midday macro / lunch-hour execution window (5)
- [[timing/new-york-local-time]] — all ICT timing in NY local + DST (6)
- [[concepts/candle-science]] — canonical home for candle-behavior heuristics and wick-based candle timing reads (2)
- [[timing/time-distortion]] — range compression / higher-time-frame fulfillment state (4)
- [[timing/asian-range]] — Asian session high/low bias scaffold; derivative routines often trade it in the first 30 minutes of each hour from 7:00–11:00 ET (3)
- [[timing/first-presented-fvg]] — first 1-minute FVG at the session open / impulse (11)
- [[timing/opening-range]] — first structured range after the session open; links OR, NDOG, and first-presented FVG (4)
- [[timing/first-hour-dealing-range]] — canonical home for the 9:30–10:30 first-hour frame (3)
- [[timing/no-initial-bias]] — wait for the first hour when bias is unclear at the open (7)
- [[timing/nightly-premarket-bias]] — pre-open bias scaffold built from previous candle close / range failure
- [[synthesis/how-to-build-daily-bias]] — parent map tying together profile, premarket, no-initial-bias, and open validation
- [[synthesis/how-to-map-ict-session-timing]] — parent timing map for sessions, macros, SB, CRT, and first-presented-FVG
- [[synthesis/how-to-trade-when-you-dont-have-an-initial-bias]] — operator guide for the no-initial-bias opening-state workflow
- [[timing/fomc]] — high-impact Fed event that often defines the weekly inflection (2)
- [[concepts/time-frame-alignment]] — HTF context must contain the LTF entry (11)

Umbrella or under-sourced timing labels now live in [[deferred/index]].

## Feedback

- [[feedback/live-execution-feedback]] — live execution feedback log for Hermes-generated trade ideas measured against MNQ delivery

## Sources

### Direct ICT
- [[sources/2023-mentorship-silver-bullet]] — ICT 2023 Mentorship: Silver Bullet Time-Based Trading Model
- [[sources/2025-lecture-series-keys-to-success-in-troubled-markets-june-16-2025]] — Keys To Success In Troubled Markets; time distortion, CE, MSS, relative equal highs, and PD-array grading
- [[sources/2022-ict-mentorship-no-rant-expectations]] — 2022 ICT Mentorship [No Rant] - Expectations; futures index focus, ES / YM / NQ contrast, and framework-first guidance
- [[sources/2022-ict-mentorship-episode-2]] — 2022 ICT Mentorship Episode 2 - Elements To A Trade Setup; foundational framework: weekly bias, liquidity, market structure break, FVG, premium/discount matrix, and live account executions
- [[sources/2022-ict-mentorship-episode-3]] — 2022 ICT Mentorship Episode 3 - Internal Range Liquidity & Market Structure Shifts; canonical killzone boundaries (London 2:00–5:00 AM, NY 7:00–10:00 AM), MSS vs break distinction, IRL definition, order block as "change in state of delivery," and multiple-FVG strategy
- [[sources/2022-ict-mentorship-episode-4]] — 2022 ICT Mentorship Episode 4 - Practical Trading Examples; live ES and NQ executions demonstrating the MSS + FVG + equilibrium target sequence, pattern recognition training, and study journal discipline
- [[sources/2022-ict-mentorship-episode-5]] — 2022 ICT Mentorship Episode 5 - Intraday Order Flow & Daily Range; session structure (pre-market / morning / lunch / afternoon / close), displacement concept, three drives pattern, swing high/low liquidity, measured move, and two core entry patterns
- [[sources/2022-ict-mentorship-episode-6]] — 2022 ICT Mentorship Episode 6 - Market Efficiency Paradigm & Institutional Order Flow; the most detailed early ICT-direct FVG three-candle formation, MSS pattern that forms every day, timeframe drilldown (15m→1m), smart money vs retail paradigm, and 8:30 employment data live NQ example
- [[sources/2022-ict-mentorship-episode-7]] — 2022 ICT Mentorship Episode 7 - Daily Bias & Consolidation Hurdles; earliest ICT-direct daily bias framework (old high vs old low), consolidation hurdle strategy (surgical strikes), intermarket correlation (three averages: Dow/NASDAQ/S&P 500), risk management by bias (3.5–4.5% with bias, 0.5–1% against), leader trades, and live NQ execution example
- [[sources/2022-ict-mentorship-episode-8]] — 2022 ICT Mentorship Episode 8 - Applying Institutional Order Flow To Forex Markets; earliest ICT-direct forex application, EUR/JPY live example with top-down analysis (daily→1m), component currency analysis for exotic crosses, killzone boundaries restated (London 2–5 AM, NY 7–10 AM), and Fibonacci target projection
- [[sources/2022-ict-mentorship-episode-9]] — 2022 ICT Mentorship Episode 9 - Power Of 3 & New York PM Session Opportunities; earliest ICT-direct Power of 3 explanation (accumulation→manipulation→distribution), Judas swing concept, PM session execution strategy (2:00 PM onward), avoid-morning-after-overnight-run rule, order block identification (consecutive down-closed candles + imbalance), limit order discipline, and live NQ example (Feb 14–15, 2022)
- [[sources/2022-ict-mentorship-episode-10]] — 2022 ICT Mentorship Episode 10 - Implementing Economic Calendar Events With The Open; economic calendar awareness (forexfactory.com, 8:30 AM news embargo), daily bias refinement, opening range concept (premium array placement), 15-minute chart as bellwether, timeframe drilldown (5m→1m), risk management ($15K+ minimum for NQ), and paper trading discipline
- [[sources/2022-ict-mentorship-episode-11]] — 2022 ICT Mentorship Episode 11 - Overcoming Mental Hurdles & Knowing When Enough Is Enough; Larry Williams swing high/low halo classification (single/double/triple), nesting effect for directional bias, live NQ short execution (246 handles), dopamine trap after big wins, push-edge-vs-sharpen-edge psychology, and demo trading as release valve
- [[sources/2022-ict-mentorship-episode-12]] — 2022 ICT Mentorship Episode 12 - Advanced Market Structure; three core pre-trade questions, market structure hierarchy (long-term/intermediate-term/short-term), intermediate-term highs defined by rebalancing, order block refined definition (consecutive series with imbalance, NOT "last candle"), directional candle resistance/support rules, daily chart primacy, and Fibonacci targeting levels
- [[sources/2022-ict-mentorship-episode-13]] — 2022 ICT Mentorship Episode 13 - Precision Price Action Execution & Risk Management; three-part OB trade-entry filter (gap + candle + liquidity narrative), pyramid position sizing (3-2-1 stable), stop-loss placement below OB low, demo trading prerequisites (6-month minimum), monthly 20% percentage-based goal, 1992 cautionary tale, and live pyramided NQ execution
- [[sources/2022-ict-mentorship-episode-14]] — 2022 ICT Mentorship Episode 14 - MSS + FVG Long Execution Example; upside MSS, Friday-close gap fill, buyside liquidity target, and retail-resistance contrast
- [[sources/2022-ict-mentorship-episode-15]] — 2022 ICT Mentorship Episode 15 - Live Equity Account Execution Example; bullish bias, swing high breakout, FVG entry at 680/630, sell-stop risk management, ~20% monthly target, and live-account proof
- [[sources/2022-ict-mentorship-episode-16]] — 2022 ICT Mentorship Episode 16 - Multiple Setups Per Session & Using Higher Timeframe Analysis; daily-chart primacy, multiple intraday setups, relative equal highs/lows, opening-price anchors, stacked FVGs, and Fibonacci projection
- [[sources/2022-ict-mentorship-episode-17]] — 2022 ICT Mentorship Episode 17 - Forex Application With This Mentorship Model; institutional round-number levels, New York Open Kill Zone timing, midnight vs 8:30 opening-price logic, EURUSD daily-chart application, and market-structure-shift context
- [[sources/2022-ict-mentorship-episode-18]] — 2022 ICT Mentorship Episode 18 - Step By Step Approach To Using This Model In Forex & Additional Insights Into Order Block Theory; daily bias, prior-day liquidity, time-frame hierarchy, killzone discipline, and tightened order-block theory
- [[sources/2022-ict-mentorship-episode-19]] — 2022 ICT Mentorship Episode 19 - Order Blocks, Judas Swing & Power of 3; order blocks as delivery change, Judas swing as the counter-move, and PO3 as the broader scaffold
- [[sources/2022-ict-mentorship-episode-22]] — 2022 ICT Mentorship Episode 22 - ICT SMT Divergence; SMT divergence on ES vs NQ, bearish daily order block, relative equal lows, imbalance/FVG behavior, premium-discount framing, and PO3 structure
- [[sources/2022-ict-mentorship-episode-34-using-the-sunday-gap-opening]] — 2022 ICT Mentorship Episode 34 - Using The Sunday Gap Opening; Sunday gap as a week-long dynamic support/resistance scaffold with FVG, OB, SMT, and relative-equal-high/low context
- [[sources/2025-price-delivery-continuum]] — ICT 2025 Lecture Series: Algorithmic Price Delivery Continuum
- [[sources/2025-lecture-series-making-money-with-smc-concepts]] — ICT 2025 Lecture Series: Making Money With SMC Concepts
- [[sources/2024-mentorship-lecture-1]] — ICT 2024 Mentorship: Lecture 1
- [[sources/2024-mentorship-lecture-3]] — ICT 2024 Mentorship: Lecture 3
- [[sources/2024-mentorship-lecture-4]] — ICT 2024 Mentorship: Lecture 4
- [[sources/2024-mentorship-lecture-5]] — ICT 2024 Mentorship: Lecture 5
- [[sources/2024-mentorship-lecture-6]] — ICT 2024 Mentorship: Lecture 6 (August 12, 2024; pre-CPI/PPI layered liquidity and inversion-FVG invitation framing)
- [[sources/2024-mentorship-lecture-12]] — ICT 2024 Mentorship: Lecture 12
- [[sources/2024-mentorship-lecture-14]] — ICT 2024 Mentorship: Lecture 14 (title-card / no usable transcript)
- [[sources/2024-mentorship-lecture-16]] — ICT 2024 Mentorship: Lecture 16
- [[sources/2024-mentorship-lecture-21]] — ICT 2024 Mentorship: Lecture 21
- [[sources/2024-mentorship-tutelage-september-04-2024]] — ICT Tutelage September 04, 2024
- [[sources/2024-04-18-ob-tape-reading]] — ICT 2024-04-18: Order Block + Live Tape Reading
- [[sources/old-daily-lows-breaker-entry-and-ifvg-reentry-after-profitable-stop-out]] — Old Daily Lows -Breaker Entry and -IFVG Reentry After Profitable Stop Out; breaker entry, IFVG reentry, and profitable stop-out continuation
- [[sources/premarket-nq-ob-to-discount-ndog-august-27-2024]] — Premarket NQ -OB To Discount NDOG August 27, 2024; order block short, NDOG draw, and institutional orderflow patience
- [[sources/nq-premium-wick-entry-live-execution-may-08-2024]] — NQ Premium Wick Entry - Live Execution May 08, 2024; premium wick micro-scaling with VI, FVG, and inversion logic
- [[sources/nq-lunch-macro-06102024]] — NQ Lunch Macro 06/10/2024; midday volume imbalance, IFVG, and consequent encroachment after the morning drive
- [[sources/how-to-read-price-with-or-without-a-bias-april-29-2024]] — How To Read Price With Or Without A Bias - April 29, 2024
- [[sources/when-do-i-expect-speed-in-my-trades-advanced-order-flow-teaching-ict-concepts]] — When Do I Expect SPEED in My Trades? Advanced Order Flow Teaching ICT CONCEPTS
- [[sources/this-trade-was-a-banger-6000-in-25-minutes-nq-live-trade-walkthrough-ict-concepts]] — This Trade Was A BANGER! $6,000 in 25 Minutes NQ Live Trade Walkthrough ICT CONCEPTS; 15-second entry, midnight-open risk, and breakaway-gap runner management
- [[sources/how-to-trade-ifvg]] — How To Actually Trade Inversion Fair Value Gaps (IFVG); HTF sweep + small-wick candle-two + V-shape reversal
- [[sources/2025-pd-array-matrix]] — ICT 2025-10-18: PD Array Matrix Revealed ("the source code")
- [[sources/ict-suspension-block-review-september-30-2025]] — ICT Suspension Block & Review — September 30, 2025 (first public ICT-direct definition of the suspension block)
- [[sources/2025-storytellers-daily-high-to-low-june-21-2025]] — 2025 Storytellers: Daily High To Low — June 21, 2025 (daily-wick CE as the intraday setup pocket for SB / MM / Unicorn on NQ)
- [[sources/2023-mentorship-market-maker-models]] — ICT 2023 Mentorship: Market Maker Buy/Sell Models
- [[sources/april-08-2024-nq-market-maker-buy-model-example]] — April 08, 2024 NQ Market Maker Buy Model Example
- [[sources/ict-opening-range-theory-1st-presented-fvg-logic]] — ICT Opening Range Theory - 1st Presented FVG Logic
- [[sources/fomc-two-stage-delivery]] — Trading FOMC Two Stage Delivery
- [[sources/trading-all-time-highs-and-disregarding-tgif]] — Trading All Time Highs and Disregarding TGIF
- [[sources/trading-friday-sellside-under-1st-presented-fvg]] — Trading Friday Sellside Under 1st Presented FVG
- [[sources/trading-premarket-and-regular-session-liquidity]] — Trading Premarket and Regular Session Liquidity
- [[sources/top-down-trade-review-september-01-2024]] — Top Down Trade Review September 01, 2024; weekly/daily top-down with NWOG, bullish OB, and Tuesday-low liquidity framing
- [[sources/ict-forex-futures-market-review-october-4-2025]] — ICT Forex & Futures Market Review October 4, 2025
- [[sources/ict-general-market-commentary-november-14-2025]] — live market commentary: draw-on-liquidity, inversion FVG, liquidity void, and market-maker buy/sell bridge
- [[sources/stop-getting-stopped-out-with-this-simple-concept-protected-highs-lows]] — derivative lesson on protected highs/lows, SMT-backed stop placement, and time-based highs
- [[sources/stop-losses-in-trading-know-when-youre-wrong]] — stop-loss invalidation built around protected swings, body-based stops, and continuation entries
- [[sources/2025-lecture-series-smc-new-york-nwog-with-forex-01272025]] — 2025 Lecture Series - SMC New York NWOG With Forex 01/27/2025
- [[sources/new-week-commentary-for-nq-futures-december-01-2024]] — New Week Commentary For NQ Futures December 01, 2024; weekly gap quadrants, CE, and inversion-FVG continuation/reversal
- [[sources/2025-lecture-review-february-03-2025]] — 2025 Lecture Review February 03, 2025
- [[sources/understanding-time-price-the-only-thing-you-need]] — Understanding Time & Price - The Only Thing You Need
- [[sources/ict-2026-futures-weekend-review-april-11-2026]] — live weekend review: continuous contract vs front month, opening-range-gap CE, and first-hour dealing range
- [[sources/ict-2026-futures-review-april-14-2026]] — ICT 2026 Futures Review | April 14, 2026
- [[sources/ict-2026-futures-review-april-24-2026]] — ICT 2026 Futures Review | April 24, 2026; three drives pattern at ATH, partial-profit discipline, and weekend geopolitical gap risk
- [[sources/ict-2026-lecture-trading-ath-in-pd-array-matrix-april-20-2026]] — ICT 2026 Lecture: Trading ATH In The ICT PD Array Matrix | April 20, 2026; continuous contract toggling, premium wick grading, TGIF, bolo, and inversion FVG at ATH
- [[sources/ict-2026-entries-and-drills-april-15-2026]] — ICT 2026 Entries & Drills | April 15, 2026
- [[sources/ict-2026-new-york-lunch-algorithmic-theory]] — ICT 2026 New York Lunch Algorithmic Theory | March 11, 2026
- [[sources/ict-2026-smart-money-concepts-lecture-january-13-2026]] — ICT 2026 Smart Money Concepts Lecture | January 13, 2026
- [[sources/ict-2026-smart-money-concepts-lecture-february-11-2026]] — ICT 2026 Smart Money Concepts Lecture | February 11, 2026; NFP Wednesday opening-range / 9:31 FVG default (1)
- [[sources/ict-2026-smart-money-concepts-in-action-january-06-2026]] — ICT 2026 Smart Money Concepts In Action | January 06, 2026; premarket first-presented FVG, 9:30 opening-range thrust, and 10:00–11:00 offboard rule
- [[sources/ict-2026-smart-money-concepts-lecture-february-23-2026]] — ICT 2026 Smart Money Concepts Lecture | February 23, 2026
- [[sources/ict-2026-market-commentary-march-08-2026]] — live morning review: RTH opening-range gap, premium/discount gap handling, first-presented FVG, and body-vs-wick validation
- [[sources/ict-2026-market-commentary-march-09-2026]] — live morning review: premium opening-range-gap, 9:44 first-presented FVG, sellside / 7-minute-after-10 rule, and propulsion-block confirmation
- [[sources/ict-2026-market-commentary-march-10-2026]] — live morning review: premium opening-range-gap, carry-forward ORG, and 7-minute-after-10 sellside discriminator
- [[sources/ict-2026-market-commentary-march-21-2026]] — live macro commentary: time distortion, HTF alignment, suspension-block / IFVG line-in-the-sand, and low-probability stand-down
- [[sources/ict-2026-market-commentary-march-25-2026]] — live morning review: high-resistance liquidity run conditions, 7:00–9:30 liquidity map, opening-range-gap, and first-presented FVG caution template
- [[sources/ict-2026-market-commentary-march-27-2026]] — live morning review: opening-range gap, first-presented FVG, CE, and suspension-block rules (1)
- [[sources/ict-2026-1st-hour-dealing-range-march-28-2026]] — live first-hour dealing range lesson; distinguishes opening range from first-hour range and adds the shallow-break / projection rule (1)

### 2025 NQ lecture-series batch
- [[sources/nq-telegram-commentary-02212025]] — NQ Futures Live Execution With Telegram Commentary 02/21/2025
- [[sources/nq-review-april-24-2025]] — NQ Review April 24, 2025
- [[sources/nq-ny-lunch-macro-02242025]] — NQ Futures Live Execution With NY Lunch Macro 02/24/2025
- [[sources/nq-live-execution-using-analysis-i-shared-in-students-livestream-02052025]] — NQ Live Execution Using Analysis I Shared In Student's Livestream 02/05/2025; disclaimer-only clip with no usable transcript
- [[sources/nq-live-execution-using-analysis-i-shared-in-telegram-02132025]] — NQ Live Execution Using Analysis I Shared In Telegram 02/13/2025; opening-range-gap, first-presented FVG, and PPI morning execution
- [[sources/nq-live-tape-reading-am-review]] — NQ Live Tape Reading + AM Market Review ICT CONCEPTS; Judas swing, IFVG selection, and lunch continuation framing
- [[sources/nq-review-april-28-2025]] — NQ April 28, 2025 Review
- [[sources/nq-review-april-30-2025]] — NQ April 30, 2025 Review
- [[sources/nq-futures-review-04012025]] — NQ Futures Review 04/01/2025
- [[sources/ict-nq-futures-market-review-october-1-2025]] — ICT NQ Futures Market Review | October 1, 2025; opening-range-gap, 9:31 first-presented FVG, and relative-equal-highs target map
- [[sources/2025-lecture-series-nq-nfp-algorithmic-price-delivery-04042025]] — NQ NFP Algorithmic Price Delivery 04/04/2025; 9:50–10:10 and 10:50–11:10 opening/news macros, gray-pool refinements, and IFVG validation
- [[sources/2025-lecture-series-turtle-soup-deferred-entry-with-rejection-block]] — Turtle Soup Deferred Entry With Rejection Block
- [[sources/nq-heavy-manipulation-review]] — NQ Heavy Manipulation Review
- [[sources/2025-lecture-series-nq-may-01-2025-review]] — NQ May 01, 2025 Review

### Sequence / top-down bias
- [[sources/the-sequence-ep-1-this-makes-trading-liquidity-easy]] — The Sequence Ep.1: This Makes Trading Liquidity Easy
- [[synthesis/how-to-use-the-sequence-model]] — operator guide for the top-down sequence / monthly-to-session narrative workflow

### Mini Batch 2 — May 2025 lecture-series
- [[sources/2025-lecture-series-nq-review-cpi-no-trade-may-13-2025]] — NQ Review CPI No Trade May 13, 2025
- [[sources/2025-lecture-series-ict-gauntlet-nq-am-session-may-07-2025-review]] — ICT Gauntlet & NQ AM Session May 07, 2025 Review
- [[sources/2025-lecture-series-ict-venom-example-may-12-2025]] — ICT Venom Example May 12, 2025
- [[sources/2025-lecture-series-nq-review-may-29-2025]] — NQ Review May 29, 2025
- [[sources/2025-lecture-series-nq-review-extraordinary-volatility-04092025]] — NQ Review & Extraordinary Volatility | 04/09/2025; volatile-day caution template with carried-forward FVGs and time-distortion framing
- [[sources/2025-lecture-series-nq-review-presession-buyside-turtle-soup-trade-may-14-2025]] — NQ Review Presession Buyside Turtle Soup Trade May 14, 2025
- [[sources/2025-lecture-series-nq-review-presession-trade-may-15-2025]] — NQ Review Presession Trade May 15, 2025
- [[sources/2025-lecture-series-nq-review-when-930am-et-is-1st-presented-fvg-may-18-2025]] — NQ Review When 9:30am ET Is 1st Presented FVG May 18, 2025
- [[sources/2025-lecture-series-nq-weekly-summary-02282025]] — NQ Weekly Summary 02/28/2025
- [[sources/2025-lecture-series-forex-nq-review-02052025]] — Forex & NQ Review 02/05/2025

### 2024 mentorship — liquidity conditions
- [[sources/ict-2024-mentorship-how-to-identify-high-resistance-liquidity-conditions-september-27-2024]] — ICT 2024 Mentorship How To Identify High Resistance Liquidity Conditions September 27, 2024
- [[sources/ict-2024-mentorship-high-resistance-low-resistance-conditions-october-28-2024]] — ICT 2024 Mentorship High Resistance & Low Resistance Conditions October 28, 2024

### 2024 mentorship — execution drills and market review
- [[sources/ict-2024-mentorship-how-to-manage-missed-entries-september-17-2024]] — ICT 2024 Mentorship How To Manage Missed Entries September 17, 2024; missed-entry recovery, lower-timeframe re-entry, and macro-window patience
- [[sources/ict-2024-mentorship-limit-orders-volatility-pinball-drills-october-01-2024]] — ICT 2024 Mentorship Limit Orders & Volatility Pinball Drills October 01, 2024; limit-order drills, no-bias execution practice, and body-vs-wick stop logic
- [[sources/ict-2024-mentorship-market-review-october-17-2024]] — ICT 2024 Mentorship Market Review October 17, 2024; opening-gap narrative, Gallow PD array, and gap-midpoint framing

### Mini Batch 3 — CRT, candle mechanics, and lunch macro
- [[sources/why-the-9-am-crt-model-could-change-your-life]] — Why the 9 AM CRT Model Could Change Your Life | CRT trading strategy | ICT Secrets
- [[sources/wick-size-matters-the-key-to-understanding-reversal-and-expansion-candles]] — Wick Size Matters: The Key to Understanding Reversal and Expansion Candles

### Mini Batch 15 — high-impact news drivers and lunch macro
- [[sources/ict-2024-mentorship-news-release-tape-reading-october-17-2024]] — ICT 2024 Mentorship News Release Tape Reading October 17, 2024; 8:30 news smoke screen, first-impulse validation, and no-front-run rule
- [[sources/ict-2024-mentorship-october-nfp-nq-october-04-2024]] — ICT 2024 Mentorship October NFP NQ October 04, 2024; 15-minute wait, pre-release liquidity map, and no-prediction rule
- [[sources/nonfarm-payroll-september-06-2024]] — ICT 2024 Mentorship NonFarm Payroll September 06, 2024; 15-minute bellwether map and no-front-run rule
- [[sources/gbpusd-london-macro-live-execution-2025-01-22]] — January 22, 2025 - Live Execution Forex GbpUsd London Macro; reclaimed FVG, immediate rebalance, and London macro execution
- [[sources/nq-ny-lunch-macro-02242025]] — 2025 Lecture Series - NQ Futures Live Execution With NY Lunch Macro 02/24/2025; first-hour dealing range and lunch objective
- [[sources/trading-high-resistance-liquidity-run-conditions-with-my-lunch-macro]] — Trading In High Resistance Liquidity Run Conditions With My Lunch Macro; stubborn-day lunch execution with inversion FVGs and partials
- [[timing/macros]] — Macros
- [[timing/lunch-macro]] — Lunch Macro
- [[concepts/no-trade]] — No Trade
- [[sources/october-03-2024-nq-market-review]] — October 03, 2024 NQ Market Review; NFP no-trade warning, opening-range-gap context, and late inversion-FVG continuation
- [[sources/secret-way-to-identify-high-probability-market-structure-shifts]] — Secret Way To Identify High Probability Market Structure Shifts..

### Mini Batch 4 — IRL/ERL and lunch macro
- [[sources/trading-irl-erl-with-order-blocks-ict-concepts]] — Trading IRL & ERL With Order Blocks! - ICT Concepts
- [[sources/game-changer-irl-erl]] — The Game Changer to ICT Concepts: IRL & ERL
- [[sources/nq-ny-lunch-macro-02242025]] — 2025 Lecture Series - NQ Futures Live Execution With NY Lunch Macro 02/24/2025

### Derivative teachers
- [[sources/how-to-trade-ifvg]] — How To Actually Trade Inversion Fair Value Gaps
- [[sources/this-stupid-simple-strategy-works-everyday-stupid-simple-and-proven]] — This Stupid Simple Strategy Works Everyday (Stupid Simple And Proven); HTF FVG tap, 5m FVG confirmation, IFVG inversion, and liquidity target
- [[sources/this-simple-fvg-strategy-made-me-12k-in-one-day]] — Tempo Trades compilation; HTF sweep, IFVG confirmation, and opposing-liquidity targeting
- [[sources/how-to-use-the-economic-calendar-for-trading]] — How To Use The Economic Calendar For Trading; news-filtered weekly profile, FOMC/NFP restraint, and post-news execution framing
- [[sources/the-twitter-model-the-mmxm-trader-ict-concepts]] — MMXM Trader Twitter Model; ERL→IRL sweep, FVG confirmation, SMT/MSS trigger, and midnight-open filter
- [[sources/the-mmxm-traders-2024-yt-mentorship-episode-1]] — MMXM Trader mentorship opener; HTF bias, SMT, premium/discount, and CISD sequencing
- [[sources/950-macro-atm-model-ict-tape-read]] — 9:50 Macro + ATM Model; external-to-internal morning macro with HTF alignment
- [[sources/live-atm-model-trade-ict-tape-read]] — LIVE A(T)M Model Trade; live tape-read demo using the daily A(T)M model
- [[sources/the-confirmation-model]] — The Confirmation Model; HTF FVG, OTE sweep, SMT, IFVG, and CISD confirmation checklist
- [[sources/the-only-trading-strategy-you-need-for-2026]] — fractal daily/hourly/5m model; daily bias, continuation order block, and time-frame alignment
- [[sources/next-day-model-fractal-way-to-get-bias-for-trading]] — Fractal next-day bias scaffold built from the previous candle close / range failure

- [[sources/internal-external-liquidity]] — Internal & External Liquidity Model (TTrades)
- [[sources/why-youre-failing-with-ict-concepts]] — Why You're Failing with ICT Concepts; single-array discipline, CISD focus, and highs/lows as execution context
- [[sources/the-3-step-a-plus-ict-strategy-that-actually-works]] — external-range-liquidity targeting, no-trade when target is unclear, and calendar-based restraint
- [[sources/simple-power-of-three]] — This Simple Power of 3 Strategy Changed My Trading (JadeCap)
- [[sources/my-forever-model-the-strategy-that-has-made-me-over-half-a-million-insane-value]] — My Forever Model; manipulation, IFVG, CISD, SMT, and opposing liquidity target
- [[sources/most-traders-lose-because-of-this-and-heres-5-ways-to-fix-it]] — mind-over-market checklist; alignment, journaling, and boring execution
- [[sources/never-miss-another-trade]] — The Sequence / candle anatomy model; three opportunities inside one candle
- [[sources/trade-continuations-using-order-blocks]] — Trade Continuations Using Order Blocks; continuation entries after reversal confirmation
- [[sources/trade-continuations-using-breaker-blocks]] — Trade Continuations Using Breaker Blocks; continuation via breaker retest, SMT exception, and FVG fallback
- [[sources/how-to-trade-turtle-soups]] — How to trade Turtle Soups / Liquidity Sweeps (Arjo, MMC series)
- [[sources/game-changer-irl-erl]] — Game Changer: IRL & ERL (The MMXM Trader, 2024-03-26)
- [[sources/hrlr-vs-lrlr]] — HRLR vs LRLR
- [[sources/what-is-icts-immediate-rebalance]] — What Is ICT's Immediate Rebalance?

- [[sources/micro-scalping-without-bias-nq-may-06-2024]] — Micro-Scalping Without Bias - NQ May 06, 2024; no-bias micro-scaling with volume imbalance, IFVG, breakaway-gap, and partial management
- [[sources/making-4-000-in-30-minutes-nq-live-trade-walkthrough-ict-concepts]] — Making $4,000 in 30 Minutes! NQ Live Trade Walkthrough ICT CONCEPTS; CBI-style discount entry, volume imbalance adds, IFVG support, and 5m order-block management
- [[sources/market-structure-shift-ict-concepts]] — Market Structure Shift - ICT Concepts; displacement, sweep-first confirmation, and post-break FVG / order-block entry
- [[sources/ict-nq-live-execution-september-6-2024-100k-osok]] — ICT NQ Live Execution September 6, 2024 100k [OSOK]; turtle-soup short, daily FVG CE, and live sell-model management
- [[sources/nq-pm-session-turtle-soup-long-full-pull-august-30-2024]] — NQ PM Session Turtle Soup Long Full Pull August 30, 2024; turtle-soup short, sell-model context, and CE management

### Psychology
- [[sources/this-speech-by-ict-hits-ict-2024-mentorship-motivation]] — This Speech By ICT Hits! [ICT 2024 Mentorship Motivation]; patience, consistency, and trust in one model
- [[sources/how-to-stop-giving-it-all-back]] — How to Stop Giving It All Back; euphoria, scarcity thinking, and self-worth traps
- [[sources/build-a-winning-trading-psychology-mindset]] — Build a Winning Trading Psychology Mindset; performance-over-money framing, probability mind, and learning to lose well
- [[sources/how-millionaire-traders-build-unshakeable-trading-discipline]] — How Millionaire Traders Build Unshakeable Trading Discipline; dopamine control, ritual, and boring consistency
- [[sources/why-you-cant-hold-trades-and-how-to-stay-calm-in-big-moves]] — why traders cut winners early, and how to stay calm while holding a winner
- [[sources/why-systematic-trading-is-the-only-way-to-profit-and-build-wealth-sustainably]] — why system adherence matters more than intelligence or effort
- [[sources/why-most-traders-lack-consistency-and-how-you-can-be-different]] — process, patience, and staying with one system long enough to compound edge
- [[sources/why-does-everything-change-when-the-money-is-real]] — money psychology, uncertainty, and the shift from paper to live risk
- [[sources/why-do-your-subconscious-beliefs-about-money-have-so-much-power-over-your-trading]] — subconscious money beliefs, threat response, and retraining for live trading
- [[sources/your-results-match-your-identity-not-your-strategy]] — identity set-point, thermostat principle, and disciplined repetition
- [[sources/the-anti-sabotage-checklist-5-rules-for-professional-execution]] — pattern interruption, premortem, physical anchors, and one-bullet discipline
- [[sources/top-trading-psychologist-reveals-the-fastest-way-to-end-self-sabotage]] — self-sabotage, hidden benefits, and replacing overtrading / overrisking with alternative coping systems
- [[sources/the-harder-you-try-the-more-success-slip-slides-away-why]] — emotional-brain bias, probability-based mind, and why brute force fails in trading
- [[sources/self-sabotage-youre-afraid-of-the-life-trading-will-give-you]] — self-sabotage as fear of success, responsibility, and identity change
- [[sources/developing-a-patient-trading-mind]] — patience, boredom, and watchful waiting instead of forcing action
- [[sources/the-foolproof-strategy-to-become-profitable-in-2025]] — behavioral discipline clip: data-proven system, action over knowledge, and repeated rule adherence
- [[sources/the-flow-state-model-the-2-step-strategy-that-has-made-me-100k-plus-this-month]] — simple two-step strategy framed around flow, repetition, and consistency
- [[sources/stop-failing-challenges-how-i-got-max-ftmo-funded-with-ict-concepts]] — sequence-style challenge execution frame built around process and discipline

### Analysis — bridge sources
- [[sources/this-ict-model-will-change-your-trading-forever-smt-cisd-time]] — This ICT Model Will Change Your Trading Forever (SMT + CISD + Time)
- [[sources/intro-smt-divergence]] — Intro to SMT Divergence (Fearing)
- [[sources/4000-in-7-minutes-trading-my-ict-30m-po3-model]] — $4,000 In 7 Minutes: Trading My ICT 30m PO3 Model; weekly/daily PO3 nesting, SMT, and 1m OB / 15s CISD
- [[sources/new-york-reversal-explained-daily-profile-strategy]] — New York Reversal Explained | Daily Profile Strategy; daily-profile filter with London failure, NY completion, and CISD
- [[sources/protected-swings-understanding-trend-and-invalidations]] — Protected Swings – Understanding Trend and Invalidations; protected highs/lows, SMT, and continuation invalidation
- [[sources/timeframe-alignment-how-to-align-timeframes-for-expansion]] — Timeframe Alignment: How To Align Timeframes For Expansion; HTF→MTF→LTF expansion stack and alignment rules
- [[sources/the-secret-to-ict-daily-bias-a-mechanical-approach]] — The Secret To ICT Daily Bias; quarterly market-profile bias, accumulation/distribution, and mechanical top-down selection
- [[sources/ict-secret-to-selecting-algorithmic-pd-arrays-october-14-2025]] — ICT Secret To Selecting Algorithmic PD Arrays; immediate rebalance, REH/NWOG, and PD-array selection

- [[sources/mnq-pm-silver-bullet-walkthrough]] — MNQ Live Trade Walkthrough — PM Silver Bullet (2025-02-13)
- [[sources/nq-live-tape-reading-am-review]] — NQ Live Tape Reading AM (Chermane Trades, 2025-05-27)
- [[sources/nq-trade-breakdown-reclaimed-ifvg-entry-with-trump-volatility-live-account-ict-concepts]] — NQ Trade Breakdown - Reclaimed IFVG Entry With Trump Volatility (Live Account)
- [[sources/nq-live-trade-walkthrough-holding-through-the-930-open-ict-concepts]] — NQ Live Trade Walkthrough - Holding Through the 9:30 Open!
- [[sources/ict-explains-how-to-trade-last-hour-macro]] — ICT Explains How To Trade Last Hour Macro
- [[sources/how-to-fix-a-losing-trade-nq-live-trade-walkthrough-ict-smart-money-concepts]] — How To Fix A Losing Trade; daily OB / IFVG / NDOG recovery with partials and reduced risk
- [[sources/this-was-my-largest-trade-ever-nq-live-trade-walkthrough-final-hour-macro-ict-concepts]] — This Was My LARGEST Trade Ever! NQ Live Trade Walkthrough - Final Hour Macro
- [[sources/nq-trade-breakdown-how-to-pick-the-right-first-presented-fvg-ict-concepts]] — NQ Trade Breakdown - How To Pick The Right First Presented FVG
- [[sources/this-very-simple-fvg-scalping-strategy-is-all-you-need-to-be-profitable-in-2026]] — This Very Simple FVG Scalping Strategy is all you need to be Profitable in 2026; London-session FVG scalping, 9:45–9:50 wait, and 15-minute open patience rule
- [[sources/from-vision-to-execution]] — From Vision To Execution; cast-the-vision draw-on-liquidity lecture with first-presented-FVG and turtle-soup examples

### Mini Batch 3 — concept/model ingest
- [[sources/algorithmic-price-delivery-live-recorded-lesson]] — Algorithmic Price Delivery - Live recorded lesson
- [[sources/always-wait-for-this-before-entering-a-trade-candle-behavior]] — Always Wait For THIS Before Entering a Trade (Candle Behavior)
- [[sources/best-ict-turtle-soup-trading-strategy-that-works-insane-winrate]] — Best ICT Turtle Soup Trading Strategy That Works! (Insane Winrate)
- [[sources/broadening-formations-ict-seek-destroy]] — Broadening Formations - ICT Seek & Destroy
- [[sources/calubs-model-conceptually-variant-1]] — Calub's Model "Conceptually" - Variant #1

### Mini Batch 4 — AM-session and entry mechanics
- [[sources/ep8-the-daily-range]] — EP8: The Daily Range
- [[sources/entries-using-order-flow]] — Entries using Order Flow
- [[sources/every-ict-trading-strategy-explained-in-13-minutes]] — Every ICT Trading Strategy Explained in 13 Minutes!
- [[sources/first-presentation-model-1-scalping]] — First Presentation Model #1 scalping
- [[sources/hrlr-vs-lrlr]] — High Resistance vs Low Resistance Liquidity - ICT Concepts
- [[sources/how-do-i-engage-markets-when-i-dont-have-an-initial-bias]] — How Do I Engage Markets When I Don't Have An Initial Bias?

### Mini Batch 5 — time delivery and journaling
- [[sources/2025-lecture-series-algorithmic-timing-and-journaling-03222025]] — Algorithmic Timing & Journaling 03/22/2025
- [[sources/2025-lecture-series-making-money-with-smc-concepts]] — Making Money With SMC Concepts

### Mini Batch 5b — forex review and weekly options
- [[sources/2025-lecture-series-smc-forex-review-02042025]] — SMC Forex Review 02/04/2025
- [[sources/2025-lecture-series-weekly-option-strategy-intro-03282025]] — Weekly Option Strategy Intro 03/28/2025

### Mini Batch 5c — weekly narrative and NQ storytelling
- [[sources/am-trades-blending-the-economic-calendar-daily-chart-weekly-profiles]] — AM Trades | Blending The Economic Calendar, Daily Chart, & Weekly Profiles
- [[sources/2025-storytellers-series-nq-review-june-02-2025]] — 2025 Storytellers Series - NQ Review June 02, 2025
- [[sources/2025-storytellers-series-nq-futures-june-05-2025]] — 2025 Storytellers Series - NQ Futures June 05, 2025

### Mini Batch 5d — wick structure and live-money psychology
- [[sources/2025-lecture-series-nq-may-01-2025-review]] — 2025 Lecture Series - NQ May 01, 2025 Review
- [[sources/master-candlestick-wicks-the-key-to-catching-reversals]] — Master Candlestick Wicks - The Key To Catching Reversals
- [[sources/controlling-your-emotions-when-the-money-is-real]] — Controlling Your Emotions When the Money Is Real

### Mini Batch 6 — opening-range gap and profile variants
- [[sources/smc-opening-range-gaps]] — 2025 Lecture Series - SMC Opening Range Gaps
- [[sources/ict-gems-opening-range-gap-secrets]] — ICT Gems - Opening Range Gap Secrets
- [[sources/ict-the-first-presented-fvg-in-the-opening-range]] — ICT - The First Presented FVG In The Opening Range
- [[sources/how-to-predict-daily-highs-and-lows]] — How To Predict Daily Highs and Lows
- [[sources/ict-daily-profile-seek-and-destroy]] — ICT Daily Profile - Seek & Destroy

### Mini Batch 7 — opening-price filter cluster
- [[sources/important-time-levels-for-trading]] — Important Time Levels For Trading
- [[sources/this-is-my-simple-trading-model-for-2025-chermanes-model-ict-concepts]] — This is My SIMPLE Trading Model for 2025
- [[sources/how-to-trade-this-easy-2025-model-chermanes-model-nq-trade-breakdown-ict-concepts]] — How to Trade This EASY 2025 Model
- [[sources/nq-trade-breakdown-how-to-achieve-intraday-bias-top-down-analysis-deep-study-ict-concepts]] — NQ Trade Breakdown: How to Achieve Intraday Bias

### Mini Batch 8 — CRT and first-hour dealing range
- [[sources/tired-of-9-5-learn-the-9-am-crt-model-to-achieve-financial-freedom]] — Tired of 9-5? Learn the 9 AM CRT Model
- [[sources/ict-2026-1st-hour-dealing-range-march-28-2026]] — ICT 2026 1st Hour Dealing Range
- [[timing/9-am-crt]] — 9 AM CRT
- [[timing/first-hour-dealing-range]] — First Hour Dealing Range
- [[concepts/consequent-encroachment]] — Consequent Encroachment

### Mini Batch 10 — turtle-soup premarket / post-open variants
- [[sources/nq-pm-session-turtle-soup-long-full-pull-20240830]] — NQ PM Session Turtle Soup Long Full Pull
- [[sources/june-24-2024-nq-turtle-soup-short]] — June 24, 2024 NQ Turtle Soup Short
- [[sources/january-21-2025-live-execution-nq-premarket-turtle-soup-short]] — January 21, 2025 Live Execution
- [[deferred/index]] — deferred niche concepts and variants, including Rejection Block

### Mini Batch 14 — no-initial-bias / no-trade / CPI-news filter cluster
- [[sources/how-do-i-engage-markets-when-i-dont-have-an-initial-bias]] — How Do I Engage Markets When I Don't Have An Initial Bias?
- [[sources/2025-lecture-series-nq-review-cpi-no-trade-may-13-2025]] — NQ Review CPI No Trade May 13, 2025
- [[concepts/no-trade]] — No Trade

### Mini Batch 15 — Episode 35 order-block / SMT / FVG scaffold
- [[sources/2022-ict-mentorship-episode-35-order-block-and-smt-divergence]] — 2022 ICT Mentorship Episode 35 - Order Block And SMT Divergence
- [[concepts/order-block]] — Order Block
- [[concepts/smt]] — SMT
- [[concepts/fair-value-gap]] — Fair Value Gap

### Mini Batch 17 — Episode 37 breaker / FVG / liquidity / journaling scaffold
- [[sources/2022-ict-mentorship-episode-37]] — 2022 ICT Mentorship Episode 37
- [[concepts/fair-value-gap]] — Fair Value Gap
- [[concepts/liquidity]] — Liquidity
- [[concepts/market-structure-shift]] — Market Structure Shift
- [[concepts/order-block]] — Order Block
- [[concepts/relative-equal-highs-lows]] — Relative Equal Highs & Lows

### Mini Batch 16 — Episode 36 premium-discount / liquidity / MSS scaffold
- [[sources/2022-ict-mentorship-episode-36]] — 2022 ICT Mentorship Episode 36
- [[concepts/premium-discount]] — Premium / Discount
- [[concepts/fair-value-gap]] — Fair Value Gap
- [[concepts/liquidity]] — Liquidity
- [[concepts/market-structure-shift]] — Market Structure Shift
- [[concepts/relative-equal-highs-lows]] — Relative Equal Highs & Lows

### Mini Batch 13 — quarter-hour opening / news / market-on-close macros
- [[sources/nq-futures-review-04012025]] — NQ Futures Review 04012025
- [[sources/nq-nfp-algorithmic-price-delivery-04042025]] — NQ NFP Algorithmic Price Delivery 04042025
- [[sources/smc-algorithmic-market-on-close-macro]] — SMC Algorithmic Market On Close Macro
- [[timing/quarters-of-the-hour]] — Quarters of the Hour

### Mini Batch 12 — Beesting at Open SMT + CISD model
- [[sources/this-ict-model-will-change-your-trading-forever-smt-cisd-time]] — This ICT Model Will Change Your Trading Forever (SMT + CISD + Time)
- [[sources/this-ict-model-will-make-you-profitable-forever-stop-paying-for-mentorships-beesting-open-vid-2]] — This ICT Model Will Make You Profitable Forever! Stop Paying For Mentorships (BeeSting Open Vid 2)
- [[synthesis/how-to-trade-the-beesting-at-open-model]] — How to Trade the Beesting at Open Model

### Mini Batch 11 — opening-range-gap and midnight-range scaffold
- [[sources/smc-opening-range-gaps]] — SMC Opening Range Gaps
- [[sources/smc-trading-opening-range-gaps]] — SMC Trading Opening Range Gaps
- [[sources/smc-midnight-opening-range]] — SMC Midnight Opening Range
- [[timing/opening-range]] — Opening Range
- [[timing/midnight-opening-range]] — Midnight Opening Range
- [[concepts/opening-range-gap]] — Opening Range Gap

### Mini Batch 9 — silver bullet windows
- [[sources/am-silver-bullet-strategy-on-nq]] — AM Silver Bullet Strategy on NQ
- [[sources/nq-pm-session-silver-bullet-august-26-2024]] — NQ PM Session Silver Bullet - August 26, 2024
- [[sources/2023-mentorship-silver-bullet]] — 2023 ICT Mentorship - ICT Silver Bullet Time Based Trading Model
- [[timing/silver-bullet-windows]] — Silver Bullet Windows

## Synthesis

- [[meta/how-hermes-trading-analyst-should-review-trade-ideas]] — review playbook for validating upstream trade ideas against wiki timing, model-family fit, confluence, contradictions, and no-trade conditions
- [[meta/how-hermes-trading-analyst-should-use-the-model-stack]] — hierarchy for reducing the model list into a cleaner delivery / execution / confluence stack for trade-idea generation
- [[synthesis/how-to-use-daily-range-and-drt-levels]] — operator guide for the EP8 daily-range / DRT / measuring-gap cluster on NQ
- [[synthesis/how-to-handle-heavy-manipulation-days]] — practical execution guide for noisy NQ conditions where the framework is still valid but execution must become more conservative
- [[synthesis/how-to-handle-cpi-no-trade-days]] — operator guide for CPI impulse days where the opening thesis may fail and no trade is the correct outcome
- [[synthesis/how-to-use-resistance-liquidity]] — operator guide for the high-resistance / low-resistance liquidity framing
- [[synthesis/how-to-use-price-delivery-continuum]] — operator guide for the price delivery continuum / quarter-of-hour execution framework
- [[synthesis/how-to-use-pd-array-matrix]] — operator guide for the PD Array Matrix selection framework and quadrant grading
- [[synthesis/how-to-trade-when-you-dont-have-an-initial-bias]] — operator guide for the no-initial-bias opening-state workflow
- [[synthesis/how-to-manage-missed-entries]] — operator guide for recovering from a missed entry without forcing a replacement trade
- [[synthesis/how-to-use-order-flow-entries]] — operator guide for FVG-based sharp turns and orderflow-lag entries
- [[synthesis/how-to-use-order-blocks-and-dealing-ranges]] — operator guide for order blocks, dealing ranges, and mean threshold
- [[synthesis/how-to-trade-turtle-soups]] — operator guide for Turtle Soup / liquidity sweep reversals
- [[synthesis/how-to-trade-ifvg]] — operator guide for trading inversion FVG continuation / reversal setups
- [[synthesis/how-to-use-first-presented-fvg]] — practical guide for using the first valid session-window FVG as the AM/PM opening anchor on NQ
- [[synthesis/how-to-journal-ict-time-signatures]] — operator guide for recording time signatures, opening ranges, and repeat behavior
- [[synthesis/how-to-trade-the-beesting-at-open-model]] — operator guide for the opening-session SMT + CISD + time model
- [[synthesis/intraday-nq-mnq-playbook]] ⭐ — end-to-end operator playbook for intraday NQ/MNQ: HTF context → session frame → window → model ID → entry → stop → target → invalidation → instrument → journal
- [[synthesis/how-to-trade-the-930-11am-window]] — operator guide for focusing only on the 9:30–11:00 a.m. ET NQ session
