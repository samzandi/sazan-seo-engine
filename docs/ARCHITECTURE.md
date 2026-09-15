# Architecture

Sazan SEO Engine is platform-independent. The core is a small orchestrator plus focused skills and project reference files.

## Layers

1. **Context** — verified brand/business facts, voice, evidence, keyword history.
2. **Research** — search intent, SERP evidence, competitors, questions, entities, local context.
3. **Planning** — content briefs, keyword/page mapping, internal links, conversion goals.
4. **Execution** — content/page recommendations or implementation guidance.
5. **Validation** — on-page, technical, schema, local, GEO/AEO, evidence and cannibalization gates.
6. **Record** — update keyword registry and material decisions.

## Skill routing
- `seo-engine` — orchestrator
- `seo-content-brief` — pre-writing research and brief
- `seo-page` — single-page optimization/audit
- `seo-technical` — crawl/index/render/site technical checks
- `seo-local` — location-dependent businesses
- `seo-schema` — structured data
- `seo-geo` — AI/answer-engine readiness

## Platform adapters
Adapters for ChatGPT, Codex, Claude Code, or other agents may call the same core skills. Platform-specific instructions must not become core SEO requirements.

## Evidence rule
Observed data, user-provided facts, and recommendations are distinct classes. If evidence is unavailable, the engine reports the gap rather than inventing certainty.
