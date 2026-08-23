# Changelog

All notable changes to Universal Research Skills will be documented in this file.

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