# Sazan SEO Engine Skill

## Purpose

Create, improve, and audit SEO work using explicit project context, evidence, and measurable quality gates. The skill is platform-independent and is designed for AI-assisted workflows across ChatGPT, Codex, Claude Code, GitHub agents, and comparable systems.

## Core workflow

1. Load relevant project and brand references.
2. Identify page type, search intent, audience, geography, locale, service/product scope, and conversion goal.
3. Build a keyword/query map and check the used-keyword registry for intent collision or cannibalization.
4. Produce an SEO brief before final content or implementation recommendations.
5. Apply brand voice and verified facts; distinguish facts, assumptions, and recommendations.
6. Run the on-page SEO quality gates.
7. Run technical SEO checks when implementation is in scope.
8. Run local SEO checks only when genuine location/service-area evidence exists.
9. Validate structured data against visible, verified content.
10. Run GEO/AEO checks for answerability, entity clarity, factual support, and citation readiness.
11. For multilingual work, validate language targeting, localized query mapping, canonicals, alternate-language relationships, and presentation concerns.
12. Record used keywords and material decisions.
13. Run `validation/assertions.md` and record evidence with `validation/validation-report-template.md`.
14. Automatically repair safe, recoverable failures and re-run the relevant gates.
15. Continue until complete or a genuine human-only blocker exists.

## Rules

- Never invent business facts, statistics, testimonials, addresses, credentials, prices, guarantees, locations, ratings, reviews, certifications, or claims.
- Do not keyword-stuff or optimize for mechanical keyword-density targets.
- Separate verified research facts from generated recommendations.
- Prefer useful human-readable content over search-engine theater.
- Avoid doorway pages and city-name substitution pages.
- Do not create structured data for facts or entities that are not supported by visible/verified content.
- Do not declare a page or project production-ready without inspectable validation evidence.
- Keep the core skill platform-independent; platform adapters may extend it without changing the evidence rules.
- A successful tool call or file write is not proof that the SEO result is correct.

## Autonomous execution

When the environment permits further safe work, continue without asking the user to say "next". Do not stop merely because a substep, file creation, or tool call completed.

Stop only for a genuine blocker such as missing credentials/access, unavailable required evidence, an owner-only decision with materially different consequences, a consequential external action requiring explicit approval, unsupported tooling, or a safety/policy restriction.

## Inputs

Use relevant files under `references/`, the used-keyword registry, project-specific context, and verified external research when required. Missing critical business facts must be marked UNKNOWN rather than fabricated.

## Outputs

A normal run should produce, as applicable:

- SEO brief
- target query and dominant search intent
- primary and supporting keyword/query map
- content/page recommendations
- on-page audit
- technical audit
- local SEO audit
- structured-data recommendations/audit
- GEO/AEO review
- multilingual review
- updated keyword registry
- validation report with evidence
- unresolved risks and blockers

## Validation fixtures

Before a production-ready claim, use representative cases under `validation/fixtures/` where applicable:

- informational
- commercial/service
- local-service
- multilingual

Use PASS, WARN, FAIL, or NOT_APPLICABLE for assertions. Any applicable critical assertion that fails or lacks evidence blocks the production-ready claim.

## Completion states

Use completion terms precisely:

- Created — artifact exists.
- Implemented — intended change is present.
- Verified — applicable checks ran and evidence was inspected/recorded.
- Production-ready — only when a concrete implementation passes all applicable release-critical validation with inspectable evidence.
