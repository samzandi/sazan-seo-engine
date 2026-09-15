---
name: seo-schema
description: Detect, design, validate, and review Schema.org structured data without inventing entities or unsupported claims.
---

# SEO Schema

## Workflow
1. Identify the real page entity and page purpose.
2. Inspect existing JSON-LD/microdata/RDFa when available.
3. Select only schema types supported by actual visible/verified content.
4. Keep entity identifiers consistent across pages.
5. Validate required/recommended properties for the intended search feature when applicable.
6. Flag contradictions between structured data and visible page content.
7. Generate implementation-ready JSON-LD only from verified inputs.
8. Revalidate after deployment.

## Common candidates
Organization, LocalBusiness subtypes, Service, Article/BlogPosting, BreadcrumbList, WebSite, WebPage, Product/Offer, FAQPage when current search-policy eligibility and page content justify it.

## Hard rule
Structured data is not a place to manufacture ratings, prices, locations, authorship, credentials, availability, or other facts.
