---
name: open-literature-scout
description: >
  Search, screen, verify, extract, appraise, and synthesize scientific
  literature using publicly accessible scholarly sources. Use this skill when the user
  asks to find scientific papers, primary studies, systematic reviews,
  DOI information, or evidence supporting a research question.
---

# Open Literature Scout
Version: 0.8.10

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

Comparability is a relationship among evidence units relative to the
intended synthesis target.

Do not assign a comparability label to a singleton evidence unit by
comparing the study with itself.

Keep eligible singleton evidence units separate until a meaningful
comparison or synthesis role can be established.

Use only these comparability labels:

- DIRECTLY_COMPARABLE
- PARTIALLY_COMPARABLE
- NOT_DIRECTLY_COMPARABLE

For CLAIM_SUPPORT, use only these study-contribution labels:

- DIRECT_SUPPORT
- INDIRECT_SUPPORT
- DIRECT_INCONCLUSIVE_EVIDENCE
- CONTRARY_EVIDENCE
- NO_DIRECT_BEARING

Use DIRECT_INCONCLUSIVE_EVIDENCE when a study directly measures
claim-relevant evidence but its result is too limited, imprecise, or
inconclusive to materially support or oppose the claim.

Do not convert non-significance, limited-condition testing, or
incomplete direct evidence into CONTRARY_EVIDENCE without sufficient
claim alignment.

Study-contribution labels must be supported by the extracted finding,
not merely by topical or methodological alignment with the claim.

Do not assign DIRECT_SUPPORT solely because a study:

- uses the requested material or intervention;
- studies the requested organism or population;
- measures a claim-relevant outcome; or
- is otherwise directly relevant to the claim.

DIRECT_SUPPORT requires an extracted finding that materially supports
the specific claim.

If a study directly investigates the claim-relevant outcome but the
direction or result cannot be verified from the available extraction
basis, do not infer a positive finding.

Use DIRECT_INCONCLUSIVE_EVIDENCE when the study is directly relevant but
the available evidence does not permit a defensible support-versus-
contrary classification.

Topical relevance or direct study alignment must never be converted
into an unverified positive result.

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


### Final integration preflight

Before rendering the final answer, perform a final integrity check across
retrieval, extraction, appraisal, and synthesis.

#### Counter-evidence retrieval preflight

Before declaring a claim-focused search ADEQUATE or applying a stopping
reason, perform a deliberate counter-evidence retrieval check.

A search that retrieves supporting studies is not sufficient by itself
to establish adequate claim-level retrieval.

For CLAIM_SUPPORT work, conduct at least one additional retrieval pass
designed to detect evidence that may oppose, fail to support, or
materially limit the claim.

Use complementary strategies when appropriate, including:

- a broad material/population query without requiring positive-effect
  terminology;
- negative or null-result terminology such as:
  `no inhibition`, `no effect`, `not effective`, `ineffective`,
  `resistant`, `no antibacterial activity`, or equivalent terms;
- title-mismatch retrieval where the title may emphasize another
  organism, outcome, or comparison even though the target evidence is
  reported in the abstract, keywords, tables, or full text;
- targeted follow-up of relevant records discovered during earlier
  search iterations.

Do not assume that a study is irrelevant merely because its title does
not foreground the target organism or because the target finding is
negative.

For example, an article whose title emphasizes Gram-negative bacteria
may still contain direct native-chitosan evidence for
Staphylococcus aureus and must be screened if the organism appears in
the record or study content.

If directly relevant contrary or inconclusive evidence is found, retain
and classify it using the existing controlled study-contribution labels.

If no contrary evidence is found, report that no such evidence was
identified in the performed retrieval; do not convert failure to retrieve
contrary evidence into proof that contrary evidence does not exist.

Do not use `ADEQUATE`, `ADEQUATE_RETRIEVAL`, `NO_MATERIAL_IMPROVEMENT`,
or `USER_SCOPE_REACHED` to stop a claim-focused search until this
counter-evidence retrieval check has been completed.

The purpose of this check is retrieval balance, not forced symmetry:
supporting and contrary evidence do not need to occur in equal numbers.

#### Independent counter-evidence discovery requirement

A counter-evidence check is not complete when all retrieval attempts are
minor variants of the supporting search that preserve the same target
terms and retrieval pathway.

For claim-focused searches with plausible title-mismatch risk, use at
least two complementary counter-evidence discovery strategies.

Strategy 1 — target-preserving, effect-neutral retrieval:

- retain the intervention, material, exposure, or phenomenon;
- retain the target organism, population, or outcome context;
- remove any requirement for a positive-effect term.

Strategy 2 — target-relaxed title-mismatch retrieval:

- retain the intervention, material, exposure, or phenomenon;
- remove the target organism or population term from at least one query;
- use broad domain, experimental, antimicrobial, null-result, or other
  context terms as appropriate;
- screen candidate abstracts, keywords, methods, results, tables, or
  full text for the target organism, population, or outcome.

The second strategy is required because a study may contain directly
relevant target evidence even when the target is absent from its title
or from the principal emphasis of the record.

For example, a study whose title emphasizes Gram-negative bacteria may
still contain direct experimental results for Staphylococcus aureus.

When feasible, counter-evidence discovery should also use more than one
retrieval channel, such as:

- a bibliographic index; and
- publisher, journal, repository, or scholarly full-text discovery.

Do not treat repeated searches through the same retrieval pathway as
independent counter-evidence discovery merely because individual query
terms differ.

If only one meaningful retrieval channel is available, report the
source limitation explicitly.

Any plausible contrary, null, inconclusive, or title-mismatch candidate
identified during any search iteration must remain in the candidate
ledger until it is screened or explicitly resolved.

Do not silently drop such a candidate when later queries return a
different evidence set.

A claim-focused search must not receive final `ADEQUATE` status merely
because:

- supporting evidence is abundant;
- negative terminology was technically tested;
- a counter-evidence iteration was recorded; or
- condition-dependent limitations were found.

The counter-evidence check must make a genuine attempt to discover
directly contrary or inconclusive evidence through a retrieval pathway
that is meaningfully different from the supporting search.

If no directly contrary evidence is found after the complementary
passes, report only that none was identified in the performed retrieval.

Do not infer that no contrary evidence exists.

Final `ADEQUATE` diagnosis and stopping decisions require completion of
both the target-preserving and target-relaxed counter-evidence discovery
strategies, unless a documented source limitation prevents one of them.

#### Citation-neighborhood counter-evidence expansion

For claim-focused searches, complementary keyword retrieval may still
miss relevant counter-evidence when the target organism, population,
outcome, or finding is not foregrounded in the article title or indexed
terms.

When both Strategy A and Strategy B have been completed but the retained
evidence set remains uniformly supportive or no direct contrary evidence
has been identified, perform an additional discovery step before final
search adequacy:

**Strategy C — citation-neighborhood expansion**

Strategy C must generate candidates through a discovery relationship
that is materially different from another keyword-query variation.

Acceptable Strategy C pathways include:

- backward reference screening from directly relevant primary studies;
- backward reference screening from relevant reviews used only as
  discovery sources;
- forward citation screening of important primary studies;
- related-article or similar-article discovery from a scholarly index;
- citation-network or reference-neighborhood discovery available through
  a publisher, bibliographic database, or scholarly search system.

A review identified during this process may be used to discover primary
studies but must not replace primary evidence when primary evidence is
required.

Strategy C is not completed by:

- adding another synonym to Strategy A or Strategy B;
- removing another keyword while using the same ranked keyword-search
  pathway;
- repeating the same broad query through another interface;
- merely searching explicit negative terminology.

When screening citation-neighborhood candidates, do not require the
article title to foreground the target organism, population, or outcome.

Inspect the abstract, keywords, methods, results, tables, figures, or
full text when available to determine whether the target is actually
tested.

Every plausible contrary, null, inconclusive, claim-limiting, or
title-mismatch record discovered through Strategy C must enter the
candidate ledger and remain there until explicit resolution.

If Strategy C cannot be performed because the available source or tool
does not expose citation, related-record, reference-list, or comparable
discovery functionality, document that limitation explicitly.

Do not silently treat another keyword query as a substitute for
citation-neighborhood discovery.

For claim-focused searches with a uniformly supportive retrieved set,
do not finalize `ADEQUATE` merely because Strategy A and Strategy B were
technically completed.

Final adequacy should follow Strategy C when citation-neighborhood
discovery is feasible.

If no directly relevant contrary evidence is identified after the
completed discovery strategies, report only that none was identified in
the performed retrieval.

Do not interpret failure to retrieve contrary evidence as evidence that
contrary evidence does not exist.

#### Candidate-ledger handoff integrity

A counter-evidence candidate ledger must remain consistent with the
downstream evidence set.

When a candidate is resolved as:

`retained as evidence`

the same scholarly study must appear in the downstream selected
literature or evidence set unless its resolution is explicitly revised
and the reason for that revision is reported.

When a candidate is retained as claim-limiting, contrary, inconclusive,
or otherwise synthesis-relevant evidence, preserve that evidence unit in
the appropriate downstream evidence record rather than allowing it to
disappear after retrieval.

Do not label a candidate `retained as evidence` if it will subsequently
be omitted from the selected evidence set without explanation.

Candidate resolution must therefore remain traceable across:

candidate ledger
→ screening decision
→ selected literature
→ extraction when performed
→ synthesis when performed.

A downstream omission is allowed only when the record is explicitly
resolved as:

- `EXCLUDED` with reason;
- `UNVERIFIED`;
- duplicate or overlapping record;
- outside claim scope after screening.

Do not silently change a candidate's resolution between retrieval and
downstream reporting.

#### Unique evidence-unit integrity

A scholarly study must appear only once as an evidence unit in the
selected literature unless the source itself contains genuinely
separable studies or datasets that the workflow explicitly treats as
distinct evidence units.

Multiple verification sources do not create multiple evidence units.

For example:

- publisher verification;
- PubMed verification;
- repository full text;
- PMC full text;
- Crossref metadata

may all support the same article identity, but the article remains one
evidence unit.

Do not create a second selected-literature row merely to represent:

- full-text verification;
- cross-channel verification;
- an alternate access route;
- an additional bibliographic source;
- the same DOI, PMID, PMCID, title, or study record.

Instead, consolidate verification and access information into the single
study record.

Before finalizing the selected literature, check for duplicate evidence
units using available stable identifiers such as:

- DOI;
- PMID;
- PMCID;
- exact article title;
- other stable scholarly identifiers.

If two records resolve to the same scholarly study, merge them unless
there is a defensible reason to treat them as separate evidence units.

Evidence-unit counts in Search quality must be based on unique evidence
units after this deduplication check.

#### Retained-set reconciliation preflight

Before finalizing the report, reconcile the candidate ledger against all
downstream evidence records.

Construct the retained-candidate set from every candidate whose final
resolution is:

`retained as evidence`

Then verify that every member of that retained set appears in the
downstream selected evidence set.

For each retained candidate, verify traceability across all downstream
stages that are performed:

candidate ledger
→ screening decision
→ selected literature
→ extraction
→ appraisal when performed
→ synthesis when performed.

A candidate must not be described as `retained as evidence` while being
absent from selected literature.

Likewise, do not state that a study "remains selected" in screening notes
if it is absent from the selected evidence set.

If further screening changes the decision, revise the candidate ledger
before finalizing the report.

For example:

`retained as evidence`

may be revised to:

- `EXCLUDED` with reason;
- `UNVERIFIED`;
- duplicate or overlapping record;
- outside claim scope after screening.

The revised resolution must be visible and must replace the earlier
retained resolution.

Do not leave contradictory resolutions in different report sections.

Before reporting:

`Unique evidence-unit check: PASS`

verify both conditions:

1. no scholarly study is duplicated as more than one selected evidence
   unit; and
2. every candidate resolved as `retained as evidence` is represented by
   exactly one downstream selected evidence unit.

If either condition fails, do not report:

`Unique evidence-unit check: PASS`

The unique selected evidence-unit count must be calculated only after
this reconciliation is complete.

The final count must equal the number of deduplicated selected evidence
units after all retained-candidate handoffs and resolution revisions have
been completed.

#### Cross-layer resolution consistency

Before final output, compare candidate-resolution statements across:

- counter-evidence candidate ledger;
- screening notes;
- selected literature;
- extraction;
- appraisal;
- claim-support map;
- search-quality counts.

The same scholarly study must not simultaneously be represented as:

- retained in one section and omitted without explanation in another;
- retained in one section and excluded in another without an explicit
  arm-level or study-level distinction;
- selected in screening notes but absent from selected literature;
- counted as a unique evidence unit without a selected-literature record.

When a mixed-comparison study contains both eligible native evidence and
excluded derivative or formulation arms, distinguish explicitly between:

`study-level resolution`

and:

`arm-level resolution`

Excluding a derivative arm does not exclude the whole study when a
separately extractable native arm remains retained.

Conversely, retaining a native arm means the study must remain traceable
as a selected evidence unit.

Do not finalize the report until these cross-layer representations are
internally consistent.

#### Controlled-label integrity

Render controlled labels exactly as defined.

Evidence status must be exactly one of:

- CONFIRMED
- PROBABLE
- UNVERIFIED
- EXCLUDED

DOI verification must use only the allowed DOI-verification labels.

Full-text access must be exactly one of:

- Open access
- Free full text
- Subscription/paywalled
- Status not verified

Do not append explanations inside a controlled-label field.

For example, do not write:

`EXCLUDED from the core evidence set`

in an evidence-status field.

Instead write:

`EXCLUDED`

and place the explanation in a separate reason field.

#### Appraisal-completeness integrity

When STRUCTURED_SCOUT_APPRAISAL is active, appraisal must be performed
and rendered separately for every unique selected evidence unit that is
eligible for appraisal.

Do not replace missing per-study appraisals with a collective statement
such as:

"the remaining abstract-only studies were treated as NOT_VERIFIED"

or equivalent summary language.

For every selected evidence unit, report:

- study identity;
- appraisal mode;
- appraisal basis;
- all nine Scout appraisal domains;
- exactly one permitted judgment for each domain.

The nine Scout appraisal domains are:

1. Experimental object / material characterization
2. Comparator / control adequacy
3. Experimental-condition transparency
4. Replication / repeatability reporting
5. Outcome-measurement appropriateness
6. Attribution of observed effect
7. Statistical-analysis reporting
8. Completeness / consistency of reported outcomes
9. Reproducibility-relevant methodological detail

Use only these domain judgments:

- `ADEQUATELY_ADDRESSED`
- `PARTIALLY_ADDRESSED`
- `NOT_ADDRESSED`
- `NOT_VERIFIED`
- `NOT_APPLICABLE`

A limited appraisal basis does not remove the requirement for a
per-study appraisal record.

For example, an `ABSTRACT_ONLY` study may legitimately have several
domains judged `NOT_VERIFIED`, but the study must still have its own
nine-domain appraisal record when STRUCTURED_SCOUT_APPRAISAL is active.

Likewise, a `METADATA_ONLY` study must not be silently omitted from
appraisal merely because methodological detail is limited.

Use `NOT_VERIFIED` whenever the available appraisal basis does not
support a stronger judgment.

A cross-study appraisal summary may be added only after all required
per-study appraisal records have been completed.

A cross-study summary must never replace the required per-study
appraisals.

Before synthesis, reconcile:

unique selected evidence units
→ required per-study appraisal records.

The completion condition is:

`selected evidence units requiring appraisal`
=
`completed per-study appraisal records`

Each unique selected evidence unit must map to exactly one appraisal
record.

Multiple discovery, verification, access, or duplicate records for the
same scholarly study do not require multiple appraisals.

Before finalizing synthesis, report appraisal as complete only when
every selected study requiring appraisal has exactly one explicit
per-study appraisal record.

If the counts differ, appraisal is incomplete and the report must not
proceed as though appraisal completion has been satisfied.

Do not create combined domain labels such as:

`ADEQUATELY_ADDRESSED to PARTIALLY_ADDRESSED`.

#### Comparability-rendering integrity

Comparability labels describe relationships among evidence units
relative to the intended synthesis target.

Do not render DIRECTLY_COMPARABLE, PARTIALLY_COMPARABLE, or
NOT_DIRECTLY_COMPARABLE as an intrinsic property of an individual study.

In a study-level claim-support map, report the study's:

`Comparability group / context`

rather than assigning the study itself a comparability label.

Place the controlled comparability judgment at the pairwise or
comparability-group level.

#### Quantitative-context integrity

Every extracted quantitative result must remain linked to the
experimental context in which it was reported.

Preserve, where applicable:

- material/preparation;
- organism and strain;
- assay;
- medium;
- concentration;
- timepoint;
- comparator/control;
- outcome definition;
- subgroup or experimental condition.

If the same paper reports different numerical values for the nominally
same outcome under different tables, conditions, experiments, or
subgroups, do not select one as a universal value.

Report the values separately with their conditions.

If the context of a value cannot be established, use the appropriate
NOT_VERIFIED terminology rather than collapsing or reconciling the
values.

#### Cross-location quantitative consistency

When FULL_TEXT extraction contains quantitative outcomes, do not stop
after locating the first apparently relevant value.

Before finalizing a quantitative result, cross-check the inspected
article for other reported values of the same nominal outcome in:

- tables;
- main-text results;
- figures;
- supplementary material when inspected;
- separate experimental series;
- subgroup or strain comparisons.

If the same study reports different values for the same nominal outcome,
do not assume that one value supersedes the other merely because it
appears later in the article.

Preserve each reported value together with:

- source location such as table, figure, or text;
- organism and strain;
- material/preparation;
- medium or experimental condition when available;
- timepoint;
- experiment or comparison context;
- number or type of determinations when reported.

For example:

`Table 1 / SG511 / CAMHB / MBC / 62.5 μg/mL / at least three determinations`

and:

`Table 3 / SG511 parent strain / MBC / 31.3 μg/mL / two determinations`

must remain separate records unless the source explicitly states that
one value corrects, replaces, or supersedes the other.

Do not explain a numerical discrepancy by assigning it to another
strain, subgroup, condition, or experiment unless the source supports
that attribution.

When the reason for differing values cannot be established, report the
difference transparently and use:

`Quantitative context: NOT_VERIFIED`

where appropriate.

A downstream synthesis table or claim-support map must not select one
of multiple context-dependent values as the study's universal result.

When a concise synthesis table cannot display all values, write:

`Multiple context-specific values reported; see detailed extraction.`

and preserve the complete values in the detailed extraction.

#### Extraction-basis traceability

FULL_TEXT may be used only when the full article content was actually
inspected.

ABSTRACT_ONLY and METADATA_ONLY must not be expanded with details that
require unavailable full text.

Extraction basis and appraisal basis must be reported independently.

#### Clean-link preflight

Before final output, remove tracking parameters from user-facing source
links.

Remove parameters such as:

- utm_source
- utm_medium
- utm_campaign
- tracking identifiers
- referral parameters

Prefer DOI, PMID, PMCID, or the clean canonical publisher URL.

Do not claim that tracking parameters were removed unless the
user-visible source representation is actually clean.

If a clickable canonical URL cannot be guaranteed to remain unmodified
by the client, interface, or rendering layer, prefer a stable scholarly
identifier rather than presenting a tracking-bearing URL as a clean
canonical URL.

Preferred fallbacks include:

- DOI;
- PMID;
- PMCID;
- source name plus stable identifier;
- canonical URL rendered as plain or code text when necessary.

Do not treat interface-added tracking parameters as part of the
scholarly source identity.

When a clean clickable destination cannot be guaranteed, report the
stable identifier or plain canonical target without claiming that a
rendered hyperlink is tracking-free.


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

### Aggregate report reconciliation

Before finalizing Search quality, reconcile every reported aggregate
count against the final deduplicated study-level records in:

- Selected literature;
- Screening notes;
- candidate-ledger final resolutions;
- DOI-verification fields;
- full-text-access fields;
- domain-specific classifications when used.

Do not calculate Search-quality counts from memory, search-result
totals, discovery records, or intermediate candidate lists.

Calculate aggregate counts only after:

1. candidate resolutions are final;
2. retained-set reconciliation is complete;
3. duplicate scholarly records have been merged;
4. study-level and arm-level resolutions have been separated;
5. Selected literature is final.

Use the following counting rules.

#### Unique selected evidence units

`Unique selected evidence units`

equals the number of deduplicated scholarly studies represented in the
final Selected literature table.

Multiple publisher, PubMed, PMC, repository, Crossref, or rediscovery
records for the same study count once.

#### Confirmed studies

`Confirmed studies`

equals the number of unique selected evidence units whose final
Evidence status is exactly:

`CONFIRMED`

Do not include PROBABLE, UNVERIFIED, or EXCLUDED records.

#### Probable studies

`Probable studies`

equals the number of unique study-level records whose final evidence
state is exactly:

`PROBABLE`

Do not count the same scholarly study twice if it appears in more than
one report location.

#### Unverified records

`Unverified records`

equals the number of unique study-level records whose final evidence
state is exactly:

`UNVERIFIED`

A NOT_VERIFIED extraction or appraisal field does not make the whole
study UNVERIFIED.

#### Excluded records

`Excluded records`

equals the number of unique scholarly study-level records whose final
evidence state is:

`EXCLUDED`

Do not count an excluded experimental arm as an excluded scholarly study
when the study-level resolution remains:

`retained as evidence`

For mixed-comparison studies, arm-level exclusions remain arm-level
records and must not inflate the study-level EXCLUDED count.

#### Verified DOI

`Verified DOI`

equals the number of unique scholarly records whose DOI-verification
field uses one of:

- `Verified — Publisher`
- `Verified — Crossref`
- `Verified — PubMed`
- `Verified — Multiple authoritative sources`

A study with:

`Not verified`

does not contribute to the Verified DOI count.

Multiple authoritative verification sources for one DOI still count as
one verified DOI record.

#### Confirmed open/full-text articles

`Confirmed open/full-text articles`

equals the number of unique selected scholarly studies whose Full-text
access field is exactly:

- `Open access`; or
- `Free full text`

Do not count:

- `Subscription/paywalled`;
- `Status not verified`.

Do not infer open/full-text availability from extraction basis.

For example:

`FULL_TEXT`

does not automatically mean:

`Open access`

or:

`Free full text`.

The count must be derived from the controlled Full-text access field in
the final Selected literature record.

#### Domain-specific classification counts

When a domain-specific summary is reported, reconcile each category
against the final study-level classification.

For mixed-comparison studies, distinguish:

- study-level classification; and
- arm-level classification.

A study containing both an eligible native arm and an ineligible
derivative, formulation, nanoparticle, chitooligosaccharide, or other arm
must not be silently counted as purely native if the reporting taxonomy
defines it as a mixed-comparison study.

Likewise, the ineligible arm must not create an additional scholarly
study count.

#### Aggregate reconciliation gate

Before final output, compare the calculated aggregate counts with the
numbers rendered in Search quality.

Report:

`Aggregate report reconciliation: PASS`

only when all reported aggregate counts match the final reconciled
study-level records.

At minimum reconcile:

- Unique selected evidence units;
- Confirmed studies;
- Probable studies;
- Unverified records;
- Excluded records;
- Verified DOI;
- Confirmed open/full-text articles;
- retained-candidate counts;
- domain-specific classification counts when reported.

If any reported count differs from the underlying final records, do not
report:

`Aggregate report reconciliation: PASS`

Correct the underlying report or the aggregate count before finalizing.

A discrepancy must not be explained away while leaving contradictory
numbers in the final report.