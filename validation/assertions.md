# Validation Assertions

## Severity

- CRITICAL: failure blocks release and production-ready claims.
- MAJOR: failure blocks the SEO quality gate until resolved or explicitly removed from scope with evidence.
- MINOR: warning requiring documentation.

## Core assertions

| ID | Severity | Assertion |
| --- | --- | --- |
| INTENT-001 | CRITICAL | The page has one dominant, explicitly defined search intent. |
| FACT-001 | CRITICAL | Material factual claims are supported by verified project references or cited research. |
| FACT-002 | CRITICAL | No testimonials, ratings, credentials, locations, prices, guarantees, statistics or business facts are invented. |
| KW-001 | MAJOR | The primary keyword/query and intent do not create unresolved cannibalization with an existing canonical page. |
| META-001 | MAJOR | Metadata accurately represents visible content and user intent. |
| HEAD-001 | MAJOR | The H1 and heading hierarchy describe the page structure without mechanical keyword repetition. |
| LINK-001 | MAJOR | Internal links are relevant, intentional and point to valid destinations when implementation evidence exists. |
| CANON-001 | CRITICAL | Canonical behavior is correct when technical implementation is in scope. |
| INDEX-001 | CRITICAL | Indexability and robots behavior match the intended search visibility when implementation is in scope. |
| SCHEMA-001 | CRITICAL | Structured data matches visible, verified content and the correct entity/page type. |
| LOCAL-001 | CRITICAL | Local business identity, NAP and service-area claims are verified when local SEO is in scope. |
| LOCAL-002 | MAJOR | Location pages provide distinct user value and are not unsupported doorway pages. |
| GEO-001 | MAJOR | Important questions have concise, factually supported answers that can be understood out of context. |
| LANG-001 | CRITICAL | Multilingual canonicals and alternate-language relationships do not collapse or misidentify valid language pages. |
| EVID-001 | CRITICAL | Every PASS on a release-critical assertion has inspectable evidence. |

## Decision rule

BLOCKED if any applicable CRITICAL assertion fails or lacks evidence.

BLOCKED if any applicable MAJOR assertion fails unless the feature is explicitly out of scope with a documented reason.

PASS only when all applicable release-blocking assertions pass and warnings are documented.
