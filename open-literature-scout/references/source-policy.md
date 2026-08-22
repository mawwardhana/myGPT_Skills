# Source Policy

## Preferred scholarly sources

Priority order:

1. Original journal or publisher
2. PubMed
3. Crossref
4. OpenAlex
5. DOAJ
6. University or institutional repository

## Source verification

A recommended paper should preferably have at least one of:

- DOI
- PMID
- Publisher record
- Stable repository record

## Evidence hierarchy

For questions requiring empirical evidence:

1. Primary research
2. Systematic review / meta-analysis for contextual support
3. Narrative review for background only

Do not substitute review articles for primary research when the
user explicitly requests primary studies.

## Open-access policy

When equivalent sources exist, prefer:

- Gold open access
- Public repository versions
- Author manuscripts legally deposited in repositories

Do not describe an article as open access unless this has been verified.

## Clean-link and stable-identifier policy

User-facing scholarly links should identify the source without relying on
tracking or referral parameters.

When available, prefer stable scholarly identifiers such as:

- DOI
- PMID
- PMCID
- stable publisher record
- stable repository record

Remove tracking parameters from canonical source URLs when they are under
the assistant's control.

Examples of parameters that should not be intentionally preserved
include:

- utm_source
- utm_medium
- utm_campaign
- referral parameters
- tracking identifiers

Do not claim that a rendered hyperlink is tracking-free unless the
user-visible destination can actually be represented without tracking
parameters.

If a client, interface, or rendering layer may rewrite a clickable URL,
prefer a stable scholarly identifier rather than presenting the
tracking-bearing rendered URL as a clean canonical link.

Acceptable fallbacks include:

- DOI plus source name;
- PMID plus PubMed;
- PMCID plus repository/source name;
- source name plus another stable identifier;
- canonical URL rendered as plain or code text when necessary.

Interface-added tracking parameters must not be treated as part of the
scholarly source identity.

The objective is source-identification integrity, not a guarantee that
every user interface will preserve the exact URL string supplied by the
assistant.