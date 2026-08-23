# Changelog

All notable changes to Universal Research Skills will be documented in this file.

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