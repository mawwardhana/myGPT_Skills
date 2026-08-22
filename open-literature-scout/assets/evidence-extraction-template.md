# Detailed Evidence Extraction Template

Use this template only when:

**Evidence extraction mode: DETAILED**

## Output integration rule

When this template is used with the mandatory output contract in
`assets/output-template.md`, all detailed evidence extraction content
must remain inside:

`## 4. Selected literature`

Use:

`### Detailed Evidence Extraction`

for the detailed extraction heading.

Do not create a new top-level `##` section between:

`## 4. Selected literature`

and:

`## 5. Screening notes`

Any interpretation, limitation separation, cross-study characterization,
or evidence judgment generated from detailed extraction must use
subheadings within Section 4.

The six mandatory top-level sections defined in `SKILL.md` must remain
unchanged.

Create one extraction block for each study.

## Study: [Article title]

| Field | Extracted information |
|---|---|
| Evidence status | |
| Extraction basis | |
| Study design | |
| Setting / context | |
| Population / object / sample | |
| Sample size | |
| Intervention / exposure / phenomenon | |
| Comparator / control | |
| Study duration / timepoint | |
| Outcome(s) | |
| Methods / assays / instruments | |
| Main findings | |
| Quantitative result(s) | |
| Author-reported limitations | |
| Relevance to the research question | |
| Extraction notes | |

Use only these Extraction basis labels:

- FULL_TEXT
- ABSTRACT_ONLY
- METADATA_ONLY

For unavailable required information, use only:

- NOT_REPORTED
- NOT_VERIFIED
- NOT_APPLICABLE

Do not leave required extraction fields blank.

Repeat the study block for every study included in detailed extraction.

## Cross-study characterization

After individual extraction, provide this summary when two or more
studies are extracted:

| Article | Study design | Population/Object | Intervention/Exposure/Phenomenon | Main outcome | Main finding | Main limitation | Relevance |
|---|---|---|---|---|---|---|---|

### Comparability note

Briefly state whether major differences in:

- population;
- methods;
- interventions/exposures;
- outcomes;
- measurement conditions;

limit direct comparison across the extracted studies.

Do not imply quantitative comparability when study methods or outcomes
are materially different.

## Quantitative-result context record

When FULL_TEXT extraction identifies quantitative results, preserve each
materially distinct reported value together with its source location and
experimental context.

Use one record per context-specific value:

| Field | Extracted information |
|---|---|
| Outcome | |
| Reported value | |
| Unit | |
| Source location | |
| Organism / strain | |
| Material / preparation | |
| Assay | |
| Medium / experimental condition | |
| Concentration / dose | |
| Timepoint | |
| Experiment / comparison context | |
| Determinations / replication context | |
| Quantitative context note | |

If the same nominal outcome is reported more than once in different
tables, figures, text passages, experimental series, subgroups, strains,
or conditions, create separate records rather than selecting one value.

Example:

| Field | Record 1 | Record 2 |
|---|---|---|
| Outcome | MBC | MBC |
| Reported value | 62.5 μg/mL | 31.3 μg/mL |
| Source location | Table 1 | Table 3 |
| Organism / strain | S. aureus SG511 | S. aureus SG511 parent strain |
| Experiment / comparison context | Table 1 susceptibility experiment | Table 3 parent-strain comparison |
| Determinations / replication context | At least three determinations | Two determinations |

Do not infer that one value replaces the other unless the source
explicitly states that it is a correction, replacement, or superseding
result.

If the reason for the discrepancy cannot be verified, retain both values
and state:

`Quantitative context: NOT_VERIFIED`

In concise downstream synthesis tables, do not select one
context-dependent value as the study-wide result.

Instead use:

`Multiple context-specific values reported; see detailed extraction.`

when all values cannot be shown without loss of context.