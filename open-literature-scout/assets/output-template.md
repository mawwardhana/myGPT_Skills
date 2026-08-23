# Open Literature Scout — Output Template

## 1. Research question

[Restate user's question]

Do not place question-framework analysis in Section 1.

Section 1 contains only the research question and any brief clarification
strictly necessary to state that question.

Question-framework selection belongs under:

`## 2. Search strategy`

and must not be moved to another mandatory section.

## 2. Search strategy

### Question framework

**Selected framework:**  
**Reason for selection:**  

| Framework element | Value | Used as searchable concept? |
|---|---|---|
| | | |

If no formal framework is required, report:

**Selected framework:** NONE

and briefly explain why a formal framework would not improve the
search.


### Core concepts

- Concept 1:
- Concept 2:
- Concept 3:




### Keywords and synonyms

| Concept | Keywords / Synonyms |
|---|---|
| Concept 1 | |
| Concept 2 | |
| Concept 3 | |

### Boolean search string

[Search string]

### Search iterations

| Iteration | Query | Source actually searched | Diagnosis | Change from previous iteration | Reason |
|---|---|---|---|---|---|
| 1 | | | | Initial search | |

Use only these Diagnosis labels:

- ADEQUATE
- TOO_BROAD
- TOO_NARROW
- TERMINOLOGY_GAP
- SOURCE_LIMITATION

If the initial query is adequate, state:

"No refinement required."

Do not report a database result count unless the source explicitly
provides it.

### Sources searched

- Source:
- Source:
- Source:


Use clean source links.

Remove tracking parameters from URLs before presenting them in the
final report.

Examples of tracking parameters that must not appear include:

- utm_source
- utm_medium
- utm_campaign

Prefer canonical publisher, database, or DOI URLs whenever available.

When a URL obtained during browsing contains tracking or session
parameters, do not reproduce the raw browsing URL in the report.

Reconstruct a clean canonical URL from a stable scholarly identifier
when this can be done without changing the resource identity.

Preferred stable identifiers include:

- DOI
- PMID
- PMCID

If a clean canonical URL cannot be guaranteed, report the source name
and stable identifier without printing the raw URL.

For example:

`PubMed — PMID 18456858`

is preferable to reproducing a tracked PubMed URL.

### Counter-evidence retrieval

For claim-focused searches, report the deliberate counter-evidence
retrieval check before the final search diagnosis and stopping decision.

| Field | Report |
|---|---|
| Counter-evidence pass performed | |
| Strategy A — target-preserving pass | |
| Strategy A query / search logic | |
| Strategy A source actually searched | |
| Positive-effect terminology removed | |
| Negative/null terminology tested | |
| Strategy B — target-relaxed title-mismatch pass | |
| Strategy B query / search logic | |
| Strategy B source actually searched | |
| Target organism / population term relaxed | |
| Title-mismatch candidates screened | |
| Retrieval-channel diversity used | |
| Strategy C triggered | |
| Strategy C — citation-neighborhood expansion | |
| Strategy C pathway used | |
| Strategy C seed study / review / scholarly record | |
| Strategy C source actually searched | |
| Strategy C new plausible candidates discovered | |
| Strategy C candidates entered candidate ledger | |
| Strategy C candidate-ledger resolution status | |
| Strategy C source limitation | |
| Candidate ledger maintained | |
| Candidate ledger resolution status | |
| Material change from the counter-evidence passes | |

For claim-focused searches with plausible title-mismatch risk, both
counter-evidence discovery strategies must be auditable:

**Strategy A — target-preserving, effect-neutral retrieval**

Retain the target organism/population and intervention/material, but
remove any requirement for positive-effect terminology.

**Strategy B — target-relaxed title-mismatch retrieval**

Retain the intervention/material but relax the target organism or
population term in at least one query so that studies whose title or
primary emphasis does not foreground the target can be discovered.

Do not describe Strategy B as completed merely because a broader synonym
for the target was used.

The target itself must be relaxed from at least one meaningful discovery
query when title-mismatch risk is relevant.

### Strategy C — citation-neighborhood expansion

When Strategy A and Strategy B have been completed but the retrieved
claim-relevant evidence remains uniformly supportive or no directly
relevant contrary evidence has been identified, report whether Strategy C
was triggered.

Strategy C must use a discovery relationship that is materially
different from another keyword-query variation.

Acceptable pathways include:

- backward reference screening from a directly relevant primary study;
- backward reference screening from a relevant review used only as a
  discovery source;
- forward citation screening;
- related-article or similar-article discovery;
- citation-network or reference-neighborhood discovery.

Report:

**Strategy C triggered:**  
**Strategy C pathway used:**  
**Seed study / review / scholarly record:**  
**Source actually exposing the citation relationship:**  
**New plausible candidates discovered:**  
**Candidates entered candidate ledger:**  
**Material effect on the evidence set:**  

Do not report Strategy C as completed when only another keyword-query
variation was performed.

The following do not independently satisfy Strategy C:

- another synonym variation;
- another broader keyword query;
- removing an additional search term;
- repeating the same keyword search through another interface;
- testing negative/null terminology alone.

When Strategy C is feasible, screen citation-neighborhood candidates
beyond the title when necessary.

A title that does not foreground the target organism, population,
outcome, or finding is not a reason to discard the candidate before
screening its accessible abstract, methods, results, tables, figures, or
full text.

Every plausible contrary, null, inconclusive, claim-limiting, or
title-mismatch candidate discovered through Strategy C must enter the
candidate ledger and remain there until explicit resolution.

If Strategy C cannot be performed because citation, related-record,
reference-list, forward-citation, or comparable discovery functionality
is unavailable, report the specific limitation rather than substituting
another keyword query.

### Counter-evidence candidate ledger

Report each plausible counter-evidence or title-mismatch candidate that
was retained during refinement until resolution.

| Candidate | Why retained | Discovery strategy | Verification status | Study-level resolution | Arm-level resolution | Downstream evidence record |
|---|---|---|---|---|---|---|
| | | | | | | |

Candidate-handoff integrity check:

Any candidate resolved as:

`retained as evidence`

must have a corresponding downstream evidence record.

Candidates retained as contrary, claim-limiting, inconclusive, or other
synthesis-relevant evidence must also remain traceable into the
downstream evidence set.

Do not allow a candidate to disappear after retrieval without an explicit
resolution.

If a candidate's final screening decision changes, update:

- `Study-level resolution`;
- `Arm-level resolution` when applicable; and
- `Downstream evidence record`.

Before finalizing the report, cross-check:

candidate ledger
→ screening resolution
→ selected literature
→ extraction when performed
→ synthesis when performed.

Every candidate marked `retained as evidence` must be accounted for.

A candidate must not disappear between search iterations without an
explicit resolution.

Allowed resolution descriptions include:

- retained as evidence;
- `EXCLUDED` with reason;
- `UNVERIFIED`;
- duplicate / overlapping record;
- outside claim scope after screening.

The candidate ledger is not an evidence-state table and does not create
new controlled evidence labels.

For claim-focused searches, final `ADEQUATE` diagnosis and stopping
decisions should only appear after:

1. Strategy A has been completed;
2. Strategy B has been completed when applicable;
3. Strategy C has been completed when triggered and feasible, or its
   specific source/tool limitation has been explicitly documented;
4. candidate-ledger records from all performed strategies have been
   resolved or explicitly retained as unresolved;
5. the material effect of the counter-evidence passes has been reported.

When Strategy A and Strategy B leave a uniformly supportive evidence set
or identify no directly relevant contrary evidence, Strategy C must be
addressed before final claim-focused search adequacy.

When `Synthesis mode` is `CLAIM_SUPPORT`, at least one search iteration
must be identifiable as the counter-evidence retrieval pass.

Do not report the search as finally `ADEQUATE` merely because supporting
studies were retrieved.

If the counter-evidence pass identifies directly relevant contrary,
inconclusive, or claim-limiting evidence, retain it for normal screening,
extraction, appraisal when applicable, comparability assessment, and
study-contribution classification.

If no directly relevant contrary evidence is identified, report only:

`No directly relevant contrary evidence was identified in the performed counter-evidence retrieval.`

Do not state or imply that contrary evidence does not exist.

For claim-focused searches, do not finalize the following stopping
reasons before the counter-evidence retrieval check is complete:

- `ADEQUATE_RETRIEVAL`
- `NO_MATERIAL_IMPROVEMENT`
- `USER_SCOPE_REACHED`

If source access prevents a meaningful counter-evidence check, report the
limitation explicitly and use the controlled stopping logic appropriate
to source limitation.

### Study-level and arm-level resolution check

For mixed-comparison studies, report separately:

**Study-level resolution**

This records whether the scholarly article as a whole is retained in the
evidence set.

**Arm-level resolution**

This records the disposition of materially distinct experimental arms.

Example:

| Level | Resolution |
|---|---|
| Study-level resolution | `retained as evidence` |
| Native chitosan arm | retained |
| Schiff-base derivative arm | `EXCLUDED` — derivative arm not eligible for native-chitosan claim |

An excluded derivative, formulation, composite, nanoparticle,
chitooligosaccharide, or other ineligible arm does not automatically
exclude the whole scholarly study when a separately extractable eligible
native arm remains.

Conversely, a study must not remain retained merely because native
chitosan is mentioned if the eligible native arm cannot be separated
from the ineligible material or active components.

When the study-level resolution is:

`retained as evidence`

the eligible study must remain traceable into selected literature and
all downstream stages that are performed.

## 3. Screening criteria

### Include

- Primary research
- Direct relevance to research question
- Bibliographic identity verifiable

### Exclude

- Review articles when primary research is requested
- Editorials
- Commentary
- Irrelevant populations or outcomes

## 4. Selected literature

| Rank | Article | Year | Journal | Study type | Evidence status | Population/Object | Main relevance | DOI | DOI verification | Full-text access | Reason selected |
|---|---|---|---|---|---|---|---|---|---|---|---|

Use only these Evidence status labels:

- CONFIRMED
- PROBABLE
- UNVERIFIED
- EXCLUDED

Use only the DOI verification labels defined in `SKILL.md`.

Use only the Full-text access labels defined in `SKILL.md`.

When a relevant domain-specific reference file requires an additional
classification field, add that field to this table without removing
the mandatory columns above.

### Retained-set reconciliation

Before finalizing selected literature, reconcile all candidate-ledger
records against the downstream evidence set.

Report:

**Retained candidates from ledger:**  
**Retained candidates represented in selected literature:**  
**Unexplained retained-candidate omissions:**  

For mixed-comparison studies, also report which eligible arm supplies the
claim-relevant evidence.

The reconciliation must satisfy:

`retained as evidence`
→ one deduplicated selected scholarly study
→ one unique evidence unit.

A study marked `retained as evidence` must not be absent from selected
literature.

A screening note must not state that a study "remains selected" when the
study is absent from selected literature.

If further screening changes the disposition of a candidate, revise the
candidate ledger before finalizing the report.

Report:

`Retained-set reconciliation: PASS`

only when:

- every study-level `retained as evidence` candidate maps to exactly one
  selected evidence unit;
- duplicate or overlapping candidates map to an existing selected
  evidence unit rather than creating another one;
- excluded, outside-scope, or unverified candidates have an explicit
  downstream resolution;
- mixed-comparison studies distinguish study-level from arm-level
  resolution;
- no contradictory resolution remains across ledger, screening notes,
  selected literature, extraction, appraisal, or synthesis.

### Unique evidence-unit check

Before finalizing selected literature, verify that each scholarly study
appears only once as an evidence unit.

Multiple scholarly records used to discover, verify, or access the same
study must be consolidated into one selected-literature row.

Do not create separate evidence-unit rows for:

- publisher verification;
- PubMed verification;
- PMC access;
- repository access;
- Crossref metadata;
- alternate full-text locations;
- rediscovery through another search strategy.

Use available stable identifiers to detect duplicates:

- DOI;
- PMID;
- PMCID;
- exact article title;
- other stable scholarly identifiers.

If multiple records resolve to the same article, merge them into one
evidence-unit record and preserve the relevant verification/access
information within that record.

A study may appear more than once only when genuinely separable studies,
datasets, cohorts, experiments, or evidence units are explicitly
documented.

Report:

`Unique evidence-unit check: PASS`

only when:

- no duplicate scholarly study remains as multiple selected-literature
  rows;
- every study-level candidate resolved as `retained as evidence` is
  represented by exactly one selected evidence unit;
- every retained candidate is traceable to its downstream evidence
  record; and
- `Retained-set reconciliation: PASS` has been satisfied.

### Evidence extraction mode

**Mode:** BASIC / DETAILED

Use BASIC for routine literature scouting when the Selected literature
table provides sufficient characterization.

Use DETAILED when the user's request requires study-level extraction or
comparison.

When DETAILED is used, follow:

`assets/evidence-extraction-template.md`

Do not omit the Selected literature table when DETAILED extraction is
performed.

Detailed extraction supplements the Selected literature record; it does
not replace it.

When DETAILED mode is active, place the detailed extraction immediately
below this subsection and keep it inside:

`## 4. Selected literature`

Use subsection headings such as:

`### Detailed Evidence Extraction`

and lower-level headings beneath it.

Do not introduce additional top-level `##` sections between Section 4
and Section 5.


### Evidence appraisal

**Appraisal mode:** NONE / FORMAL_TOOL / STRUCTURED_SCOUT_APPRAISAL

Use NONE when methodological appraisal was not requested or required.

When appraisal is performed, follow:

`assets/evidence-appraisal-template.md`

Keep all appraisal content inside:

`## 4. Selected literature`

Use subsection headings only.

Do not create a new mandatory top-level section for appraisal.

A CONFIRMED article must not be described as high quality merely because
its evidence status is confirmed.

### Appraisal completion reconciliation

When:

`Appraisal mode: STRUCTURED_SCOUT_APPRAISAL`

every unique selected evidence unit requiring appraisal must have one
explicit per-study appraisal record.

Report:

**Selected evidence units requiring appraisal:**  
**Completed per-study appraisal records:**  
**Missing per-study appraisal records:**  

The completion condition is:

`Selected evidence units requiring appraisal`
=
`Completed per-study appraisal records`

and:

`Missing per-study appraisal records`
=
`0`

Do not omit a selected study from appraisal merely because its appraisal
basis is:

- `ABSTRACT_ONLY`;
- `METADATA_ONLY`; or
- otherwise methodologically limited.

Instead, retain the per-study appraisal record and use `NOT_VERIFIED`
for domains that cannot be defensibly assessed.

Do not replace missing per-study appraisal tables with a collective
statement about the remaining studies.

Report:

`Per-study appraisal completion: PASS`

only when every unique selected evidence unit requiring appraisal has
exactly one explicit per-study appraisal record.

Otherwise report:

`Per-study appraisal completion: FAIL`

Do not proceed as though appraisal were complete when this reconciliation
fails.


### Evidence synthesis

**Synthesis mode:** NONE / NARRATIVE_SYNTHESIS / CLAIM_SUPPORT

Use NONE when no cross-study conclusion or claim-level synthesis is
required.

When synthesis is active, follow:

`assets/evidence-synthesis-template.md`

Keep all synthesis content inside:

`## 4. Selected literature`

Use subsection headings only.

Do not create a new mandatory top-level section for synthesis.

Comparing study characteristics alone does not automatically activate
evidence synthesis.

Do not determine synthesis conclusions from study counts alone.

Do not provide numerical pooling, meta-analytic estimates, or formal
certainty grades unless a separate appropriate workflow has explicitly
been applied.


## 5. Screening notes

### Excluded candidates

| Article | Evidence status | Reason for exclusion |
|---|---|---|
| | EXCLUDED | |

### Probable candidates

| Article | Evidence status | Unresolved issue |
|---|---|---|
| | PROBABLE | |

### Unverified records

| Article | Evidence status | Verification needed |
|---|---|---|
| | UNVERIFIED | |

If no records exist in a category, state:

"None identified."


## 6. Search quality

**Unique selected evidence units:** 

Evidence-unit counts must be based on deduplicated scholarly studies,
not the number of discovery, verification, or access records.

**Retained candidates from ledger:**  
**Retained candidates represented downstream:**  
**Unexplained retained-candidate omissions:**  
**Retained-set reconciliation:** 

Confirmed studies:  
Probable studies:  
Unverified records:  
Excluded records:  
Verified DOI:  
Confirmed open/full-text articles:  
Unresolved verification issues:

### Aggregate report reconciliation

Calculate Search-quality aggregates only from the final reconciled
study-level records.

Do not calculate these counts from:

- search-result totals;
- discovery records;
- duplicate publisher/PubMed/PMC records;
- intermediate candidate lists;
- memory of earlier search iterations.

Reconcile the following fields against the final Selected literature and
Screening notes:

| Aggregate field | Reconciled count | Basis checked |
|---|---:|---|
| Unique selected evidence units | | Deduplicated Selected literature |
| Confirmed studies | | Final `CONFIRMED` study-level records |
| Probable studies | | Final `PROBABLE` study-level records |
| Unverified records | | Final `UNVERIFIED` study-level records |
| Excluded records | | Final study-level `EXCLUDED` records |
| Verified DOI | | Allowed verified DOI labels |
| Confirmed open/full-text articles | | `Open access` + `Free full text` only |
| Retained candidates from ledger | | Final study-level retained candidates |
| Retained candidates represented downstream | | Reconciled selected evidence set |
| Unexplained retained-candidate omissions | | Retained-set reconciliation |

Counting rules:

**Confirmed studies**

Count only unique selected evidence units whose Evidence status is
exactly:

`CONFIRMED`

**Probable studies**

Count unique study-level records whose final Evidence status is exactly:

`PROBABLE`

**Unverified records**

Count unique study-level records whose final Evidence status is exactly:

`UNVERIFIED`

Do not count a study as UNVERIFIED merely because an extraction,
appraisal, or quantitative field contains `NOT_VERIFIED`.

**Excluded records**

Count unique scholarly studies whose final study-level evidence state is:

`EXCLUDED`

Do not count excluded experimental arms as separate excluded studies when
the scholarly study remains retained because an eligible arm exists.

**Verified DOI**

Count a unique scholarly record when its DOI-verification field is one
of:

- `Verified — Publisher`
- `Verified — Crossref`
- `Verified — PubMed`
- `Verified — Multiple authoritative sources`

Do not count:

`Not verified`

Multiple verification sources for the same study still count once.

**Confirmed open/full-text articles**

Count only unique selected studies whose Full-text access field is
exactly:

- `Open access`; or
- `Free full text`

Do not count:

- `Subscription/paywalled`;
- `Status not verified`.

Do not infer Full-text access from Extraction basis.

`FULL_TEXT` does not automatically mean `Open access` or
`Free full text`.

### Domain-classification reconciliation

When a domain-specific summary is reported, reconcile its counts against
the same final study-level evidence records.

For mixed-comparison studies, distinguish:

- study-level classification;
- arm-level classification.

A mixed-comparison study with an eligible native arm and an ineligible
derivative, formulation, nanoparticle, chitooligosaccharide, or other arm
must not be silently counted as a purely native-only study when the
domain taxonomy classifies the scholarly study as mixed comparison.

Arm-level exclusions must not create additional scholarly-study counts.

If no domain-specific classification is used, omit this subsection.

Search iterations performed:  
Final search diagnosis:  
Search stopping reason:

Use only the search stopping reason labels defined in
`references/search-refinement.md`:

- ADEQUATE_RETRIEVAL
- NO_MATERIAL_IMPROVEMENT
- SOURCE_LIMITATION_REACHED
- USER_SCOPE_REACHED

If explanation is needed, provide it separately after the controlled
label.

### Aggregate reconciliation gate

Report:

`Aggregate report reconciliation: PASS`

only when all reported aggregate counts match the final reconciled
study-level records.

At minimum verify consistency for:

- Unique selected evidence units;
- Confirmed studies;
- Probable studies;
- Unverified records;
- Excluded records;
- Verified DOI;
- Confirmed open/full-text articles;
- retained-candidate counts;
- domain-specific classification counts when reported.

If any count differs from the underlying final records, do not report:

`Aggregate report reconciliation: PASS`

Correct the underlying table, classification, or aggregate count before
finalizing the report.

Do not leave contradictory counts in the final report and explain the
difference only in prose.

### Domain-specific summary

If a domain-specific reference file was used, report any additional
classification counts or quality indicators required by that reference.

If no domain-specific reference was used, omit this subsection.