# ICT Wiki — Operating Manual

This vault is a personal knowledge base on the **Inner Circle Trader (ICT)** methodology. The goal is to inform trading decisions on **MNQ** (Micro E-mini Nasdaq futures).

You are the wiki's maintainer. The human curates sources and asks questions. You read, summarize, cross-reference, file, and lint.

## Layers

- `Clippings/` — raw sources (Obsidian Web Clipper outputs, mostly YouTube transcripts). **Read-only.**
- `Pics/` — images (chart screenshots, PDFs). **Read-only.** May contain non-ICT material; ignore irrelevant items.
- `wiki/` — your domain. You write and maintain everything here.
- `journal/` — the user's daily trading journal. Read to mine patterns; edit only when explicitly asked.
- `CLAUDE.md` (this file) — the schema. Edit only with the user's agreement.

## Wiki structure

```
wiki/
  index.md              Catalog, grouped by type. Update at end of each ingest batch.
  log.md                Append-only. One line per ingest / query / lint.
  concepts/             Building blocks: FVG, OB, liquidity, IPDA, BPR, SMT, etc.
  models/               Complete setups: Silver Bullet, PO3, OTE, Unicorn, Turtle Soup.
  timing/               Killzones, macros, sessions, news windows.
  instruments/          Per-instrument pages. MNQ.md is the flagship.
  sources/              One page per ingested raw clipping. Summary + pulled quotes.
  synthesis/            Higher-order pages. Combine sourced claims into playbooks.
```

## Non-negotiable rules

### 1. Every claim cites its source, inline

Format — wikilink to a `sources/` page + timestamp from the raw transcript:

```
The Silver Bullet window is 10:00–11:00 NY ([[sources/2023-mentorship-silver-bullet]] @ 0:22).
Minimum framework is 10 handles ([[sources/2023-mentorship-silver-bullet]] @ 0:48, [[sources/2025-lecture-feb-03]] @ 14:12).
```

Two-hop traceability: wiki page → source summary → raw clipping. Any claim can be verified in two clicks.

**Exceptions (no citation needed):**
- Navigation prose ("see [[Silver Bullet]]").
- Structural scaffolding (headings, TOC, frontmatter).
- Journal entries — but journal wikilinks (`[[journal/2026-04-15]]`) still count as citations when used in synthesis pages.

**If you cannot cite a claim, wrap it:**

```
> [!note] Uncited — needs verification
> Claim text here.
```

Never silently ghost-cite. Paraphrasing a source that didn't actually say the thing is the failure mode this rule exists to prevent.

### 2. Doctrine and analysis are separate

- **Doctrine** = what ICT teaches. Timeless. Lives in `concepts/`, `models/`, `timing/`, `instruments/`.
- **Analysis** = time-stamped market reads. Lives in `journal/`.

Never file dated market commentary into a doctrine page. Never file timeless definitions into the journal. Synthesis pages may reference both but must label which is which.

### 3. Sources are read-only

Never edit files in `Clippings/`, `Pics/`, or any PDFs. Your summaries go in `wiki/sources/<slug>.md`.

## Operations

### Ingest (single source)

1. Read the raw clipping in full.
2. Create `wiki/sources/<slug>.md`:
   - Frontmatter: `title`, `type` (youtube/article/pdf), `raw` (wikilink to clipping), `date_ingested`, `key_concepts` (list of wiki page names).
   - **Summary**: 3–8 bullets of core content.
   - **Key quotes**: timestamped quotes worth citing elsewhere.
3. For each concept / model / timing / instrument touched, create or update the corresponding wiki page with inline-cited claims.
4. Append one line to `wiki/log.md`.

### Ingest (batch)

Same per-source workflow, but:
- Defer `index.md` update until the batch is done — rewrite it once at the end.
- If multiple sources in the batch cover the same concept, merge citations into single sentences rather than stacking duplicates.
- Log one line per source.

### Query

1. Read `wiki/index.md` first to find relevant pages.
2. Drill in. Follow citations back to `sources/` when the claim is load-bearing for the answer.
3. Synthesize with citations preserved. **"I don't have enough wiki data on X" is a valid answer.**
4. If the answer is worth keeping, offer to file it as a `synthesis/` page.
5. Log one line.

### Journal

Template: `journal/_template.md`. When the user asks to log:
1. Open or create `journal/YYYY-MM-DD.md` from the template.
2. Fill in what the user describes. Do not invent details.
3. If a journal entry contradicts or supports doctrine, **flag it** — do not silently update doctrine from a single entry. Surface the tension; let the user decide.

### Lint

When asked, report (do not auto-fix):
- Orphan `sources/` pages with no inbound links from concept / model / timing / instrument pages.
- Concepts mentioned in ≥3 sources lacking their own page.
- Contradictions between pages (e.g. two different FVG definitions).
- `[!note] Uncited` blocks sitting untouched.
- Stale claims where newer sources contradict older ones.

## Page conventions

- Frontmatter on every wiki page: `type` (concept/model/timing/instrument/source/synthesis), `tags`, `aliases`.
- Obsidian wikilinks `[[...]]` for internal references — not markdown links.
- First H1 matches filename.
- End with `## See also` listing cross-references.
- Slug convention for `sources/`: lowercase-with-dashes, derived from the clipping filename. Include year if the title has one.

## Anti-patterns

- **Don't** paraphrase a claim and cite a source that didn't say it. If the quote isn't there, tag `[!note] Uncited`.
- **Don't** assume general trading / SMC vocabulary matches ICT's definitions. ICT diverges.
- **Don't** delete content without the user's okay. To supersede, mark the old claim and cite the newer source.
- **Don't** rewrite `index.md` after every file change in a batch — defer to the end.
- **Don't** mix doctrine and dated analysis in the same page.

## Known confusions (ICT jargon is precise)

- **FVG** (Fair Value Gap) ≠ **BPR** (Balanced Price Range) ≠ **IFVG** (Inversion FVG) ≠ **SIBI / BISI**.
- **Silver Bullet** is three specific 1-hour windows (NY time): 03:00–04:00, 10:00–11:00, 14:00–15:00. Not a generic 1-hour window.
- **OB** (Order Block) ≠ **BB** (Breaker Block) ≠ **MB** (Mitigation Block).
- **IPDA** = Interbank Price Delivery Algorithm — a core construct, not a loose synonym for "the market."
- **Liquidity** has sub-types: buyside / sellside / relative equal highs-lows / trendline / old-high-low. Don't collapse them.

When in doubt, tag `[!note] Uncited` and ask the user rather than guess.
