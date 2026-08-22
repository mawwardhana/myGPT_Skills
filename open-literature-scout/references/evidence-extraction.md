# Evidence Extraction Rules

## Purpose

Use evidence extraction to characterize the methods, samples,
interventions, outcomes, and findings of studies that have passed
literature screening.

Evidence extraction must remain faithful to the information supported
by the inspected scholarly source.

Do not fill missing study details from assumptions or general knowledge.

## Extraction modes

Use only these extraction modes:

### BASIC

Use BASIC by default for routine literature scouting when the user
primarily asks to:

- find articles;
- identify primary studies;
- verify DOI information;
- locate supporting literature;
- obtain a short evidence list.

In BASIC mode, the Selected literature table in
`assets/output-template.md` is sufficient.

Detailed study characterization is not required.

### DETAILED

Use DETAILED when the user asks to:

- extract study characteristics;
- compare methods or results across studies;
- build an evidence table;
- summarize intervention, exposure, population, or outcomes;
- identify study limitations;
- support a manuscript discussion or literature review;
- characterize evidence in greater methodological detail.

When DETAILED mode is used, follow:

`assets/evidence-extraction-template.md`

Do not activate DETAILED mode merely because more information is
available.

## Evidence eligibility rule

Detailed extraction should normally be performed for CONFIRMED studies.

PROBABLE studies may be extracted only when useful to the user's
request, but their unresolved status must remain clearly visible.

Do not present UNVERIFIED records as established extracted evidence.

EXCLUDED studies do not require detailed extraction unless the user
specifically asks why they were excluded.

Evidence extraction must not change an article's evidence status.

## Extraction basis

For every detailed extraction, report one of these labels:

- FULL_TEXT
- ABSTRACT_ONLY
- METADATA_ONLY

### FULL_TEXT

Use when study content was inspected from the article full text.

### ABSTRACT_ONLY

Use when substantive study information was extracted only from the
abstract.

Do not imply that methods, limitations, or numerical details were
checked in the full article.

### METADATA_ONLY

Use when only bibliographic or publisher metadata was available.

Do not use METADATA_ONLY to make detailed claims about study findings.

## Source preference

For study-content extraction, prefer:

1. article full text from the publisher or trusted repository;
2. authoritative full-text database;
3. abstract from publisher or PubMed;
4. bibliographic metadata.

Use bibliographic databases primarily for identity verification when a
more complete study source is available.

Do not merge unsupported details from unrelated secondary sources into
a primary-study extraction.

## Required detailed extraction fields

When DETAILED mode is active, extract when applicable:

- Study design
- Setting / context
- Population / object / sample
- Sample size
- Intervention / exposure / phenomenon
- Comparator / control
- Study duration / timepoint
- Outcome(s)
- Methods / assays / instruments
- Main findings
- Quantitative result(s)
- Author-reported limitations
- Relevance to the research question
- Extraction notes

Use the terminology that best matches the study design.

For example:

- laboratory studies may use object, strain, assay, concentration, and
  control;
- clinical studies may use population, intervention, comparator, and
  outcome;
- observational studies may use population, exposure, comparator, and
  outcome;
- qualitative studies may use participants, phenomenon, context,
  data-collection method, and themes.

Do not force clinical terminology onto laboratory or qualitative
studies.

## Missing-information labels

Use only these labels when a detailed extraction field cannot be
populated:

### NOT_REPORTED

Use when the inspected source is sufficiently complete for the field
but the information is not reported.

### NOT_VERIFIED

Use when the information may exist in the article but the available
source does not allow it to be verified.

Example:

An abstract-only source does not report sample size, but the full text
was not inspected.

Use:

`NOT_VERIFIED`

rather than assuming that the article did not report it.

### NOT_APPLICABLE

Use when the field does not logically apply to the study.

Example:

A comparator may be NOT_APPLICABLE in a single-group qualitative
study.

Do not use blank cells for required detailed extraction fields.

## Source-fidelity rule

Extract only information that is supported by the inspected source.

Do not convert:

- growth reduction into MIC;
- association into causation;
- statistical significance into clinical importance;
- absence of statistical significance into proof of no effect;
- an author's hypothesis into an observed result.

Preserve the distinction between:

- what the study measured;
- what the study found;
- what the authors concluded.

## Numerical-integrity rule

Preserve reported:

- units;
- denominators;
- concentration units;
- timepoints;
- effect measures;
- uncertainty measures;
- statistical measures;

when they are relevant to the user's question.

Do not silently convert or normalize numerical results.

If a calculation is performed from reported data at the user's request,
label it:

`Derived calculation`

and distinguish it from a value directly reported by the article.

Do not invent missing numerical values.

### Condition-linked quantitative extraction

A numerical value must not be detached from the experimental condition
that produced it.

When a source reports more than one value for the same nominal outcome,
preserve each distinct value together with its context.

For example:

| Condition | Outcome | Value |
|---|---|---|
| Medium A, 24 h | MIC | value |
| Medium B, 24 h | MIC | value |
| Parent strain, experiment 1 | MBC | value |
| Parent strain, experiment 2 | MBC | value |

Do not silently select one value as the representative result when
another value is reported under a different experimental condition,
table, subgroup, or experiment.

Do not average, reconcile, or infer equivalence between such values
unless the source explicitly provides that analysis.

If the distinction cannot be verified, report the ambiguity and use
NOT_VERIFIED where appropriate.

### Cross-location quantitative consistency

For FULL_TEXT extraction, quantitative verification must include a
cross-location check within the inspected article.

Do not finalize a numerical outcome after locating only the first
apparently relevant value.

For each claim-relevant quantitative outcome, check other inspected
locations where the same nominal outcome may also be reported,
including:

- tables;
- main-text results;
- figures;
- supplementary material when inspected;
- separate experimental series;
- subgroup or strain comparisons.

When the same study reports different numerical values for the same
nominal outcome, preserve each value as a separate context-linked
record unless the source explicitly states that one value corrects,
replaces, or supersedes another.

Each retained quantitative record should preserve, when available:

- source location;
- organism and strain;
- material or preparation;
- assay;
- medium or experimental condition;
- concentration or dose;
- timepoint;
- experiment or comparison context;
- number or type of determinations;
- reported numerical value and unit.

Do not resolve a discrepancy by guessing that one value belongs to a
different strain, subgroup, condition, or experiment.

Such attribution is allowed only when supported by the source.

If the source reports different values but the reason for the
difference cannot be verified, retain the values separately and state:

`Quantitative context: NOT_VERIFIED`

Do not average, reconcile, prioritize, or silently choose one of the
values.

A concise downstream table may summarize the study as:

`Multiple context-specific values reported; see detailed extraction.`

but the detailed extraction must preserve all verified context-specific
values.

For example, if one article reports:

`Table 1 / S. aureus SG511 / MBC / 62.5 μg/mL`

and elsewhere reports:

`Table 3 / S. aureus SG511 parent strain / MBC / 31.3 μg/mL`

both values must remain visible unless the article explicitly states
that one supersedes the other.

## Multiple-group rule

When a study contains multiple relevant groups, interventions,
concentrations, organisms, or comparators, do not collapse materially
different findings into one generalized statement.

Report group-specific findings when the distinction affects
interpretation.

For example, distinguish:

- native chitosan vs derivative;
- treatment vs control;
- different concentrations;
- different bacterial species;
- different patient subgroups.

## Outcome-integrity rule

Use the outcome actually measured by the study.

Do not substitute a related but different outcome merely because it
better matches the user's question.

When several outcomes are reported, prioritize outcomes directly
relevant to the research question and note important secondary outcomes
when useful.

## Limitation-integrity rule

Under:

`Author-reported limitations`

report only limitations explicitly stated or clearly acknowledged by
the study authors.

Do not present an inferred weakness as an author-reported limitation.

If the user explicitly asks for critical appraisal or your own
interpretation, separate inferred limitations under:

`Scout inference`

and clearly identify them as interpretation rather than author-reported
content.

## Finding-versus-relevance rule

Keep these fields conceptually separate:

### Main findings

Report what the study found.

### Relevance to the research question

Explain why those findings matter to the user's specific question.

Do not replace factual study findings with interpretive relevance.

## Cross-study comparability rule

Do not imply that results are directly comparable when studies use
materially different:

- populations;
- assays;
- concentrations;
- follow-up durations;
- outcome definitions;
- measurement instruments;
- effect measures.

When comparison is useful but methodological heterogeneity is present,
state the limitation explicitly.

Do not rank studies solely by the numerical magnitude of incompatible
outcomes.

## Extraction consistency rule

Before finalizing detailed extraction, cross-check:

- article identity;
- evidence status;
- extraction basis;
- study design;
- sample information;
- intervention/exposure/phenomenon;
- comparator/control;
- outcomes;
- numerical findings;
- limitations;
- relevance statement.

The detailed extraction must remain consistent with the Selected
literature record.

## Evidence integrity rule

Evidence extraction characterizes selected studies.

It does not independently determine:

- evidence status;
- DOI verification;
- study inclusion;
- study exclusion;
- search diagnosis;
- search stopping reason.

Continue to follow `SKILL.md` and all relevant reference files for
those decisions.