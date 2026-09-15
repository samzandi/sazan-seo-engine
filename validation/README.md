# Sazan SEO Engine — Validation Protocol

This directory defines repeatable evidence-based validation before any production-ready claim.

## Required fixtures

Every release candidate must be checked against four representative cases:

1. Informational content
2. Commercial/service content
3. Local-service content
4. Multilingual content

## Validation sequence

1. Load the relevant brand/context references.
2. Generate or inspect the SEO brief.
3. Verify one dominant search intent per page.
4. Check the used-keyword registry for cannibalization.
5. Run on-page quality gates.
6. Run technical quality gates when a page/site implementation exists.
7. Validate structured data against visible, verified facts.
8. Validate local SEO only when a real location/service area is supported by evidence.
9. Validate GEO/AEO answerability, entity clarity, factual support, and citation readiness.
10. Record PASS, WARN, FAIL, NOT_APPLICABLE, and evidence for every assertion.
11. Record unresolved risks.

## Release rule

A release may not be described as production-ready when:

- a critical assertion is FAIL;
- required evidence is missing;
- an invented or unsupported fact is present;
- keyword cannibalization is unresolved;
- indexability/canonical behavior is unknown when technical SEO is in scope;
- structured data contains claims not visible or supported on the page.

Warnings require an explicit risk note. NOT_APPLICABLE requires a reason.
