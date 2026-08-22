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
| Search iteration used | |
| Query or search logic | |
| Source actually searched | |
| Positive-effect terminology removed | |
| Negative/null terminology tested | |
| Title-mismatch candidates screened | |
| Material change from the pass | |

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