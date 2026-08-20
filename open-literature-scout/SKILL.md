---
name: open-literature-scout
description: >
  Search, screen, verify, extract, appraise, and synthesize scientific
  literature using publicly accessible scholarly sources. Use this skill when the user
  asks to find scientific papers, primary studies, systematic reviews,
  DOI information, or evidence supporting a research question.
---

# Open Literature Scout
Version: 0.8

## Purpose

Help identify relevant and credible scientific literature using
a transparent and reproducible workflow.

## When to use

Use this skill when the user asks to:

- find scientific papers;
- identify primary research articles;
- find supporting literature for a research topic;
- verify DOI or bibliographic information;
- distinguish primary and secondary literature;
- identify recent evidence;
- find open-access scientific sources.

Do not use this skill for:

- general news;
- casual web searches;
- non-academic information requests.

## Required inputs

Identify when available:

1. Research topic or question
2. Population or object of study
3. Main variables or concepts
4. Publication year range
5. Preferred study design
6. Language restriction
7. Open-access requirement

If information is incomplete, derive reasonable search concepts
from the research question.

## Workflow

### Step 1 — Understand the research question

Identify:

- population;
- intervention or exposure;
- outcome;
- context;
- key concepts;
- synonyms.

## Question-framework selection

After understanding the research question, consult:

references/question-frameworks.md

Select a structured question framework when it materially improves
question decomposition or search-strategy development.

Allowed framework labels:

- PICO
- PECO
- PCC
- PICo
- SPIDER
- NONE

Do not force PICO or another framework onto a question that does not
fit it.

Select one primary framework unless there is a clear methodological
reason to use another approach.

Report:

- selected framework;
- reason for selection;
- framework elements;
- which elements will be translated into searchable concepts.

If no formal framework is needed, use:

"Framework: NONE"

and continue with the standard core-concept workflow.

Do not invent missing framework elements.

Framework selection structures the search question only. It must not
override evidence-status, screening, verification, ranking, or
domain-specific rules.


### Step 2 — Generate search terms

Create:

- main keywords;
- synonyms;
- scientific terminology;
- Boolean combinations when useful.

## Search transparency

Before presenting the selected literature, report:

1. Core search concepts
2. Main keywords and synonyms
3. At least one Boolean search string
4. Scholarly sources actually used

Do not silently perform the literature search without reporting
the search strategy.

The search strategy should be concise but sufficiently transparent
for the user to understand how the literature was identified.

### Step 3 — Search scholarly sources

Prefer:

1. Publisher or journal website
2. PubMed
3. Crossref
4. OpenAlex
5. DOAJ
6. Institutional repositories
7. Other credible scholarly databases

Avoid relying on blogs or commercial aggregator pages when
the original scholarly source is available.

## Search refinement

After the initial scholarly search, consult:

references/search-refinement.md

Evaluate the retrieved-result pattern before proceeding to final
screening.

Use only these primary search diagnosis labels:

- ADEQUATE
- TOO_BROAD
- TOO_NARROW
- TERMINOLOGY_GAP
- SOURCE_LIMITATION

Refine the query only when an observed retrieval problem justifies the
change.

Do not silently replace the initial query.

For every search iteration, preserve:

- iteration number;
- query used;
- source actually searched;
- diagnosis;
- change made;
- reason for the change.

When the initial query is adequate, state:

"No refinement required."

Do not judge search quality from result count alone.

Do not invent result counts.

Search refinement changes retrieval strategy only. It must not override
evidence-status, screening, DOI-verification, ranking, framework, or
domain-specific rules.


### Step 4 — Screen results

Assess:

- relevance;
- article type;
- population or sample;
- methods;
- variables;
- outcomes;
- publication year;
- journal;
- DOI;
- full-text availability.

### Step 5 — Classify evidence

Classify each article as:

- Primary research
- Systematic review
- Meta-analysis
- Narrative review
- Guideline
- Other

Never classify a review article as primary research.

## Primary-study enforcement

When the user explicitly requests primary research:

Include an article in the confirmed primary-research results only when
there is sufficient evidence that the authors generated or analyzed
original empirical data.

Primary research may include:

- experimental laboratory studies;
- clinical studies;
- observational studies;
- in vivo studies;
- in vitro studies;
- original quantitative or qualitative studies.

Do not include as confirmed primary research:

- narrative reviews;
- systematic reviews;
- meta-analyses;
- editorials;
- perspectives;
- commentaries;
- protocols without results.

If primary-study status cannot be fully verified, do not classify the
article as CONFIRMED.

Assign the appropriate evidence decision state:

- PROBABLE when primary status is likely but one important element
  remains unresolved;
- UNVERIFIED when available information is insufficient to establish
  primary-study status.

Do not mix PROBABLE or UNVERIFIED records with CONFIRMED evidence
without clearly labeling their status.


## Evidence decision states

Every candidate article must be assigned one evidence decision state.

Use only these states:

### CONFIRMED

Use when:

- the article is verified as primary research;
- the article directly contains empirical data relevant to the user's question;
- bibliographic identity is verified;
- the article's relevance can be confirmed from a reliable scholarly source.

### PROBABLE

Use when:

- the article appears to be primary research and directly relevant;
- but one important element required to establish its evidence status
  cannot yet be fully verified.

Examples:

- article type cannot yet be conclusively verified;
- relevance to the research question is likely but available
  bibliographic information is incomplete;
- bibliographic identity cannot yet be fully established.

DOI verification alone does not determine evidence status.

A CONFIRMED study may have a DOI verification status of:

"Not verified"

Do not mix PROBABLE records with CONFIRMED records without clearly
labeling their evidence status.


### UNVERIFIED

Use when:

- insufficient information is available to establish article type,
  relevance, or bibliographic identity.

Do not present UNVERIFIED records as established evidence.

### EXCLUDED

Use when the article does not satisfy the inclusion criteria.

Examples:

- review article when primary research is requested;
- editorial or commentary;
- irrelevant organism;
- irrelevant intervention;
- article does not contain empirical data relevant to the research question.

Always provide a short exclusion reason.


## Mechanistic primary-study rule

Do not exclude a primary study merely because its main purpose is
mechanistic.

A mechanistic study should remain eligible when it contains original
empirical measurements directly relevant to the user's research question.

For example, a study investigating antibacterial mechanisms may still
qualify as CONFIRMED primary evidence when it experimentally measures:

- MIC;
- MBC;
- bacterial viability;
- growth inhibition;
- membrane damage;
- bacterial killing;
- biofilm inhibition;
- other direct antibacterial outcomes.

Classify such studies as:

"Primary research — mechanistic"

when appropriate.


### Step 6 — Verify bibliographic information

For every article recommended as a confirmed result, verify whenever possible:

- exact title;
- authors;
- publication year;
- journal;
- DOI;
- article type;
- relevance to the requested research topic.

### DOI verification rule

A DOI should be treated as verified only when the DOI can be matched
to the same article title through a reliable scholarly source.

Preferred verification sources:

1. Original publisher or journal
2. Crossref
3. PubMed
4. Other authoritative bibliographic database

Do not infer a DOI from citations found on unrelated webpages.

If the DOI cannot be independently matched to the article title,
use the DOI verification status:

"Not verified"

### Link rule

When providing a DOI, prefer the canonical DOI format:

https://doi.org/[DOI]

Avoid tracking parameters such as:

utm_source
utm_campaign
utm_medium

when a clean canonical identifier is available.

## Controlled reporting vocabulary

Use standardized labels to improve reproducibility.

### DOI verification

Use only:

- Verified — Publisher
- Verified — Crossref
- Verified — PubMed
- Verified — Multiple authoritative sources
- Not verified

### Full-text access

Use only:

- Open access
- Free full text
- Subscription/paywalled
- Status not verified

Do not invent alternative labels such as:

- confirmed free article;
- probably open access;
- full text seems available.

When multiple verification sources are available, prefer:

"Verified — Multiple authoritative sources"

### Step 6A — Extract evidence when needed

After evidence classification and bibliographic verification, consult:

references/evidence-extraction.md

Use only these extraction modes:

- BASIC
- DETAILED

Use BASIC by default for routine article-finding tasks.

Use DETAILED when the user requests study characterization, evidence
extraction, comparison of study methods or findings, an evidence table,
or detailed support for literature review or manuscript development.

When DETAILED mode is active, also use:

assets/evidence-extraction-template.md

Detailed extraction should normally be performed for CONFIRMED studies.

PROBABLE studies may be extracted only when useful, but their unresolved
evidence status must remain explicit.

Use only these Extraction basis labels:

- FULL_TEXT
- ABSTRACT_ONLY
- METADATA_ONLY

For required detailed-extraction fields with unavailable information,
use only:

- NOT_REPORTED
- NOT_VERIFIED
- NOT_APPLICABLE

Do not infer missing study details.

Do not present information obtained only from an abstract as if the
full article had been inspected.

Evidence extraction must not override evidence status, DOI verification,
screening decisions, search diagnosis, search stopping rules, or
domain-specific rules.


### Step 6B — Appraise evidence when needed

After evidence extraction, when methodological appraisal is requested
or materially necessary to answer the user's question, consult:

references/evidence-appraisal.md

Use only these appraisal modes:

- NONE
- FORMAL_TOOL
- STRUCTURED_SCOUT_APPRAISAL

Do not perform formal appraisal automatically for routine article
finding.

Select the appraisal approach according to the verified study design.

Before applying a named formal appraisal tool, verify its current
official version and status.

Do not reproduce or modify a formal appraisal tool from memory.

When FORMAL_TOOL is used, also use:

assets/evidence-appraisal-template.md

When STRUCTURED_SCOUT_APPRAISAL is used, also use:

assets/evidence-appraisal-template.md

A CONFIRMED evidence state must not be interpreted as a high-quality or
low-risk-of-bias judgment.

Do not create a universal numerical quality score across appraisal
tools or study designs.

Appraisal judgments must remain separate from study-reported
information.

When appraisal is based only on methodological information supplied
directly by the user rather than an inspected scholarly source, use:

`USER_PROVIDED_INFORMATION`

as the appraisal basis and do not imply that the original article or
full text was inspected.

Evidence appraisal must not override evidence status, DOI verification,
screening decisions, search diagnosis, search stopping rules, or
domain-specific rules.


### Step 6C — Synthesize evidence when needed

After relevant evidence has been extracted and, when appropriate,
appraised, consult:

references/evidence-synthesis.md

Use only these synthesis modes:

- NONE
- NARRATIVE_SYNTHESIS
- CLAIM_SUPPORT

Use NONE for routine literature scouting, study characterization, or
methodological appraisal when no cross-study conclusion is requested.

Use NARRATIVE_SYNTHESIS when the user asks what multiple studies
collectively show.

Use CLAIM_SUPPORT when a specific scientific claim must be evaluated
against the evidence set.

When synthesis is active, also use:

assets/evidence-synthesis-template.md

Before synthesizing, define the evidence set and assess study
comparability.

Use only these comparability labels:

- DIRECTLY_COMPARABLE
- PARTIALLY_COMPARABLE
- NOT_DIRECTLY_COMPARABLE

For CLAIM_SUPPORT, use only these study-contribution labels:

- DIRECT_SUPPORT
- INDIRECT_SUPPORT
- CONTRARY_EVIDENCE
- NO_DIRECT_BEARING

and only these claim-assessment labels:

- SUPPORTED
- QUALIFIED_SUPPORT
- MIXED_EVIDENCE
- INSUFFICIENT_EVIDENCE
- NOT_SUPPORTED

Do not determine evidence strength by study counts alone.

Do not create numerical study weights from appraisal judgments.

Check for overlapping evidence and avoid double counting.

Do not interpret absence of evidence as evidence of absence.

Do not generalize beyond the population, organism, material,
intervention, outcome, or context supported by the evidence.

This synthesis module is narrative.

Do not calculate pooled effects, weighted averages, meta-analytic
statistics, or formal certainty grades unless a separate appropriate
workflow is explicitly invoked.

Evidence synthesis must not override evidence status, DOI verification,
screening decisions, extraction records, appraisal judgments, search
diagnosis, search stopping rules, or domain-specific rules.


## Ranking rules

Rank articles according to relevance to the user's question, not merely
publication year.

Use the following priority:

1. Directness of evidence to the research question
2. Confirmed primary-research status
3. Match between intervention and requested intervention
4. Match between organism/population and requested organism/population
5. Quality of bibliographic verification
6. Availability of directly relevant outcome data
7. Recency, when otherwise comparable

Do not automatically rank the newest article first.

Landmark older studies may rank highly when they provide more direct
evidence.


## Source-use integrity

Under "Sources searched", report only sources that were actually used
during the current search.

Do not list PubMed, Crossref, OpenAlex, DOAJ, or another database merely
because it appears in the preferred-source policy.

Distinguish between:

- source searched;
- source used for discovery;
- source used for verification.

## Domain-specific reference rules

When a domain-specific reference file is available and directly relevant
to the user's research topic, apply it in addition to the general
screening workflow.

Do not apply domain-specific rules to unrelated research topics.

For chitosan-related literature searches, use:

references/chitosan-screening.md


### Step 7 — Mandatory output contract

For every literature-search task, use the structure defined in:

assets/output-template.md

The output template is mandatory.

Do not create an alternative response structure.

Do not skip, rename, merge, or reorder the following sections:

1. Research question
2. Search strategy
3. Screening criteria
4. Selected literature
5. Screening notes
6. Search quality

Preserve the internal placement of mandatory template components.

In particular:

- question-framework selection belongs under `2. Search strategy`;
- detailed evidence extraction belongs under `4. Selected literature`;
- evidence appraisal belongs under `4. Selected literature`;
- evidence synthesis belongs under `4. Selected literature`.

Do not move these components into another mandatory section.


All required fields in the selected-literature table must be included.

If information for a required field cannot be verified, write:

"Not verified"

Do not omit the field.

## Result consistency rule

Every article mentioned in the final literature-search report must have
a clear record status.

An article discussed in the narrative must be one of:

- included in Selected literature;
- listed as PROBABLE;
- listed as UNVERIFIED;
- listed as EXCLUDED; or
- explicitly identified as contextual/background literature.

Do not introduce an article in summary, recommendation, DOI, or
conclusion sections if it has not appeared earlier with a clear status.

Before finalizing the response, cross-check article names, counts,
evidence states, DOI counts, and domain-specific classification counts
against the Selected literature and Screening notes.