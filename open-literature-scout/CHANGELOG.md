# Open Literature Scout — Changelog

## v0.8.11

### Fixed
- Added row-level aggregate derivation so Search-quality counts must be
  calculated from explicit reconciled study-level records rather than
  reconstructed from narrative text, search hits, or memory.
- Added a mandatory row-level reconciliation table covering study
  identity, Selected-literature membership, final evidence state,
  study-level resolution, DOI verification, Full-text access,
  study-level domain classification, retained-candidate status, and
  downstream representation.
- Required `Confirmed open/full-text articles` to equal the number of
  selected study-level rows whose Full-text access is exactly
  `Open access` or `Free full text`.
- Required `Excluded records` to be counted only from records whose final
  study-level Evidence status is exactly `EXCLUDED`.
- Prevented descriptions such as `outside claim scope`, `outside core
  evidence set`, or arm-level exclusion from being counted as
  study-level EXCLUDED unless the final Evidence status is explicitly
  normalized to `EXCLUDED`.
- Strengthened domain-specific reconciliation so aggregate
  classifications must be derived from explicit study-level
  classifications.
- Expanded the chitosan `Mixed comparison` rule beyond derivatives to
  include formulations/composites, nanoparticles, films, gels,
  chitooligosaccharides, hydrolyzed/oligomeric chitosan, grafted or
  conjugated chitosan, and other materially distinct chitosan forms.
- Required a study containing an eligible native-chitosan arm plus
  materially distinct chitosan arms to remain classified at study level
  as `Mixed comparison` when required by the domain taxonomy.
- Clarified that study-level `Mixed comparison` classification may
  coexist with a retained native-chitosan arm.
- Prevented a mixed-comparison scholarly study from being relabeled as
  `Native chitosan` merely because only its native arm contributes to
  extraction or synthesis.
- Strengthened `Aggregate report reconciliation: PASS` so it requires a
  complete row-level reconciliation table and exact agreement between
  row-derived counts and reported Search-quality aggregates.

### Preserved
- Strategy A target-preserving counter-evidence retrieval.
- Strategy B target-relaxed title-mismatch retrieval.
- Strategy C citation-neighborhood counter-evidence expansion.
- Counter-evidence candidate ledger.
- Candidate-handoff integrity.
- Retained-set reconciliation.
- Unique evidence-unit deduplication.
- Study-level versus arm-level resolution.
- Per-study STRUCTURED_SCOUT_APPRAISAL completion.
- Nine-domain Scout appraisal taxonomy.
- Controlled evidence-status, DOI-verification, and Full-text access
  vocabularies.
- Extraction-basis integrity.
- Cross-location quantitative consistency.
- Claim-contribution integrity.
- DIRECT_INCONCLUSIVE_EVIDENCE semantics.
- Negative-result safeguards.
- Comparability and overlap safeguards.
- No vote counting, numerical quality weighting, pooling, or formal
  certainty grading.
- Mandatory six-section output contract.

## v0.8.10

### Fixed
- Added Strategy C citation-neighborhood counter-evidence expansion for
  claim-focused searches whose Strategy A and Strategy B retrieval
  remains uniformly supportive or identifies no direct contrary
  evidence.
- Required Strategy C to use a materially different discovery pathway,
  such as backward references, forward citations, related-article
  discovery, or citation-network/reference-neighborhood discovery,
  rather than another keyword-query variation.
- Required citation-neighborhood candidates to enter the existing
  counter-evidence candidate ledger and remain traceable until explicit
  resolution.
- Added an explicit Strategy C completion gate before final claim-focused
  search adequacy when citation-neighborhood discovery is feasible.
- Required source/tool limitations to be documented when Strategy C
  cannot be performed.
- Strengthened per-study STRUCTURED_SCOUT_APPRAISAL completeness so every
  unique selected evidence unit requiring appraisal receives exactly one
  explicit appraisal record.
- Prevented collective statements about remaining abstract-only or
  metadata-only studies from substituting for required per-study
  appraisal records.
- Required all nine Scout appraisal domains to be rendered for every
  selected study when STRUCTURED_SCOUT_APPRAISAL is active, using
  NOT_VERIFIED where the appraisal basis does not support a stronger
  judgment.
- Added appraisal-completion reconciliation between selected evidence
  units and completed per-study appraisal records.
- Added aggregate report reconciliation for Search quality.
- Required Search-quality counts to be calculated from final,
  deduplicated, reconciled study-level records rather than search hits,
  discovery records, or intermediate candidate lists.
- Added deterministic counting rules for CONFIRMED, PROBABLE,
  UNVERIFIED, EXCLUDED, verified DOI, and confirmed open/full-text
  articles.
- Prevented excluded experimental arms in retained mixed-comparison
  studies from inflating study-level EXCLUDED counts.
- Required open/full-text counts to be derived only from the controlled
  Full-text access field, not from FULL_TEXT extraction basis.
- Added domain-classification reconciliation for mixed-comparison studies.
- Added `Aggregate report reconciliation: PASS` as a final consistency
  gate for Search-quality counts.

### Preserved
- Complementary Strategy A target-preserving counter-evidence retrieval.
- Strategy B target-relaxed title-mismatch retrieval.
- Retrieval-channel diversity.
- Counter-evidence candidate ledger.
- Study-level versus arm-level resolution.
- Retained-set reconciliation.
- Unique evidence-unit deduplication.
- Candidate-to-downstream evidence handoff.
- Exact controlled evidence-status, DOI-verification, and full-text
  access labels.
- Native-chitosan versus derivative/formulation screening integrity.
- Detailed extraction and extraction-basis rules.
- Cross-location quantitative consistency.
- Context-linked quantitative-result records.
- Per-study STRUCTURED_SCOUT_APPRAISAL nine-domain taxonomy.
- Relational comparability rendering.
- Study-overlap safeguards.
- DIRECT_SUPPORT finding-integrity requirements.
- DIRECT_INCONCLUSIVE_EVIDENCE semantics.
- Negative-result integrity.
- Condition-dependent heterogeneity safeguards.
- No vote counting, quality scoring, numerical weighting, or pooling.
- Stable scholarly identifier fallback.
- Mandatory six-section output contract.


## v0.8.9

### Fixed
- Added retained-set reconciliation before final report completion.
- Required every study-level candidate resolved as `retained as evidence`
  to map to exactly one downstream selected evidence unit.
- Prevented candidates from being retained in the ledger while silently
  disappearing from selected literature, extraction, appraisal, or
  synthesis.
- Added cross-layer resolution consistency across candidate ledger,
  screening notes, selected literature, extraction, appraisal,
  claim-support mapping, and search-quality counts.
- Added explicit distinction between study-level resolution and
  arm-level resolution for mixed-comparison studies.
- Prevented exclusion of an ineligible derivative, formulation,
  composite, nanoparticle, or other arm from silently excluding an
  otherwise eligible study-level native arm.
- Prevented a mixed-comparison study from remaining retained when its
  eligible native arm cannot be separated from ineligible material or
  active components.
- Required candidate-ledger resolution revisions to replace earlier
  retained decisions when further screening changes study eligibility.
- Required `Retained-set reconciliation: PASS` before
  `Unique evidence-unit check: PASS` can be reported.
- Required unique selected evidence-unit counts to be calculated only
  after retained-set reconciliation and deduplication are complete.
- Added retained-candidate counts, downstream representation counts,
  unexplained omission counts, and reconciliation status to Search
  quality.

### Preserved
- Independent counter-evidence discovery using complementary Strategy A
  and Strategy B.
- Retrieval-channel diversity.
- Counter-evidence candidate ledger.
- Candidate handoff and unique evidence-unit deduplication.
- Exact controlled evidence-status, DOI-verification, and full-text
  access labels.
- Native-chitosan versus derivative/formulation screening integrity.
- Detailed extraction and extraction-basis rules.
- Cross-location quantitative consistency.
- Context-linked quantitative-result records.
- Per-study STRUCTURED_SCOUT_APPRAISAL with nine domains.
- Relational comparability rendering.
- Study-overlap safeguards.
- DIRECT_SUPPORT finding-integrity requirements.
- DIRECT_INCONCLUSIVE_EVIDENCE semantics.
- Negative-result integrity.
- Condition-dependent heterogeneity safeguards.
- No vote counting, quality scoring, numerical weighting, or pooling.
- Stable scholarly identifier fallback.
- Mandatory six-section output contract.

## v0.8.8

### Fixed
- Added candidate-ledger handoff integrity from retrieval through
  downstream evidence reporting.
- Required every candidate resolved as `retained as evidence` to remain
  traceable into selected literature or another explicit downstream
  evidence record.
- Prevented contrary, claim-limiting, inconclusive, or other
  synthesis-relevant candidates from disappearing after retrieval.
- Required candidate-resolution changes to be explicitly updated rather
  than silently changing between search iterations and downstream
  reporting.
- Added unique evidence-unit integrity so one scholarly study is counted
  as one evidence unit regardless of how many discovery, verification,
  or access channels were used.
- Prevented publisher, PubMed, PMC, repository, Crossref, or alternate
  full-text records for the same article from creating duplicate
  selected-literature rows.
- Added stable-identifier-based deduplication using DOI, PMID, PMCID,
  exact article title, and other scholarly identifiers.
- Required Search quality evidence counts to use deduplicated unique
  evidence units.
- Added downstream-evidence-record traceability to the counter-evidence
  candidate ledger.
- Added an auditable `Unique evidence-unit check` to the output
  template.

### Preserved
- Independent counter-evidence discovery using complementary Strategy A
  and Strategy B.
- Retrieval-channel diversity.
- Counter-evidence candidate ledger.
- Exact controlled evidence-status and full-text-access labels.
- DOI-verification controlled labels.
- Native-chitosan versus derivative/formulation screening integrity.
- Detailed extraction and extraction-basis rules.
- Cross-location quantitative consistency.
- Context-linked quantitative-result records.
- Per-study STRUCTURED_SCOUT_APPRAISAL with nine domains.
- Relational comparability rendering.
- Study-overlap safeguards.
- DIRECT_SUPPORT finding-integrity requirements.
- DIRECT_INCONCLUSIVE_EVIDENCE semantics.
- Negative-result integrity.
- Condition-dependent heterogeneity safeguards.
- No vote counting, quality scoring, numerical weighting, or pooling.
- Stable scholarly identifier fallback.
- Mandatory six-section output contract.

## v0.8.7

### Fixed
- Added independent counter-evidence discovery requirements for
  claim-focused searches.
- Required two complementary counter-evidence strategies when
  title-mismatch risk is plausible:
  target-preserving effect-neutral retrieval and target-relaxed
  title-mismatch retrieval.
- Prevented minor variations of the supporting query from being treated
  as sufficient independent counter-evidence discovery.
- Added retrieval-channel diversity guidance so bibliographic-index and
  publisher/full-text discovery pathways are distinguished when
  feasible.
- Added a counter-evidence candidate ledger to preserve plausible
  contrary, null, inconclusive, claim-limiting, and title-mismatch
  records across search iterations until resolution.
- Prevented plausible counter-evidence candidates from disappearing
  silently when later search iterations return different evidence sets.
- Required candidate-ledger records to be resolved as retained evidence,
  EXCLUDED with reason, UNVERIFIED, duplicate/overlap, or outside claim
  scope after screening.
- Prevented final ADEQUATE diagnosis from being based solely on abundant
  supporting evidence, technically tested negative terminology, or a
  nominal counter-evidence iteration.
- Added auditable Strategy A, Strategy B, retrieval-channel diversity,
  and candidate-ledger reporting to the output template.

### Preserved
- Exact controlled evidence-status and full-text-access labels.
- DOI-verification controlled labels.
- Native-chitosan versus derivative/formulation screening integrity.
- Detailed extraction and extraction-basis rules.
- Cross-location quantitative consistency.
- Context-linked quantitative-result records.
- Per-study STRUCTURED_SCOUT_APPRAISAL with nine domains.
- Relational comparability rendering.
- Study-overlap safeguards.
- DIRECT_SUPPORT finding-integrity requirements.
- DIRECT_INCONCLUSIVE_EVIDENCE semantics.
- Negative-result integrity.
- Condition-dependent heterogeneity safeguards.
- No vote counting, quality scoring, numerical weighting, or pooling.
- Stable scholarly identifier fallback.
- Mandatory six-section output contract.

## v0.8.6

### Fixed
- Added a mandatory counter-evidence retrieval check for claim-focused
  searches before final adequacy or stopping decisions.
- Prevented supporting-study retrieval alone from being treated as
  sufficient evidence of balanced claim-level retrieval.
- Required at least one deliberate retrieval pass aimed at finding
  contrary, null, inconclusive, or claim-limiting evidence.
- Added retrieval strategies that remove positive-effect terminology
  and test negative or null-result terminology where appropriate.
- Added title-mismatch screening so directly relevant evidence is not
  missed merely because the title emphasizes another organism,
  population, comparator, outcome, or intervention arm.
- Required useful seed records from earlier iterations to be re-screened
  when they may reveal contrary or claim-limiting evidence.
- Prevented final `ADEQUATE` diagnosis and claim-focused stopping reasons
  from being applied before the counter-evidence check is complete.
- Added auditable counter-evidence retrieval reporting to the output
  template.
- Clarified that failure to retrieve contrary evidence does not establish
  that contrary evidence does not exist.

### Preserved
- Exact controlled evidence-status and full-text-access labels.
- Native-chitosan versus derivative/formulation screening integrity.
- Detailed extraction and extraction-basis rules.
- Cross-location quantitative consistency.
- Context-linked quantitative-result records.
- Per-study STRUCTURED_SCOUT_APPRAISAL with nine domains.
- Relational comparability rendering.
- Study-overlap safeguards.
- DIRECT_SUPPORT finding-integrity requirements.
- DIRECT_INCONCLUSIVE_EVIDENCE semantics.
- Negative-result integrity.
- Condition-dependent heterogeneity safeguards.
- No vote counting, quality scoring, numerical weighting, or pooling.
- Stable scholarly identifier fallback.
- Mandatory six-section output contract.

## v0.8.5

### Fixed
- Added cross-location quantitative consistency checks for FULL_TEXT
  extraction.
- Required claim-relevant numerical outcomes to be checked across
  tables, main-text results, figures, supplementary material when
  inspected, separate experimental series, and subgroup or strain
  comparisons.
- Prevented one context-specific numerical value from being selected as
  a universal study result when the same nominal outcome is reported
  differently elsewhere in the article.
- Required each differing quantitative result to remain linked to its
  source location and experimental context.
- Prohibited unsupported explanations of numerical discrepancies across
  tables, strains, subgroups, conditions, or experiments.
- Added `Quantitative context: NOT_VERIFIED` when the reason for
  differing reported values cannot be established.
- Added a dedicated quantitative-result context record to the evidence
  extraction template.
- Added synthesis-level protection against collapsing multiple
  context-specific values into one claim-support-map value.
- Added the concise fallback:
  `Multiple context-specific values reported; see detailed extraction.`

### Preserved
- Exact controlled evidence-status and full-text-access labels.
- Detailed extraction basis rules.
- Per-study STRUCTURED_SCOUT_APPRAISAL with nine domains.
- Relational comparability rendering.
- Claim-dependent comparability.
- Study-overlap safeguards.
- DIRECT_SUPPORT finding-integrity requirements.
- DIRECT_INCONCLUSIVE_EVIDENCE semantics.
- Negative-result integrity.
- Condition-dependent heterogeneity safeguards.
- No vote counting, quality scoring, numerical weighting, or pooling.
- Stable scholarly identifier fallback.
- Mandatory six-section output contract.


## v0.8.4

### Fixed
- Added study-contribution integrity so DIRECT_SUPPORT requires a
  verified extracted finding that materially supports the specific
  claim.
- Prevented direct study alignment, topical relevance, or outcome
  measurement alone from being interpreted as DIRECT_SUPPORT.
- Required directly relevant studies with unverified or indeterminate
  finding direction to use DIRECT_INCONCLUSIVE_EVIDENCE when
  appropriate.
- Added claim-support-map integrity checks linking contribution labels
  to the extracted key finding.
- Strengthened clean-link handling when interface or rendering layers
  may rewrite clickable URLs.
- Added stable-identifier fallback using DOI, PMID, PMCID, source name,
  or plain canonical target representation.
- Clarified that interface-added tracking parameters are not part of
  scholarly source identity.

### Preserved
- Exact controlled evidence-status and full-text-access labels.
- Per-study STRUCTURED_SCOUT_APPRAISAL with nine domains.
- Appraisal-basis integrity.
- Condition-linked quantitative extraction.
- Relational comparability rendering.
- Claim-dependent comparability.
- Singleton comparability integrity.
- DIRECT_INCONCLUSIVE_EVIDENCE semantics.
- Negative-result integrity.
- No-vote-counting safeguard.
- Evidence-overlap safeguards.
- Heterogeneity-versus-conflict distinction.
- Appraisal without numerical scoring.
- Claim-scope and generalizability safeguards.
- Narrative-only synthesis boundary.
- Mandatory six-section output contract.

## v0.8.3

### Fixed
- Added a final integration preflight for controlled-label integrity.
- Required exact rendering of evidence-state and full-text-access
  vocabularies.
- Required STRUCTURED_SCOUT_APPRAISAL to be rendered per evidence unit
  with explicit appraisal basis and all nine domains.
- Prevented aggregate appraisal from replacing study-level appraisal.
- Prevented comparability labels from being treated as intrinsic
  study-level properties.
- Added explicit comparability-group/context rendering for claim-support
  maps.
- Strengthened condition-linked quantitative extraction when one source
  reports multiple values for the same nominal outcome.
- Added extraction-basis traceability checks.
- Added final clean-link removal of tracking and referral parameters.

### Preserved
- Evidence-state semantics.
- DOI-verification semantics.
- Claim-dependent comparability.
- Singleton comparability integrity.
- DIRECT_INCONCLUSIVE_EVIDENCE.
- Negative-result integrity.
- No-vote-counting safeguard.
- Evidence-overlap safeguards.
- Heterogeneity-versus-conflict distinction.
- Appraisal without numerical scoring.
- Claim-scope and generalizability safeguards.
- Narrative-only synthesis boundary.
- Mandatory six-section output contract.

## v0.8.2

### Fixed
- Added `DIRECT_INCONCLUSIVE_EVIDENCE` for studies that directly
  investigate a claim-relevant outcome but cannot responsibly be
  classified as supporting or contrary evidence.
- Distinguished direct inconclusive evidence from
  `NO_DIRECT_BEARING`.
- Clarified that limited-condition no-effect findings must remain
  bounded to the tested condition.
- Clarified that non-significant or imprecise findings are not
  automatically contrary evidence.

### Preserved
- DIRECT_SUPPORT and INDIRECT_SUPPORT semantics.
- CONTRARY_EVIDENCE safeguards.
- Negative-result integrity.
- Claim-dependent comparability.
- No-vote-counting rule.
- Evidence-overlap safeguards.
- Narrative-only synthesis boundary.
- Mandatory six-section output contract.

## v0.8.1

### Fixed
- Clarified that comparability is a relationship among evidence units
  relative to an intended synthesis target.
- Prevented singleton evidence units from being labelled
  DIRECTLY_COMPARABLE by comparison with themselves.
- Added explicit handling for unclustered/singleton evidence units.
- Clarified that singleton status does not imply irrelevance, weakness,
  indirectness, or exclusion.

### Preserved
- NONE, NARRATIVE_SYNTHESIS, and CLAIM_SUPPORT modes.
- Claim-dependent comparability.
- Comparability-group clustering.
- No-vote-counting safeguard.
- Evidence-overlap safeguards.
- Heterogeneity-versus-conflict distinction.
- Narrative-only synthesis boundary.
- Mandatory six-section output contract.


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