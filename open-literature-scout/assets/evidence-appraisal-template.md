# Evidence Appraisal Template

Use this template only when methodological appraisal is requested.


## Output integration rule

When this template is used with the mandatory output contract, do not
emit the file title as an additional report heading.

All appraisal content must remain inside:

`## 4. Selected literature`

Begin the rendered appraisal content with:

`### Appraisal control`

Use `###` for appraisal subsections and `####` for headings nested
within those subsections.

Do not create any additional top-level `##` section between:

`## 4. Selected literature`

and:

`## 5. Screening notes`


### Appraisal control

| Field | Value |
|---|---|
| Evidence status | |
| Study design | |
| Appraisal mode | |
| Appraisal approach/tool | |
| Tool version | |
| Tool status | |
| Appraisal basis | |

Allowed appraisal modes:

- NONE
- FORMAL_TOOL
- STRUCTURED_SCOUT_APPRAISAL

For formal tools, preserve the judgment terminology required by the
official tool.

Do not replace official tool terminology with generic scout labels.


Allowed appraisal-basis labels:

- FULL_TEXT
- ABSTRACT_ONLY
- METADATA_ONLY
- USER_PROVIDED_INFORMATION

Use `USER_PROVIDED_INFORMATION` when the appraisal relies only on study
details supplied directly by the user.

Do not use `NOT_VERIFIED` as an appraisal-basis label.


### Study-reported methodological information

Summarize only information supported by the inspected study source.

| Methodological feature | Study-reported information |
|---|---|
| Design | |
| Sampling / experimental object | |
| Allocation / grouping | |
| Comparator / control | |
| Blinding / masking | |
| Replication | |
| Outcome measurement | |
| Missing/incomplete data | |
| Statistical analysis | |
| Protocol / prespecification | |
| Other relevant information | |

Use:

- NOT_REPORTED
- NOT_VERIFIED
- NOT_APPLICABLE

when appropriate.

### Formal-tool appraisal

Use this subsection only when:

**Appraisal mode: FORMAL_TOOL**

Report the official tool's domains and judgments using the official
terminology.

Do not reproduce the full official checklist unless permitted and
necessary.

| Official domain | Judgment | Support for judgment |
|---|---|---|
| | | |

**Overall official judgment:**  

If the official tool cannot be completely applied, report:

`FORMAL_APPRAISAL_NOT_COMPLETED`

and explain why.

### Structured scout appraisal

Use this subsection only when:

**Appraisal mode: STRUCTURED_SCOUT_APPRAISAL**

State explicitly:

> STRUCTURED_SCOUT_APPRAISAL is a transparent methodological assessment
> used by this skill and is not a validated formal risk-of-bias
> instrument.

#### Mandatory per-study appraisal

Render this structured scout appraisal separately for every evidence
unit being appraised.

For each study, explicitly report:

**Study:** [study identifier]

**Appraisal mode:** STRUCTURED_SCOUT_APPRAISAL

**Appraisal basis:** FULL_TEXT / ABSTRACT_ONLY / METADATA_ONLY /
USER_PROVIDED_INFORMATION

Then assess all nine Scout domains in the table below.

Use exactly one allowed domain label per study per domain:

- ADEQUATELY_ADDRESSED
- PARTIALLY_ADDRESSED
- NOT_ADDRESSED
- NOT_VERIFIED
- NOT_APPLICABLE

Do not replace study-level appraisal with a single aggregate appraisal
of the whole evidence set.

A cross-study methodological summary may be added only after all
required study-level appraisals have been completed.

Do not create combined or ranged labels such as:

`ADEQUATELY_ADDRESSED to PARTIALLY_ADDRESSED`

| Scout appraisal domain | Judgment | Basis |
|---|---|---|
| Experimental object / material characterization | | |
| Comparator and control adequacy | | |
| Experimental-condition transparency | | |
| Replication / repeatability reporting | | |
| Outcome-measurement appropriateness | | |
| Attribution of the observed effect | | |
| Statistical-analysis reporting | | |
| Completeness and consistency of reported outcomes | | |
| Reproducibility-relevant methodological detail | | |

Use only:

- ADEQUATELY_ADDRESSED
- PARTIALLY_ADDRESSED
- NOT_ADDRESSED
- NOT_VERIFIED
- NOT_APPLICABLE

#### Overall methodological appraisal

Provide a narrative synthesis.

Do not calculate a total score.

Do not label the result as an official risk-of-bias judgment.

### Appraisal implications

#### Methodological strengths

- 

#### Methodological concerns

- 

#### Implication for the research question

Explain how the appraisal affects confidence in using this study to
answer the user's question.

Do not change the article's evidence status merely because
methodological concerns are present.

### Appraisal notes

Clearly separate:

- study-reported facts;
- formal-tool judgments;
- scout interpretation.

## Appraisal completion reconciliation

Use this reconciliation when:

**Appraisal mode: STRUCTURED_SCOUT_APPRAISAL**

and more than one unique selected evidence unit requires appraisal.

Every unique selected evidence unit requiring appraisal must have one
explicit per-study appraisal record.

Each per-study appraisal record must include:

- study identity;
- appraisal mode;
- appraisal basis;
- all nine Scout appraisal domains;
- exactly one permitted judgment for each domain.

Do not omit an appraisal record merely because the study is:

- `ABSTRACT_ONLY`;
- `METADATA_ONLY`; or
- otherwise limited in methodological detail.

Use `NOT_VERIFIED` for domains that cannot be defensibly assessed from
the available appraisal basis.

Do not replace missing study-level appraisal records with a collective
statement about several studies.

Before synthesis, report:

**Selected evidence units requiring appraisal:**  
**Completed per-study appraisal records:**  
**Missing per-study appraisal records:**  

The required relationship is:

`Selected evidence units requiring appraisal`
=
`Completed per-study appraisal records`

and:

`Missing per-study appraisal records`
=
`0`

Multiple discovery, verification, publisher, PubMed, PMC, repository,
or other access records for the same scholarly study count as one
evidence unit and therefore require only one appraisal record.

Report:

`Per-study appraisal completion: PASS`

only when every unique selected evidence unit requiring appraisal has
exactly one explicit per-study appraisal record.

Otherwise report:

`Per-study appraisal completion: FAIL`

Do not proceed to evidence synthesis as though appraisal were complete
when this reconciliation fails.

When this template is rendered inside the mandatory literature report,
keep the reconciliation inside:

`## 4. Selected literature`

and render it as a subsection such as:

`### Appraisal completion reconciliation`

Do not create an additional mandatory top-level report section.