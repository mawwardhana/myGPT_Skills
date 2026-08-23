# Changelog

All notable changes to Universal Research Skills will be documented in this file.

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