---
type: timing
aliases: [Killzones, Kill Zones]
tags: [timing]
---

# Killzones

Named sessions where ICT models require entries to be taken. The [[models/internal-external-liquidity-model|Internal-External Liquidity Model]] explicitly gates entries by killzone ([[sources/internal-external-liquidity]] @ 1:56, @ 3:47, @ 8:49).

## Killzones referenced in ingested sources

- **London Killzone** — used in example entries ([[sources/internal-external-liquidity]] @ 3:47).
- **New York Killzone** — used in example entries ([[sources/internal-external-liquidity]] @ 8:49).

## Boundaries

Canonical killzone boundaries from the 2022 ICT Mentorship ([[sources/2022-ict-mentorship-episode-3]], [[sources/2022-ict-mentorship-episode-8]]):

|| Session | Time (New York local) | Notes |
||---------|----------------------|-------|
|| **London Killzone** | **2:00 AM – 5:00 AM** | Track session highs and lows; market often sweeps above/below these levels |
|| **New York Killzone** | **7:00 AM – 10:00 AM** | Primary execution window |
|| **Asia Session** | **7:00 PM – 9:00 PM** | Evening session; less emphasized for intraday futures |

**Optimal trading hours** ([[sources/2022-ict-mentorship-episode-3]], [[sources/2022-ict-mentorship-episode-8]]):
- **8:30 AM – 11:00 AM** (can extend to noon)
- **Avoid**: Noon hour (problematic)
- **Resume**: 1:30 PM – 4:00 PM (afternoon trend)
- **Best afternoon setup**: 2:00 PM – 3:00 PM

## See also

- [[models/internal-external-liquidity-model]]
- [[timing/silver-bullet-windows]]
- [[timing/macros]]
