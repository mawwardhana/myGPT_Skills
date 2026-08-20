# Open Literature Scout — Changelog

## v0.8

### Added
- Evidence synthesis as a distinct post-extraction and post-appraisal
  workflow.
- NONE, NARRATIVE_SYNTHESIS, and CLAIM_SUPPORT synthesis modes.
- Study comparability classification using DIRECTLY_COMPARABLE,
  PARTIALLY_COMPARABLE, and NOT_DIRECTLY_COMPARABLE.
- Comparability-group clustering before cross-study interpretation.
- DIRECT_SUPPORT, INDIRECT_SUPPORT, CONTRARY_EVIDENCE, and
  NO_DIRECT_BEARING study-contribution labels.
- SUPPORTED, QUALIFIED_SUPPORT, MIXED_EVIDENCE,
  INSUFFICIENT_EVIDENCE, and NOT_SUPPORTED claim-assessment labels.
- Claim decomposition for compound scientific claims.
- No-vote-counting safeguard.
- Study-overlap and double-counting safeguards.
- Directness and generalizability safeguards.
- Heterogeneity-versus-conflict distinction.
- Negative-result integrity rules.
- Narrative integration of methodological appraisal without numerical
  weighting.
- Explicit boundary between narrative synthesis and quantitative
  meta-analysis.
- Evidence-synthesis output template.

### Preserved
- Evidence-status independence.
- Evidence extraction and numerical integrity.
- Study-level evidence appraisal.
- Replication-integrity safeguards.
- Formal-tool version and completion safeguards.
- No-universal-quality-score rule.
- Clean scholarly link handling.
- Mandatory six-section output contract.


## v0.7.2

### Fixed
- Clarified that an untreated control does not automatically establish
  adequate control structure when a potentially active treatment vehicle
  lacks a matched vehicle-only control.
- Separated the consequences of a missing matched vehicle control for
  control adequacy and attribution of effect.
- Added a fallback that reports stable scholarly identifiers rather than
  reproducing tracked browsing URLs.
- Reinforced placement of question-framework selection under Search
  strategy.

### Preserved
- Evidence-status independence.
- DETAILED evidence extraction.
- STRUCTURED_SCOUT_APPRAISAL.
- User-provided appraisal basis.
- Replication-integrity safeguards.
- Formal-tool routing and completion safeguards.
- No-universal-quality-score rule.


## v0.7.1

### Fixed
- Added `USER_PROVIDED_INFORMATION` as a controlled appraisal-basis
  label for appraisal based on user-supplied study information.
- Prevented `NOT_VERIFIED` from being used as an appraisal-basis label.
- Separated comparator/control adequacy from attribution of observed
  effects in laboratory studies.
- Clarified that an active solvent control may still be an adequate
  control while limiting attribution of the treatment effect.

### Preserved
- Evidence-status independence.
- Formal-tool routing and version integrity.
- Structured Scout Appraisal domains.
- Replication-integrity safeguards.
- No-universal-quality-score rule.


## v0.7

### Added
- Evidence-appraisal routing by study design.
- NONE, FORMAL_TOOL, and STRUCTURED_SCOUT_APPRAISAL modes.
- Separation of evidence status from methodological trustworthiness.
- Formal-tool version and status verification.
- RCT routing to RoB 2.
- Non-randomized intervention routing to ROBINS-I.
- Diagnostic-accuracy routing to QUADAS-3.
- Systematic-review routing to AMSTAR 2.
- Design-appropriate JBI routing.
- Structured scout appraisal for laboratory/in-vitro studies.
- Replication-integrity and statistical-appraisal rules.
- Separation of study-reported information from appraisal judgment.
- Evidence-appraisal template.

### Preserved
- Evidence extraction from v0.6.2.
- Numerical and multiple-group integrity.
- Search refinement and stopping logic.
- Question-framework selection.
- DOI verification and clean-link rules.
- Domain-specific screening.


## v0.6.2

### Fixed
- Enforced clean source links in the mandatory output template.
- Prevented tracking parameters such as `utm_source`, `utm_medium`,
  and `utm_campaign` from appearing in reported source URLs.

### Preserved
- DETAILED extraction integration from v0.6.1.
- Controlled search-stopping labels.
- Evidence extraction and integrity rules from v0.6.


## v0.6.1

### Fixed
- Preserved the six mandatory top-level output sections during DETAILED
  evidence extraction.
- Required detailed extraction to remain nested under Selected
  literature.
- Enforced controlled search-stopping reason labels in the output
  template.

### Preserved
- Evidence extraction rules from v0.6.
- Numerical integrity.
- Multiple-group extraction.
- Cross-study comparability.
- Source fidelity.
- Limitation integrity.


## v0.6

### Added
- Conditional BASIC and DETAILED evidence-extraction modes.
- Structured study characterization.
- Extraction-basis labels for full-text, abstract-only, and metadata-only evidence.
- Controlled missing-information labels.
- Source-fidelity rules.
- Numerical-integrity rules.
- Multiple-group extraction rules.
- Outcome-integrity rules.
- Author-reported limitation handling.
- Cross-study comparability rules.
- Detailed evidence-extraction template.

### Preserved
- Search refinement and stopping logic from v0.5.
- Question-framework selection.
- Boolean sensitivity rules.
- Evidence decision states.
- DOI verification.
- Domain-specific screening.
- Result consistency checking.

## v0.5

### Added
- Iterative search-refinement workflow.
- Controlled search-diagnosis labels.
- Query broadening and narrowing rules.
- Terminology-gap detection.
- Source-limitation handling.
- Search-iteration history.
- Search stopping rules.
- Result-count integrity rule.
- Query-comparison rule.

### Preserved
- Question-framework selection from v0.4.1.
- Framework-to-search translation rules.
- Boolean sensitivity rules.
- Evidence decision states.
- DOI verification.
- Domain-specific screening.
- Result consistency checking.


## v0.4.1

### Fixed
- Preserved experiential and perceptual meaning when translating PICo
  and SPIDER questions into searchable concepts.
- Clarified that OR-based synonym expansion generally increases search
  sensitivity.
- Clarified that additional AND-based concept blocks generally reduce
  search sensitivity.
- Added guidance for combining overlapping framework elements when
  separate Boolean blocks would unnecessarily restrict retrieval.

### Regression issues addressed
- PCC Boolean sensitivity.
- PICo qualitative phenomenon translation.


## v0.4

### Added
- Question-framework selection.
- PICO support for intervention/effectiveness questions.
- PECO support for exposure and association questions.
- PCC support for scoping and evidence-mapping questions.
- PICo support for qualitative questions.
- SPIDER support for qualitative and mixed-method searches.
- NONE option for searches that do not require a formal framework.
- Framework-to-search translation rules.

### Preserved
- Evidence decision states from v0.3.2.
- DOI verification rules.
- Domain-specific screening rules.
- Result consistency checking.


## v0.3.2 — Baseline Stable

Status: Baseline stable.

### Added
- Derivative inclusion rule.
- Result consistency rule.

### Fixed
- Derivative-only studies are no longer automatically excluded.
- Articles cannot appear in recommendations or conclusions without
  a prior record status.

### Regression tests passed
- Mechanistic primary-study inclusion.
- Chitosan formulation/composite inclusion.
- Chitosan derivative secondary-evidence handling.
- Result consistency checking.

## v0.3.1
- Added formulation inclusion rule.

## v0.3
- Added evidence decision states.
- Added domain-specific chitosan classification.
- Added controlled reporting vocabulary.
- Added ranking rules.
- Added source-use integrity rules.

## v0.2
- Added DOI verification.
- Added mandatory structured output.

## v0.1
- Initial literature-search workflow.