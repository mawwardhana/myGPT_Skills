# Open Literature Scout — Output Template

## 1. Research question

[Restate user's question]

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