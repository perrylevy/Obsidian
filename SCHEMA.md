# Wiki Schema

## Domain
This wiki covers Inner Circle Trader (ICT) methodology and related execution knowledge for trading NQ/MNQ futures.

## Active governing documents
- `AGENTS.md` — current canonical operating manual
- `CLAUDE.md` — original schema/provenance
- `SCHEMA.md` (this file) — llm-wiki compatibility layer and concise schema summary

If these differ, follow `AGENTS.md` first, then `SCHEMA.md`, while preserving historical intent from `CLAUDE.md`.

## Architecture mapping
This vault predates the generic llm-wiki folder template and uses a domain-specific structure:

- `Clippings/` — immutable raw source material
- `Pics/` — immutable assets / screenshots / PDFs
- `wiki/sources/` — source-summary bridge pages
- `wiki/concepts/` — concept pages
- `wiki/models/` — setup/model pages
- `wiki/timing/` — time-window/session pages
- `wiki/instruments/` — instrument pages
- `wiki/synthesis/` — durable query results, playbooks, operator guides
- `journal/` — dated observations and execution notes; not doctrine
- `wiki/index.md` — catalog
- `wiki/log.md` — append-only action log

Equivalent llm-wiki layer mapping:
- Raw layer = `Clippings/`, `Pics/`
- Wiki layer = `wiki/...`
- Schema layer = `AGENTS.md`, `SCHEMA.md`, `CLAUDE.md`

## Conventions
- Use lowercase, dash-separated filenames for wiki pages where practical.
- Use Obsidian `[[wikilinks]]` for internal references.
- Every wiki page should have YAML frontmatter.
- Every material doctrinal claim should be source-traceable.
- Raw sources are immutable.
- Update `wiki/index.md` and `wiki/log.md` whenever meaningful wiki changes are made.
- Expand the structure when justified, including new folders, but only when it improves retrieval and maintenance.

## Frontmatter
Minimum expected fields on wiki pages:

```yaml
---
type: concept | model | timing | instrument | source | synthesis | index | journal
tags: []
aliases: []
---
```

Source pages should additionally include fields such as:
- `title`
- `source_type`
- `raw`
- `date_ingested`
- `key_concepts`

## Tag taxonomy
Tags are intentionally lightweight in this vault. Prefer the established families:
- `concept`
- `model`
- `timing`
- `instrument`
- `source`
- `synthesis`
- `futures`
- `NQ`
- `MNQ`
- `review`
- `playbook`
- `regimes`
- `ict-core`
- `pd-array`
- `liquidity`
- `price-action`
- `market-maker`
- `structure`

Add new tags deliberately; avoid freeform tag sprawl.

## Page thresholds
- Create a page when a concept/model/instrument is central to one source or appears across multiple sources.
- Prefer updating an existing page when the concept already has a durable home.
- Keep passing mentions inside source pages; do not promote every mention into doctrine.
- Split overloaded pages when they become too broad or hard to scan.
- New folders are allowed when a truly durable new page category emerges.

## Update policy
When new information conflicts with existing content:
1. Prefer newer and more direct sources.
2. Distinguish ICT-direct doctrine from derivative-teacher interpretation.
3. Preserve explicit tensions instead of silently flattening them.
4. Mark uncertainty with an uncited/note block when needed.

## Session orientation rule
At the start of each session involving this wiki, orient by reading:
1. `SCHEMA.md`
2. `AGENTS.md`
3. `wiki/index.md`
4. recent entries from `wiki/log.md`

Then search the existing wiki before creating new pages.
