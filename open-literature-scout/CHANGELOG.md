# Open Literature Scout — Changelog

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