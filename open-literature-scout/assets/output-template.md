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
| Candidate ledger maintained | |
| Candidate ledger resolution status | |
| Material change from the passes | |

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

### Counter-evidence candidate ledger

Report each plausible counter-evidence or title-mismatch candidate that
was retained during refinement until resolution.

| Candidate | Why retained | Discovery strategy | Verification status | Final resolution | Downstream evidence record |
|---|---|---|---|---|---|
| | | | | | |

Candidate-handoff integrity check:

Any candidate resolved as:

`retained as evidence`

must have a corresponding downstream evidence record.

Candidates retained as contrary, claim-limiting, inconclusive, or other
synthesis-relevant evidence must also remain traceable into the
downstream evidence set.

Do not allow a candidate to disappear after retrieval without an explicit
resolution.

If a candidate's final screening decision changes, update both:

- `Final resolution`; and
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
3. candidate-ledger records have been resolved or explicitly retained as
   unresolved;
4. the material effect of the counter-evidence passes has been reported.

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
  rows; and
- every candidate marked `retained as evidence` is traceable to a
  downstream evidence record.

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

Confirmed studies:  
Probable studies:  
Unverified records:  
Excluded records:  
Verified DOI:  
Confirmed open/full-text articles:  
Unresolved verification issues:

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

### Domain-specific summary

If a domain-specific reference file was used, report any additional
classification counts or quality indicators required by that reference.

If no domain-specific reference was used, omit this subsection.