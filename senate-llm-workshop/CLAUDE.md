# senate-llm-workshop

Dual-purpose public folder: workshop materials for the Academic Senate AI workshop AND temporary Inter Metro AI Knowledge Base. Everything committed here is immediately public on GitHub (`pwayland/The-Repository/senate-llm-workshop/`).

## Structure

```
workshop/       ← delivery materials (prompt guide, templates, provocation, resources)
catalog/        ← GENERATED program/degree .md files from curricular-sequence YAML
institutional/  ← MANUAL curated institutional context files
data/           ← reference data (CSV, job market compilations)
archive/        ← Workshop 1.0 materials (preserved, not active)
```

Not committed: `scripts/` (generation tools), `drafts/` (WIP), `private/` (source docs).

## File Standards

Every .md knowledge base file uses this frontmatter:

```yaml
---
title: [descriptive title]
source: generated | manual
owner: Paul Wayland
last-updated: YYYY-MM-DD
catalog-year: 2020-21  # only for catalog/ files
---
```

- **Target**: 200–400 lines. **Hard max**: 500 lines → split the file.
- Each file must be independently useful — no dependencies between KB files.
- Catalog data is in Spanish (from SmartCatalog). Workshop materials are bilingual (English + Spanish) within single files.

## Generation

`catalog/` files are generated from curricular-sequence YAML. **Do not hand-edit them.** To fix content, fix the source or regenerate.

Read-only sources (never write to these):
- `~/curricular-sequence/data/degrees/2020-21/*.yaml` — 146 degree files
- `~/curricular-sequence/data/courses/courses-2025-26.yaml` — course definitions
- `~/curricular-sequence/data/gen-ed/gen-ed-bachelor.yaml`, `gen-ed-associate.yaml`

Current approach: Claude reads YAML directly and writes .md. Post-workshop: build `scripts/generate-catalog-md.py` for repeatability.

## Git

This folder is inside `The-Repository` (git root one level up). Commit messages: lowercase imperative ("add programs-business.md to catalog"). Push to `origin/main` — public immediately.

Never commit: `scripts/`, `drafts/`, `private/`, any file with credentials or personal data.

## Model Strategy

Sonnet default. This is content creation and file generation work.

## Output Discipline

- No sycophantic openers or closers
- Act first; explain only if non-obvious
- Do not suggest changes outside requested scope
