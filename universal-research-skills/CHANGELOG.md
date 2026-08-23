# Changelog

All notable changes to Universal Research Skills will be documented in this file.

## [0.4.0] - Evidence & Reference Integrity Layer

### Added

- `citation-chaining` skill for expanding verified scholarly corpora through backward citations, forward citations, related-paper discovery, author lineage, theory lineage, method lineage, replication tracking, contradiction tracking, and closest-competitor discovery.
- `literature-screening` skill for creating transparent and purpose-specific eligible literature corpora using explicit inclusion and exclusion criteria.
- `evidence-synthesis` skill for integrating findings across verified and screened studies into defensible scientific conclusions.
- Backward and forward citation chaining for identifying foundational literature, replications, validations, extensions, critiques, contradictions, and subsequent scientific development.
- Citation genealogy and scientific-lineage mapping.
- False-gap protection through citation-network expansion and terminology-aware literature recovery.
- Screening modes for exploratory research, research landscapes, trends, emerging topics, State of the Art, gap validation, novelty validation, continuation research, systematic review, meta-analysis, methodology, and manuscript support.
- Transparent title, abstract, and full-text screening logic.
- Explicit screening exclusion reasons and duplicate-study controls.
- Shared-dataset awareness to prevent false independent replication.
- Contradictory and negative-result protection during literature screening.
- Evidence synthesis across convergent, contradictory, heterogeneous, mechanistic, contextual, methodological, and temporal patterns.
- Evidence-maturity assessment.
- Evidence-strength assessment.
- Consensus classification.
- Explicit distinction between evidence absence and evidence of no effect.
- Evidence maps linking synthesis claims to supporting and contradictory studies.
- Handoff from narrative synthesis to meta-analysis when quantitative pooling is scientifically appropriate.

### Completed Architecture

The Evidence & Reference Integrity Layer now follows:

`scopus-literature-search`
→ `source-verification`
→ `reference-integrity-guard`
→ `citation-chaining`
→ `literature-screening`
→ `evidence-synthesis`

### Functional Responsibilities

`scopus-literature-search`
- DISCOVER relevant scholarly literature.

`source-verification`
- VERIFY publication identity, metadata, DOI, scholarly status, Scopus status, correction, and retraction information.

`reference-integrity-guard`
- GUARD the relationship between scientific claims, citations, verified sources, and reference-list entries.

`citation-chaining`
- EXPAND the corpus through scientific relationships around verified anchor papers.

`literature-screening`
- SELECT scientifically relevant and eligible evidence.

`evidence-synthesis`
- SYNTHESIZE the included evidence into defensible cross-study scientific conclusions.

### Scientific Integrity

The completed Evidence & Reference Integrity Layer enforces:

- no fabricated references;
- no guessed DOI values;
- no metadata mashups;
- no unsupported Scopus claims;
- no citation padding;
- no target-journal citation manipulation;
- no exclusion of contradictory evidence merely because it conflicts with a preferred interpretation;
- no treatment of publication counts as evidence quality;
- no treatment of journal quartile as study quality;
- no APC-based evidence filtering;
- no confusion between discovered and verified literature;
- no confusion between eligible literature and strong evidence;
- no confusion between evidence absence and evidence of no effect;
- no synthesis from unverified or inadequately screened evidence.

### Evidence Pipeline

The framework now supports the complete evidence flow:

Research Question / Research Direction
→ Scholarly Discovery
→ Source Verification
→ Reference Integrity
→ Citation Expansion
→ Literature Screening
→ Evidence Synthesis

The resulting evidence architecture is ready to support:

- State-of-the-Art development;
- research-gap discovery;
- research-gap validation;
- novelty construction;
- novelty auditing;
- theoretical positioning;
- methodological design;
- scientific discussion;
- manuscript preparation.

## [0.4.0-alpha.1] - Evidence & Reference Integrity Foundation

### Added

- `scopus-literature-search` skill as the primary scholarly literature discovery layer.
- `source-verification` skill for validating scholarly publication identity, metadata, DOI integrity, peer-review status, journal legitimacy, Scopus status, corrections, and retractions.
- `reference-integrity-guard` skill for auditing the complete relationship between scientific claims, in-text citations, verified sources, and reference-list entries.
- Scopus-first literature discovery with fallback support for OpenAlex, Crossref, PubMed, Semantic Scholar, publisher platforms, and discipline-specific scholarly sources.
- Explicit separation between Scopus source-level status and document-level Scopus verification.
- Historical Scopus coverage awareness to prevent incorrect indexing claims for articles published outside a journal's Scopus coverage period.
- Search-query decomposition using concept blocks, synonyms, historical terminology, disciplinary terminology, and terminology drift.
- Dedicated search modes for exploratory research, research landscapes, State of the Art, gap validation, novelty validation, continuation studies, methodology, target-journal context, systematic review, meta-analysis, and manuscript support.
- Mandatory contradictory-evidence and competing-theory search principles to reduce confirmation bias.
- DOI normalization, bibliographic normalization, duplicate detection, and provenance preservation.
- Source-verification tiers covering publication identity, scholarly status, indexing status, and integrity checks.
- Retraction, correction, preprint, conference-paper, and duplicate-publication handling.
- Reference-mashup and citation-hallucination detection.
- Claim-to-source support auditing.
- Claim-strength auditing to prevent causal or universal claims that exceed the underlying evidence.
- In-text citation and reference-list consistency checks.
- Target-journal citation integrity safeguards.
- Citation-padding detection.
- Explicit prohibition of fabricated references, guessed DOI values, unsupported Scopus claims, and "vibe citation."

### Architecture

Evidence and Reference Integrity architecture — foundation:

`scopus-literature-search`
→ `source-verification`
→ `reference-integrity-guard`

Responsibilities are intentionally separated:

- `scopus-literature-search` discovers potentially relevant scholarly records.
- `source-verification` determines whether individual sources are real, traceable, bibliographically consistent, legitimate, and appropriately verified.
- `reference-integrity-guard` determines whether verified sources are used accurately and appropriately to support scientific claims.

### Scientific Integrity

The Evidence Layer establishes the following non-negotiable principles:

- discovered does not mean verified;
- Scopus source status does not automatically prove Scopus document status;
- DOI-like syntax does not prove DOI validity;
- a real source can still be cited incorrectly;
- a relevant title does not prove claim support;
- target-journal citations must remain scientifically relevant;
- APC status must not influence scientific evidence selection;
- journal prestige does not substitute for evidence quality;
- unverified references must not silently enter evidence-dependent scientific claims;
- retracted literature must not support scientific conclusions;
- references must never be assembled from mixed metadata belonging to different publications.

### Status

This is the first development checkpoint of the Evidence & Reference Integrity Layer.

Remaining components planned for v0.4.0:

- `citation-chaining`
- `literature-screening`
- `evidence-synthesis`

## [0.3.0] - Research Discovery Layer

### Added

- `idea-discovery` skill for transforming broad interests, real-world problems, scientific observations, available resources, and strategic priorities into focused candidate research directions.
- `research-landscape` skill for mapping the structure of a research field across themes, concepts, theories, methods, populations, contexts, evidence streams, and scientific maturity.
- `trend-detection` skill for distinguishing meaningful scientific change from simple publication-volume growth.
- `emerging-topic-discovery` skill for identifying genuinely emerging scientific topics, concepts, methods, technologies, interdisciplinary combinations, and early research frontiers.
- Explicit distinction between research ideas, trends, emerging topics, research gaps, and novelty.
- Research maturity mapping from discovery through validation, prediction, intervention, implementation, and translation.
- Preliminary research-direction comparison based on scientific importance, researchability, feasibility, program potential, and evidence needs.
- Multi-signal trend evaluation covering topic growth, methodological shifts, theory changes, population shifts, evidence maturity, technology adoption, interdisciplinary development, saturation, and durability.
- Emerging-topic assessment covering emergence strength, evidence maturity, saturation, durability, hype risk, terminology stability, and long-term research-program potential.
- Strong anti-trend-chasing rules to prevent fashionable technologies, publication growth, geographic absence, or advanced methods from being treated automatically as novelty.
- Explicit requirement that candidate directions and emerging topics proceed to Scopus-first evidence assessment before research-gap or novelty claims are finalized.

### Architecture

New-research discovery architecture:

`research-router`
→ `research-intake`
→ `idea-discovery`
→ `research-landscape`
→ `trend-detection`
→ `emerging-topic-discovery`
→ Scopus-first evidence investigation

The Research Discovery Layer produces candidate scientific directions and emerging-topic signals.

It does not independently declare:

- confirmed research gaps;
- final novelty;
- guaranteed publication potential;
- confirmed journal suitability.

Those decisions require downstream evidence verification and scientific synthesis.

### Scientific Integrity

The discovery layer reinforces these principles:

- trend does not equal research gap;
- emerging topic does not equal novelty;
- publication volume does not equal scientific importance;
- sparse literature does not automatically indicate opportunity;
- new location does not automatically indicate novelty;
- advanced methodology does not automatically indicate scientific contribution;
- fashionable technology does not replace a research problem.

## [0.2.0] - Research Continuation Layer

### Added

* `research-trajectory-mapper` skill for reconstructing the evolution of multiple previous studies across time.
* `continuation-opportunity-finder` skill for generating and prioritizing scientifically defensible next-study opportunities.
* Research trajectory assessment covering themes, research-question evolution, theory, methods, analysis, population, evidence accumulation, and research maturity.
* Research niche and signature research-program detection.
* Research stagnation and trajectory-fragmentation detection.
* Continuation pathway taxonomy covering replication, validation, mechanism, mediation, moderation, longitudinal research, experimentation, methodological advancement, prediction, intervention, implementation, translation, contextual extension, and integrative research.
* Candidate continuation comparison based on scientific importance, validated gap strength, novelty potential, methodological progression, feasibility, research-program coherence, and roadmap value.
* Explicit distinction between historical research opportunities and currently validated continuation opportunities.
* Risk–reward and trade-off assessment for alternative next studies.
* Research capability and collaboration-awareness for continuation planning.

### Changed

* Revised `research-resume` to focus specifically on research-state recovery and continuity rather than duplicating detailed scientific auditing.
* Clarified the division of responsibility between:

  * `research-resume`
  * `prior-research-auditor`
  * `research-trajectory-mapper`
  * `continuation-opportunity-finder`

### Architecture

Research continuation architecture:

`research-router`
→ `research-resume`
→ `prior-research-auditor`
→ `research-trajectory-mapper` when multiple studies exist
→ current literature revalidation
→ `continuation-opportunity-finder`

The continuation layer does not declare final research gaps or novelty before current evidence has been verified.


## [0.1.0] - Initial Architecture

### Added

- Initial plugin repository structure.
- Plugin manifest under `.codex-plugin/plugin.json`.
- `research-router` skill.
- `research-intake` skill.
- `research-resume` skill.
- `prior-research-auditor` skill.
- Scopus-first research principle.
- Evidence-driven gap and novelty policy.
- No-mandatory-APC publication preference.
- Target-journal citation integrity principle.
- Research continuity and previous-study continuation workflow.

### Architecture

Initial research entry architecture:

`research-router`
→ `research-intake` or `research-resume`
→ `prior-research-auditor`

This release establishes the foundation for future research discovery, evidence synthesis, research trajectory mapping, methodology, analysis, manuscript development, and publication-support skills.