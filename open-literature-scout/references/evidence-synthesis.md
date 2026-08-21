# Evidence Synthesis Rules

## Purpose

Use evidence synthesis to determine what can legitimately be concluded
across multiple studies or evidence units after relevant evidence has
been identified, extracted, and, when appropriate, appraised.

Evidence synthesis is conceptually separate from:

- literature retrieval;
- evidence status;
- bibliographic verification;
- DOI verification;
- evidence extraction;
- study-level methodological appraisal;
- formal certainty-of-evidence assessment;
- quantitative meta-analysis.

Evidence synthesis asks:

"What can the available evidence set collectively support?"

## Synthesis modes

Use only these synthesis modes:

### NONE

Use when the user requests:

- routine literature scouting;
- DOI or bibliographic verification;
- study-level extraction;
- study characterization;
- methodological appraisal;

without asking for a cross-study conclusion or claim-level evidence
judgment.

Comparing study characteristics does not automatically activate evidence
synthesis.

### NARRATIVE_SYNTHESIS

Use when the user asks:

- what several studies collectively show;
- whether findings are consistent across studies;
- how results differ across studies;
- for a narrative evidence synthesis;
- for an integrated interpretation of multiple studies.

This mode synthesizes the evidence set without requiring one predefined
claim.

### CLAIM_SUPPORT

Use when:

- the user provides a scientific claim and asks whether evidence
  supports it;
- the user asks what evidence supports a particular statement;
- the user wants to know whether a manuscript conclusion is supported by
  the available literature;
- a precise claim must be mapped to supporting, indirect, contrary, or
  non-bearing evidence.

## Evidence-set rule

Define the evidence set before synthesis.

For every evidence unit considered, preserve:

- article identity;
- study design;
- evidence status;
- population / organism / object;
- intervention / exposure / phenomenon;
- comparator when relevant;
- outcome;
- methods / assay;
- relevant findings;
- appraisal information when available.

Do not silently add studies to the synthesis that were not previously
identified with a clear record status.

### Evidence-state handling

CONFIRMED evidence may contribute directly to synthesis.

PROBABLE evidence may be discussed when useful, but its unresolved status
must remain explicit.

UNVERIFIED evidence must not be treated as established support for a
claim.

EXCLUDED evidence must not contribute to the substantive synthesis unless
the user specifically asks why it was excluded.

Evidence synthesis does not change evidence status.

## Comparability gate

Before combining study findings narratively, assess whether the evidence
units are sufficiently comparable for the intended conclusion.

Use only these comparability labels:

- DIRECTLY_COMPARABLE
- PARTIALLY_COMPARABLE
- NOT_DIRECTLY_COMPARABLE

### DIRECTLY_COMPARABLE

Use when the evidence units are sufficiently aligned on the dimensions
that materially determine interpretation of the requested claim.

Relevant dimensions may include:

- population / organism;
- intervention / exposure / material;
- formulation;
- comparator;
- assay / method;
- outcome definition;
- effect measure;
- timepoint / duration;
- experimental conditions.

DIRECTLY_COMPARABLE does not mean identical in every detail.

### PARTIALLY_COMPARABLE

Use when studies address substantially the same claim but differ on one
or more important methodological or contextual dimensions.

Narrative comparison is possible, but the differences must remain
explicit.

### NOT_DIRECTLY_COMPARABLE

Use when major differences in method, population, intervention,
formulation, outcome, or effect measure prevent direct comparison.

Such studies may still contribute to a broader narrative synthesis, but
their numerical results must not be treated as being on one common
scale.

## Comparability-group rule

Do not force all studies into one synthesis group.

A comparability group normally contains two or more evidence units.

Do not assign a comparability label to a single evidence unit by
comparing the study with itself.

When an evidence unit does not fit a meaningful multi-study
comparability group, retain it as an unclustered or singleton evidence
unit.

A singleton evidence unit:

- remains part of the evidence set when otherwise eligible;
- may contribute to later narrative synthesis or claim support;
- must not be labelled DIRECTLY_COMPARABLE merely because no second
  study is present;
- should not receive a within-group comparability judgment until another
  relevant evidence unit is available for comparison.

Comparability labels describe relationships among evidence units
relative to the intended synthesis target; they are not intrinsic
quality labels assigned to individual studies.

When material differences exist, create comparability groups or clusters.

Possible grouping dimensions include:

- native material versus derivative;
- solution versus film/formulation/composite;
- organism or strain;
- clinical versus laboratory evidence;
- MIC/MBC versus diffusion-zone outcomes;
- exposure duration;
- assay type;
- population context.

Synthesize within the most comparable groups first.

Only then describe relationships across groups.

Do not calculate a common average across incompatible groups.

## Claim decomposition rule

When a user claim contains materially distinct assertions, decompose it
before evaluating support.

For example:

"Chitosan is effective, safe, and superior to antibiotics."

must be decomposed into separate claims concerning:

1. antibacterial effectiveness;
2. safety;
3. superiority to antibiotics.

Each claim must have its own relevant evidence set.

Do not transfer evidence supporting one component to another component.

## Study-contribution rule

In CLAIM_SUPPORT mode, classify each evidence unit according to its
relationship to the specific claim.

Use only:

- DIRECT_SUPPORT
- INDIRECT_SUPPORT
- DIRECT_INCONCLUSIVE_EVIDENCE
- CONTRARY_EVIDENCE
- NO_DIRECT_BEARING

### DIRECT_SUPPORT

Use when the study directly measures evidence relevant to the claim in a
sufficiently aligned population, intervention, and outcome.

### INDIRECT_SUPPORT

Use when the study contributes mechanistic, contextual, adjacent, or
otherwise relevant information but does not directly test the exact
claim.

### DIRECT_INCONCLUSIVE_EVIDENCE

Use when the study directly investigates a claim-relevant population,
intervention/material, and outcome, but the observed evidence does not
materially support or oppose the claim because interpretation remains
inconclusive or too narrowly bounded.

Examples include:

- a directly relevant outcome tested only under a limited condition
  that does not cover the broader claim;
- an estimated effect that is too imprecise to distinguish meaningful
  effect from no effect;
- a directly relevant experiment whose result cannot responsibly be
  classified as either support or contrary evidence.

DIRECT_INCONCLUSIVE_EVIDENCE is not:

- DIRECT_SUPPORT;
- CONTRARY_EVIDENCE;
- evidence of no effect;
- NO_DIRECT_BEARING.

The study must directly measure evidence relevant to the claim.

If the relevant outcome was not measured, use NO_DIRECT_BEARING rather
than DIRECT_INCONCLUSIVE_EVIDENCE.

If the study directly tests conditions aligned with the claim and the
finding materially opposes the claim, use CONTRARY_EVIDENCE instead.

### CONTRARY_EVIDENCE

Use when a sufficiently relevant study reports a finding that materially
opposes the claim under the studied conditions.

Do not use CONTRARY_EVIDENCE merely because:

- an outcome was not measured;
- a result was not statistically significant;
- available information is insufficient.

### NO_DIRECT_BEARING

Use when the study does not materially inform the specific claim.

A study may be scientifically relevant to the broader topic while still
having NO_DIRECT_BEARING on a particular claim.

## Claim-assessment rule

For CLAIM_SUPPORT mode, use only these claim-level assessment labels:

- SUPPORTED
- QUALIFIED_SUPPORT
- MIXED_EVIDENCE
- INSUFFICIENT_EVIDENCE
- NOT_SUPPORTED

### SUPPORTED

Use when sufficiently direct and relevant evidence consistently supports
the claim within a clearly defined scope and no major unresolved
contradiction materially changes the conclusion.

SUPPORTED is not a formal certainty grade.

### QUALIFIED_SUPPORT

Use when the claim receives meaningful direct support but the conclusion
requires important qualification because of:

- methodological limitations;
- partial comparability;
- heterogeneous conditions;
- limited populations or strains;
- formulation differences;
- indirect evidence;
- unresolved attribution;
- restricted generalizability.

### MIXED_EVIDENCE

Use when sufficiently relevant evidence units provide materially
different or opposing findings that cannot be adequately explained by
known methodological or contextual differences.

Do not label evidence MIXED merely because studies used different
methods or conditions.

### INSUFFICIENT_EVIDENCE

Use when the evidence set is too limited, indirect, heterogeneous,
unverified, or methodologically incomplete to support or reject the
claim responsibly.

INSUFFICIENT_EVIDENCE does not mean no effect exists.

### NOT_SUPPORTED

Use when relevant direct evidence has been examined but does not provide
adequate support for the claim.

NOT_SUPPORTED does not mean the claim has been proven false.

## Claim-assessment independence rule

Synthesis labels are internal evidence-synthesis judgments.

Do not translate them into formal certainty-of-evidence grades.

For example:

SUPPORTED

does not mean:

- high certainty;
- GRADE high;
- definitive evidence.

QUALIFIED_SUPPORT does not mean moderate certainty.

MIXED_EVIDENCE does not mean low certainty.

A formal certainty framework requires a separate explicit workflow.

## No vote-counting rule

Do not determine the strength of evidence merely by counting studies.

Do not conclude:

"8 of 10 studies were positive, therefore the evidence is strong."

Do not convert the number of supporting studies into a percentage
quality or certainty score.

Counts may be reported descriptively when useful, but interpretation
must also consider:

- directness;
- comparability;
- study design;
- methodological appraisal;
- outcome relevance;
- population / organism;
- experimental conditions;
- study overlap.

Do not assume that multiple weak or indirect studies outweigh one highly
direct study merely because they are more numerous.

## Appraisal-integration rule

When methodological appraisal is available, incorporate it narratively
into synthesis.

Do not convert appraisal judgments into numerical study weights.

Do not assign values such as:

- ADEQUATELY_ADDRESSED = 1;
- PARTIALLY_ADDRESSED = 0.5;
- Low risk = 3;
- High risk = 1.

Instead explain how methodological strengths or concerns affect
interpretation of each study's contribution.

Evidence appraisal and evidence synthesis remain distinct.

## Evidence-overlap rule

Check whether apparently separate publications represent independent
evidence units.

Potential overlap may include:

- the same patient cohort;
- the same experimental dataset;
- companion publications;
- follow-up publications;
- subgroup or secondary analyses;
- conference and full-paper versions;
- systematic reviews containing the same primary studies.

Do not double-count overlapping evidence as independent confirmation.

When overlap is established, describe it explicitly.

When overlap may exist but cannot be verified, report:

`Study overlap: NOT_VERIFIED`

Do not treat a systematic review and all of its included primary studies
as completely independent evidence without accounting for overlap.

## Directness rule

Match the synthesis conclusion to the scope of the evidence.

Do not generalize:

in-vitro evidence

into:

clinical effectiveness.

Do not generalize:

one bacterial strain

into:

all strains of the species.

Do not generalize:

native material

into:

all derivatives or formulations.

Do not generalize:

one assay outcome

into:

all possible antibacterial outcomes.

The conclusion must retain material population, intervention, outcome,
and contextual boundaries.

## Heterogeneity-versus-conflict rule

Distinguish heterogeneous findings from genuinely conflicting evidence.

Different results may be explainable by:

- concentration;
- formulation;
- molecular characteristics;
- medium;
- strain;
- population;
- assay;
- outcome definition;
- duration;
- experimental conditions.

When differences are plausibly explained by these factors, describe the
evidence as condition-dependent or heterogeneous rather than
automatically MIXED_EVIDENCE.

Use MIXED_EVIDENCE only when materially opposing findings remain after
relevant differences have been considered.

## Negative-result integrity rule

Distinguish:

- outcome not measured;
- outcome measured but no effect detected;
- statistically non-significant result;
- inconclusive result;
- information not available;
- evidence insufficient to determine effect.

Do not collapse all of these into:

"negative study."

A non-significant result does not automatically prove no effect.

Failure to measure an outcome is not evidence that the outcome is absent.

When a study directly measures a claim-relevant outcome but its result
is too imprecise, inconclusive, or limited in scope to materially
support or oppose the claim, use:

`DIRECT_INCONCLUSIVE_EVIDENCE`

when applicable.

Do not use NO_DIRECT_BEARING merely because a directly relevant study
fails to support the broader claim.

Preserve the tested condition explicitly.

For example, absence of inhibition at one low concentration may define a
condition-specific boundary without establishing absence of activity at
higher concentrations.

## Finding-versus-synthesis rule

Preserve the distinction between:

### Study finding

What an individual study reports.

### Synthesis interpretation

What can be concluded across the evidence set.

Do not rewrite a synthesis judgment as if it were the conclusion of an
individual study.

Do not attribute a scout synthesis conclusion to study authors.

## Quantitative-synthesis boundary

Evidence synthesis in this module is narrative unless a separate
quantitative-synthesis workflow is explicitly invoked.

Do not calculate:

- pooled effects;
- pooled means;
- weighted averages;
- standardized pooled effects;
- meta-analytic confidence intervals;
- heterogeneity statistics;
- meta-regression;
- numerical study weights.

Do not present informal arithmetic pooling as meta-analysis.

## Synthesis-limitations rule

Every active synthesis should identify limitations that materially
affect interpretation.

Examples may include:

- small evidence set;
- indirect evidence;
- methodological concerns;
- partial comparability;
- outcome heterogeneity;
- formulation heterogeneity;
- unresolved study overlap;
- limited populations or strains;
- unavailable full text;
- incomplete appraisal.

Do not invent limitations that are unsupported by the evidence set.

## Bottom-line synthesis rule

The final synthesis must state:

1. what the evidence supports;
2. under what scope and conditions;
3. important qualifications;
4. what the evidence does not establish.

Avoid stronger wording than the evidence set supports.

## Synthesis consistency rule

Before finalizing synthesis, cross-check:

- evidence-set membership;
- evidence states;
- article identities;
- comparability labels;
- comparability groups;
- study contribution labels;
- appraisal information;
- overlap status;
- claim-assessment label;
- bottom-line conclusion.

No study may influence the synthesis without a traceable role in the
evidence set.

## Evidence integrity rule

Evidence synthesis does not independently change:

- evidence status;
- DOI verification;
- inclusion/exclusion decisions;
- extraction basis;
- appraisal mode or judgment;
- search diagnosis;
- search stopping reason.

Continue to follow `SKILL.md` and all relevant reference files.