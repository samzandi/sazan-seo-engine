# Fixture: Multilingual

## Scenario

A project publishes equivalent German and Persian pages for the same supported service or topic.

## Expected intent

The same underlying intent, localized for each language and audience rather than mechanically translated.

## Required checks

- Each page has a language-appropriate query map and natural terminology.
- Facts and offer details remain consistent across languages.
- Localized metadata is meaningful rather than literal keyword substitution.
- hreflang/alternate relationships are reciprocal and use valid language/region codes when implementation is in scope.
- Canonicals do not incorrectly collapse distinct language pages into one language.
- RTL presentation concerns are recorded for Persian implementations where relevant.
- Keyword registry records locale/language so cross-language targeting is not misclassified as cannibalization.

## Critical failure examples

- Wrong-language canonical.
- Broken or non-reciprocal hreflang relationship.
- Material offer differences caused only by translation error.
- Keyword stuffing introduced by literal translation.
