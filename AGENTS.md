# ICT Wiki — AGENTS Handoff Manual

This file is the active operating manual for any agent maintaining this Obsidian vault.

Purpose: maintain a personal knowledge base on the **Inner Circle Trader (ICT)** methodology to support trading decisions in **MNQ** (Micro E-mini Nasdaq futures).

The human curates sources, asks questions, and approves structural changes.
The agent reads, summarizes, cross-references, files, lints, and maintains the wiki.

If `CLAUDE.md` and `AGENTS.md` differ, follow `AGENTS.md` as the current canonical schema, while preserving the intent and conventions established in `CLAUDE.md`.

## Model policy

- Use **GPT-5.4 mini** for routine source ingestion, batch summarization, source-page creation, backlinking, and index/log maintenance.
- Escalate to a larger model only when explicitly requested by the user, or when a task is unusually synthesis-heavy, ambiguous, or requires deep reconciliation across many sources.
- Default assumption: **ingest work should be done with GPT-5.4 mini**.
- If a non-mini model is used for ingest or doctrine updates, note that fact in the chat reply or log entry.

## Layers

- `Clippings/` — raw sources (Obsidian Web Clipper outputs, mostly YouTube transcripts). **Read-only.**
- `Pics/` — images (chart screenshots, PDFs). **Read-only.** May contain irrelevant material; ignore what is not useful.
- `wiki/` — agent-owned knowledge layer. Write and maintain everything here.
- `journal/` — the user's dated trading observations. Read to mine patterns; edit only when explicitly asked.
- `CLAUDE.md` — original schema and provenance.
- `AGENTS.md` (this file) — current canonical instructions.

## Vault structure

Current core structure:

```
wiki/
  index.md              Catalog grouped by type. Update at end of each ingest batch.
  log.md                Append-only operational record.
  concepts/             Building blocks: FVG, OB, liquidity, IPDA, BPR, SMT, etc.
  models/               Full setups: Silver Bullet, PO3, OTE, Unicorn, Turtle Soup.
  timing/               Killzones, macros, sessions, news windows.
  instruments/          Per-instrument pages. MNQ.md is the flagship page.
  sources/              One page per ingested clipping/source.
  synthesis/            Higher-order pages, playbooks, comparisons, checklists.
```

This structure is a strong starting schema, not a hard ceiling. In the spirit of the LLM Wiki pattern, the vault may gain new folders when the knowledge base evolves and a new durable page category clearly deserves its own lane.

Only add a new folder when it improves retrieval, maintenance, and conceptual clarity — not just aesthetics. Prefer extending the current structure first, but create a new folder when a distinct page type repeatedly emerges and would otherwise overload an existing directory.

Examples of justified future folders include categories like `playbooks/`, `regimes/`, `checklists/`, `frameworks/`, or other durable lanes that become necessary as the wiki compounds.

## Core operating principles

### 1. Raw sources are immutable

Never edit files in:
- `Clippings/`
- `Pics/`
- PDFs or downloaded attachments

All interpretation and summarization belongs in `wiki/sources/` and downstream wiki pages.

### 2. Doctrine and analysis stay separate

- **Doctrine** = what ICT teaches, or what repeated sourced material supports. Lives in `concepts/`, `models/`, `timing/`, `instruments/`.
- **Analysis** = dated market reads, trade reviews, observations, and execution notes. Lives in `journal/`.
- **Synthesis** = durable operator knowledge built from doctrine, source comparisons, and repeated evidence. Lives in `synthesis/`.

Never file dated market commentary into doctrine pages.
Never convert a single journal observation into doctrine.
If a journal entry seems important, surface it as evidence or as a hypothesis in synthesis.

### 3. Every material claim is traceable

Inline-citation format:

```
Claim text ([[sources/some-source-page]] @ 12:34).
Claim text with multiple citations ([[sources/source-a]] @ 1:22, [[sources/source-b]] @ 18:09).
```

Target standard:
- wiki page -> `wiki/sources/...`
- source page -> raw clipping

Any important claim should be verifiable in two clicks.

No-citation exceptions:
- navigation prose
- headings and structural text
- frontmatter
- explicitly labeled journal observations and hypotheses

If a claim cannot be substantiated, use:

```
> [!note] Uncited — needs verification
> Claim text here.
```

Never ghost-cite.
Never imply a source said more than it actually said.

### 4. Preserve provenance and confidence

When writing doctrine or synthesis, distinguish among these evidence tiers:

1. **ICT-direct** — direct ICT source material. Highest doctrinal weight.
2. **Derivative teacher** — teacher/commentator interpreting ICT. Useful, but not equal to ICT-direct.
3. **Single observed example** — one trade or one session example. Evidence, not doctrine.
4. **Repeated journal observation** — user-observed recurring pattern. Hypothesis until strongly supported.
5. **Uncited** — explicitly marked as needing verification.

When a derivative teacher conflicts with ICT-direct material, do not silently merge them. State the conflict.
When multiple derivative teachers agree but ICT-direct confirmation is missing, say so.

### 5. Do not delete knowledge casually

Do not delete substantive content without user approval.
If something is outdated or contradicted:
- preserve the old claim when useful
- mark tension or supersession clearly
- cite the newer source

## Standard operations

## Ingest — single source

1. Read the raw clipping in full.
2. Create `wiki/sources/<slug>.md` with frontmatter including:
   - `type: source`
   - `title`
   - `source_type`
   - `raw`
   - `date_ingested`
   - `key_concepts`
   - `tags`
   - `aliases`
3. Add sections:
   - `## Summary` with 3–8 core bullets
   - `## Key quotes` with timestamped quotes worth reusing
   - `## See also`
4. Update touched doctrine pages in:
   - `concepts/`
   - `models/`
   - `timing/`
   - `instruments/`
5. If the source creates a durable cross-source insight, consider updating or creating a `synthesis/` page.
6. Append one line to `wiki/log.md`.

## Ingest — batch

Same per-source workflow, with these additional rules:
- Use **GPT-5.4 mini** as the default ingest model.
- Defer `wiki/index.md` rewrite until the batch is complete.
- Merge duplicate claims into existing doctrine pages instead of stacking repetitive prose.
- Prefer strengthening existing pages over creating shallow new pages.
- Log one line per source or one clearly enumerated batch line.

## Query

1. Read `wiki/index.md` first.
2. Follow relevant doctrine/synthesis pages.
3. Follow source citations when the answer depends on a specific claim.
4. Answer with citations preserved when appropriate.
5. If the answer is durable, offer to file it into `wiki/synthesis/`.
6. Log meaningful filed outputs.

## Journal handling

Use `journal/_template.md` when creating dated entries.

Rules:
- Fill only what the user describes.
- Do not invent bias, levels, results, or emotions.
- If a journal entry supports or contradicts doctrine, flag the relationship rather than silently updating doctrine.
- Repeated journal observations may be elevated into a synthesis page as hypotheses.

## Lint

When asked to lint, report before fixing unless the user asks for auto-remediation.

Check for:
- orphan `sources/` pages with no inbound doctrinal links
- concepts/models/timing pages referenced repeatedly but missing
- contradictions between doctrine pages
- stale claims superseded by newer sources
- `[!note] Uncited` blocks still unresolved
- overloaded pages that should be split
- source pages with weak key_concepts or missing quotes

## Page creation rules

Create a missing doctrine page when one or more are true:
- it is linked repeatedly across existing wiki pages
- it appears in at least 3 ingested sources
- it is load-bearing for MNQ execution decisions
- it is needed to resolve ambiguous backlinks or pending references

Otherwise, it may remain pending in `index.md` until enough evidence exists.

When creating a page, prefer substance over stubs. A short but well-cited page is better than an empty placeholder.

## Page conventions

- Every wiki page should include frontmatter with at least:
  - `type`
  - `tags`
  - `aliases`
- First H1 matches the page title.
- Use Obsidian wikilinks `[[...]]` for internal references.
- End with `## See also`.
- `sources/` filenames use lowercase dash-separated slugs derived from clipping titles.
- Preserve existing naming unless there is a clear consistency problem.

## Synthesis pages

`synthesis/` is for durable operator knowledge, not raw doctrine repetition.

Good synthesis page types:
- playbooks
- checklists
- regime-recognition guides
- comparisons
- contradictions across teachers
- MNQ execution notes derived from multiple sources
- recurring hypotheses grounded in journal evidence

A synthesis page should normally answer a practical question such as:
- How do I recognize a valid MNQ Silver Bullet?
- What distinguishes low-resistance from high-resistance delivery?
- When should MNQ be preferred over ES/NQ/YM alternatives?
- What invalidates this setup quickly?

Synthesis pages must preserve source provenance.
If a page includes judgment or interpretation, label it clearly.

## Anti-patterns

- Don't paraphrase beyond the source.
- Don't flatten ICT jargon into generic trading language.
- Don't treat derivative teachers as equal to ICT-direct doctrine without saying so.
- Don't silently convert a single example into a rule.
- Don't rewrite `index.md` after every file change in a batch.
- Don't mix doctrine, observations, and hypotheses without labels.
- Don't create many tiny low-information stub pages just to satisfy links.

## Recommended working order for this vault

When resuming maintenance on this specific vault:

1. Preserve the existing structure and conventions.
2. Use **GPT-5.4 mini** for ingest by default.
3. Prioritize high-centrality missing pages already referenced throughout the wiki.
4. Continue ingesting clippings in manageable batches.
5. Start creating `synthesis/` pages early so the vault compounds into practical trading guidance.

Suggested near-term page priorities include:
- `concepts/liquidity-sweep`
- `concepts/market-structure-shift`
- `concepts/change-in-state-of-delivery`
- `concepts/buyside-liquidity`
- `concepts/sellside-liquidity`
- `concepts/discount-premium`
- `concepts/new-week-opening-gap`
- `timing/quarters-of-the-hour`
- `instruments/NQ`
- `models/internal-external-liquidity-model`

## Handoff note

This vault was originally scaffolded under `CLAUDE.md` in the LLM Wiki pattern.
This `AGENTS.md` file is a continuity handoff, not a reset.
The goal is to preserve the existing wiki architecture while continuing maintenance with disciplined, source-traceable updates.
