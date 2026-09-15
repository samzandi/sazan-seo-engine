# Sazan SEO Engine

A reusable, platform-independent SEO workflow and skill system for AI-assisted projects.

## What it does

Sazan SEO Engine turns verified brand context and search evidence into SEO briefs, page audits, technical audits, local SEO plans, structured-data guidance, and GEO/AEO recommendations. It keeps evidence separate from generated recommendations and uses explicit quality gates before work is considered complete.

## Core skills

- `skills/seo-engine/` — orchestrator and shared workflow
- `skills/seo-content-brief/` — writer-ready evidence-backed briefs
- `skills/seo-page/` — single-page on-page audit/optimization
- `skills/seo-technical/` — crawl, index, canonical, sitemap, rendering and performance checks
- `skills/seo-local/` — local business/service-area SEO
- `skills/seo-schema/` — Schema.org/JSON-LD design and validation
- `skills/seo-geo/` — AI search / answer-engine readiness

## Context and evidence

- `references/brand-context-template.md` — reusable brand/business context
- `references/content-evidence-template.md` — verified facts and sources
- `references/used-keywords.md` — keyword/page registry to reduce cannibalization

## Quality gates

`checklists/seo-quality-gates.md` covers intent, on-page, structured data, technical checks, evidence, documentation, and completion criteria.

## Architecture

See `docs/ARCHITECTURE.md` for the platform-independent layered design and routing model.

## Design principles

1. Search intent before keyword mechanics.
2. Humans before keyword density.
3. Verified facts before generated claims.
4. Evidence and recommendations remain distinguishable.
5. Avoid doorway pages and keyword cannibalization.
6. Conventional SEO and GEO/AEO complement each other.
7. Platform adapters may vary; the SEO core stays portable.
8. No production-ready claim without validation evidence.

## Origin

The architecture was inspired in part by public SEO workflow demonstrations that separate brand voice/reference files, keyword history, on-page checks, and technical SEO stages. Sazan SEO Engine generalizes those ideas into a platform-independent system rather than copying a demo website or tying the workflow to one AI vendor.

## Status

Core v0.1 structure is implemented. It is usable as a workflow specification, but not yet declared production-ready: automated validation, fixtures, and repeatable test evidence are still required.
