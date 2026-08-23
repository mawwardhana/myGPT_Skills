# Evidence Appraisal Rules

## Purpose

Use evidence appraisal to evaluate the methodological trustworthiness,
risk of bias, or methodological limitations of studies that have already
been identified and characterized.

Evidence appraisal is conceptually separate from:

- evidence status;
- bibliographic verification;
- DOI verification;
- study inclusion;
- evidence extraction.

A CONFIRMED article is not automatically high-quality evidence.

CONFIRMED means that the article's identity, primary-study status, and
relevance have been sufficiently verified.

## Appraisal modes

Use only these appraisal modes:

### NONE

Use when the user requests routine literature scouting, bibliographic
verification, or evidence extraction without methodological appraisal.

Do not perform formal appraisal merely because an article is available.

### FORMAL_TOOL

Use when:

- the user explicitly requests risk-of-bias or methodological-quality
  appraisal; and
- an appropriate established appraisal tool exists for the study design.

When FORMAL_TOOL is used, identify the exact appraisal tool and verify
its current official version or status from an authoritative source
before applying it.

### STRUCTURED_SCOUT_APPRAISAL

Use when methodological appraisal is requested but no suitable formal
validated tool has been selected or is appropriate for the study design.

This mode may be used for laboratory or in-vitro experimental studies
when no appropriate validated formal risk-of-bias instrument is being
applied.

Always state:

"STRUCTURED_SCOUT_APPRAISAL is a transparent methodological assessment
used by this skill and is not presented as a validated formal
risk-of-bias instrument."

Do not describe this mode as RoB 2, ROBINS-I, QUADAS, JBI, AMSTAR, or
another established tool.

## Appraisal routing rule

Select the appraisal approach according to study design.

### Randomized controlled trial

Preferred formal approach:

`RoB 2`

Use the appropriate official version for the randomized design.

Examples may include:

- individually randomized parallel-group trials;
- cluster-randomized trials;
- crossover trials.

Do not use RoB 2 merely because a study contains an intervention.
Confirm that the design is randomized.

### Non-randomized study of an intervention

Preferred formal approach:

`ROBINS-I`

Before application, verify the current official version and whether it
is final or draft.

If a draft version is used, explicitly report:

`Tool status: DRAFT`

Do not silently treat a draft tool as a finalized standard.

### Diagnostic test accuracy study

Preferred formal approach:

`QUADAS-3`

Use the current official QUADAS version.

For comparative diagnostic-accuracy questions, determine whether an
appropriate comparative extension is also required according to current
official guidance.

### Systematic review of healthcare interventions

Preferred formal approach:

`AMSTAR 2`

Do not calculate or invent a numerical total quality score when the
tool itself does not support such scoring.

### Other quantitative or qualitative study designs

When appropriate, use the current official JBI critical appraisal tool
matching the study design.

Examples may include:

- cohort study;
- case-control study;
- analytical cross-sectional study;
- quasi-experimental study;
- prevalence study;
- qualitative study;
- case series;
- case report.

Verify the current official JBI tool before use.

Do not assume that one JBI checklist applies to all designs.

### Laboratory / in-vitro experimental study

Do not automatically apply a clinical risk-of-bias tool.

When no validated domain-appropriate formal appraisal tool has been
specified, use:

`STRUCTURED_SCOUT_APPRAISAL`

and clearly disclose its non-validated status.

## Tool-version integrity rule

Formal appraisal tools may be revised over time.

Before applying a named formal tool:

1. verify the current official tool;
2. identify the tool version when available;
3. identify whether the version is final, draft, archived, or otherwise
   qualified by the official source;
4. report that status.

Do not select a tool version from memory when current verification is
possible.

## Tool-content integrity rule

Do not reproduce, rewrite, or invent the complete official checklist,
signalling questions, algorithms, or proprietary tool content from
memory.

When applying a formal appraisal tool:

- use the official tool or official guidance;
- preserve its official judgment terminology;
- do not silently modify its domains;
- do not create a hybrid tool while continuing to use the official tool
  name.

If the complete official tool cannot be inspected, do not claim that a
formal appraisal has been completed.

Use:

`FORMAL_APPRAISAL_NOT_COMPLETED`

and explain what could not be verified.

## Appraisal-source rule

Report the basis used for appraisal.

Use only:

- FULL_TEXT
- ABSTRACT_ONLY
- METADATA_ONLY
- USER_PROVIDED_INFORMATION

Formal risk-of-bias appraisal should normally require sufficient study
detail, usually from FULL_TEXT.

Use `USER_PROVIDED_INFORMATION` when appraisal is based only on study
information supplied directly by the user rather than on an inspected
scholarly source.

When `USER_PROVIDED_INFORMATION` is used:

- do not imply that the full article was inspected;
- do not convert absence from the supplied information into
  article-level `NOT_REPORTED`;
- use `NOT_VERIFIED` when information may exist in the original study
  but cannot be checked from the material supplied;
- formal appraisal should not be claimed complete unless the selected
  formal tool and sufficient study information are actually available.

Do not produce a confident formal risk-of-bias judgment from
METADATA_ONLY.

When source information is insufficient, use:

`NOT_VERIFIED`

for the affected appraisal domain or item where compatible with the
selected appraisal approach.

### Per-study appraisal rendering rule

When appraisal is active, appraisal is an evidence-unit-level
assessment.

Each appraised study must explicitly report:

`Appraisal basis: FULL_TEXT / ABSTRACT_ONLY / METADATA_ONLY /
USER_PROVIDED_INFORMATION`

followed by all nine applicable Scout domains.

Do not replace study-level appraisal with a single aggregate appraisal
of the whole evidence set.

An aggregate methodological summary may be provided only after the
individual study appraisals have been completed.

Each domain must contain exactly one allowed domain label:

- ADEQUATELY_ADDRESSED
- PARTIALLY_ADDRESSED
- NOT_ADDRESSED
- NOT_VERIFIED
- NOT_APPLICABLE

Do not create ranges, hybrid labels, averages, percentages, or
cross-study domain scores.

For ABSTRACT_ONLY or METADATA_ONLY appraisal, use NOT_VERIFIED whenever
the available source does not permit a defensible domain judgment.


## Reported-information versus judgment rule

Separate:

### Study-reported information

What the authors actually report regarding:

- design;
- randomization;
- blinding;
- controls;
- sampling;
- missing data;
- outcome measurement;
- analysis;
- protocol;
- limitations.

### Appraisal judgment

The methodological interpretation made by the formal appraisal tool or
by the scout.

Do not write a scout judgment as if it were reported by the study
authors.

## Evidence-status independence rule

Do not translate evidence states into appraisal judgments.

For example:

`CONFIRMED`

does not mean:

- low risk of bias;
- high methodological quality;
- strong evidence;
- high certainty.

Likewise:

a study with methodological concerns may still be a CONFIRMED primary
study.

## No universal quality-score rule

Do not create a universal numerical quality score across study designs.

Do not convert:

- RoB 2 judgments;
- ROBINS-I judgments;
- QUADAS judgments;
- JBI appraisal findings;
- AMSTAR 2 ratings;
- STRUCTURED_SCOUT_APPRAISAL findings;

into a single common percentage or score unless the official method
explicitly requires it.

Do not rank studies merely by counting checklist items.

## Structured scout appraisal domains

When STRUCTURED_SCOUT_APPRAISAL is used for laboratory or in-vitro
studies, assess the following methodological domains when applicable:

1. Experimental object / material characterization
2. Comparator and control adequacy
3. Experimental-condition transparency
4. Replication / repeatability reporting
5. Outcome-measurement appropriateness
6. Attribution of the observed effect
7. Statistical-analysis reporting
8. Completeness and consistency of reported outcomes
9. Reproducibility-relevant methodological detail

Use only these scout-domain labels:

- ADEQUATELY_ADDRESSED
- PARTIALLY_ADDRESSED
- NOT_ADDRESSED
- NOT_VERIFIED
- NOT_APPLICABLE

These labels are internal structured-appraisal labels.

They must not be presented as official judgments from RoB 2, ROBINS-I,
QUADAS-3, JBI, AMSTAR 2, or another validated appraisal tool.


## Control-adequacy versus attribution rule

For laboratory studies, assess control adequacy separately from
attribution of effect.

`Comparator and control adequacy` asks whether appropriate controls
needed to interpret the experiment are present and appropriately
matched.

The fact that a solvent or vehicle control itself produces a measurable
effect does not automatically make the control inadequate.

When an active solvent or vehicle is appropriately included as a
control, the control structure may still be adequately addressed.

Its measurable activity should instead be considered under:

`Attribution of the observed effect`

because the observed treatment response may reflect contributions from
both the target intervention and the solvent, vehicle, formulation, or
other active component.

Do not downgrade control adequacy solely because the control itself has
a measurable effect.

The presence of an untreated control does not automatically establish
adequate control structure when the intervention is delivered using a
potentially active solvent, vehicle, carrier, or formulation component.

When a potentially active solvent or vehicle is part of the treatment
preparation, assess whether an appropriately matched vehicle-only
control is available.

If a matched vehicle-only control is materially necessary to distinguish
the target intervention from the vehicle effect but is absent or cannot
be verified:

`Comparator and control adequacy`

should not be judged `ADEQUATELY_ADDRESSED` solely because an untreated
control is present.

Depending on the available information, use:

- PARTIALLY_ADDRESSED
- NOT_VERIFIED
- NOT_ADDRESSED

as appropriate.

The same missing vehicle control may also create a separate concern
under:

`Attribution of the observed effect`

because control adequacy and causal attribution evaluate different
methodological questions.

Therefore:

presence of an active but appropriately matched vehicle control
does not automatically reduce control adequacy;

but

absence of a materially necessary matched vehicle control may reduce
control adequacy.


## Laboratory attribution rule

For laboratory studies, explicitly examine whether the observed effect
can reasonably be attributed to the tested intervention or material.

Consider when applicable:

- solvent effects;
- vehicle effects;
- active co-ingredients;
- formulation effects;
- control performance;
- concentration differences;
- organism or strain differences;
- assay-specific limitations.

Do not attribute the entire observed effect to the target intervention
when an uncontrolled active component may contribute materially.

## Replication-integrity rule

Distinguish:

- technical replicates;
- biological replicates;
- independent experiments.

Do not describe repeated measurements as independent biological
replication unless the study supports that interpretation.

If replication type cannot be determined, use:

`NOT_VERIFIED`

## Statistical-appraisal rule

Do not infer statistical adequacy merely because a p-value is reported.

Assess only what can be supported regarding:

- statistical method;
- unit of analysis;
- replicate structure;
- uncertainty reporting;
- multiple comparisons when relevant;
- consistency between analysis and design.

Do not invent unreported statistical procedures.

## Overall-appraisal rule

For FORMAL_TOOL mode:

Use the overall judgment terminology defined by the selected official
tool.

Do not replace official judgments with an invented common label.

For STRUCTURED_SCOUT_APPRAISAL:

Do not generate a validated "overall risk of bias" label.

Instead provide:

`Overall methodological appraisal`

as a concise narrative synthesis of the domain-level observations.

Do not convert the scout-domain labels into a numerical total score.

## Cross-study appraisal rule

Do not directly compare appraisal judgments produced by different tools
as though they share one common scale.

For example:

- RoB 2 "Low risk";
- AMSTAR 2 "High confidence";
- scout-domain "ADEQUATELY_ADDRESSED";

are not interchangeable categories.

When comparing studies with different designs, describe methodological
strengths and concerns within the appropriate appraisal framework.

## Per-study appraisal completion rule

When appraisal mode is:

`STRUCTURED_SCOUT_APPRAISAL`

every unique selected evidence unit that remains eligible for appraisal
must have one explicit per-study appraisal record.

A selected study must not be omitted from appraisal merely because its
appraisal basis is limited to:

- `ABSTRACT_ONLY`; or
- `METADATA_ONLY`.

Limited source detail affects the strength of domain judgments, not the
requirement to create the appraisal record.

For each unique selected study, report:

- study identity;
- appraisal mode;
- appraisal basis;
- all nine Scout appraisal domains;
- exactly one permitted judgment for each domain.

Use `NOT_VERIFIED` for any domain that cannot be defensibly assessed from
the available appraisal basis.

Do not replace missing per-study appraisals with a collective statement
such as:

"the remaining abstract-only studies have domains treated as
NOT_VERIFIED"

or equivalent wording.

A cross-study appraisal summary may be provided only after the required
per-study appraisal records have been rendered.

### Appraisal-completion reconciliation

Before appraisal is considered complete, reconcile the deduplicated
selected evidence set against the per-study appraisal set.

Report:

`Selected evidence units requiring appraisal: [n]`

`Completed per-study appraisal records: [n]`

`Missing per-study appraisal records: [n]`

The required completion condition is:

`selected evidence units requiring appraisal`
=
`completed per-study appraisal records`

and:

`missing per-study appraisal records`
=
`0`

Each unique selected evidence unit must map to exactly one per-study
appraisal record.

Multiple:

- discovery records;
- publisher records;
- PubMed records;
- repository records;
- full-text access routes;
- duplicate search hits

for the same scholarly study must not create additional appraisal
records.

If one or more selected evidence units lack an explicit appraisal
record, appraisal is incomplete.

Do not proceed as though appraisal completion has been satisfied merely
because the available studies have been summarized collectively.

When STRUCTURED_SCOUT_APPRAISAL is active, report:

`Per-study appraisal completion: PASS`

only when every selected evidence unit requiring appraisal has exactly
one explicit per-study appraisal record.

Otherwise report:

`Per-study appraisal completion: FAIL`

## Appraisal consistency rule

Before finalizing appraisal, cross-check:

- study identity;
- study design;
- evidence status;
- extraction basis;
- appraisal mode;
- appraisal tool;
- tool version/status;
- reported study information;
- appraisal judgments;
- overall appraisal statement.

Appraisal must remain consistent with the evidence extraction.

## Evidence integrity rule

Evidence appraisal evaluates methodological trustworthiness.

It does not independently change:

- evidence status;
- DOI verification;
- inclusion/exclusion decision;
- search diagnosis;
- search stopping reason.

Continue to follow `SKILL.md` and all relevant reference files.