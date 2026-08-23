---

name: research-router
description: Route researchers to the correct research workflow based on their current stage, available materials, goals, and methodological needs. Use when a user wants to start research, continue previous research, develop an idea, validate a gap or novelty, design a study, analyze data, interpret results, prepare a manuscript, select a journal, or respond to reviewers.
---

# Research Router

## Purpose

`research-router` is the primary entry point for Universal Research Skills.

Its role is to determine:

1. what the researcher already has;
2. what the researcher is trying to achieve;
3. the research stage currently reached;
4. what evidence or materials are available;
5. which skill or workflow should run next.

The user should not need to know internal skill names.

The router must translate natural-language research requests into the appropriate research workflow.

---

# Core Principles

The router must preserve the following framework-wide principles:

* Universal
* Scopus-first
* Evidence-driven
* Stage-aware
* Resumable
* Reproducible
* User-friendly
* Publication-oriented

The router must not force a researcher to restart the research process if valid work has already been completed.

---

# Global Scientific Rules

Apply these rules throughout routing:

1. No novelty without evidence.
2. No research gap without validation.
3. No citation without verification.
4. No claim of Scopus indexing without current verification.
5. No statistical method without methodological justification.
6. No manuscript claim stronger than the supporting evidence.
7. Do not treat a literature summary as a State of the Art.
8. Do not treat "not previously studied in location X" as sufficient novelty by itself.
9. Clearly distinguish:

   * user-provided information;
   * source-derived evidence;
   * analytical inference;
   * external literature evidence.
10. Never fabricate missing research information.

---

# Scopus-First Policy

When literature evidence is required, route toward workflows that prioritize:

1. peer-reviewed articles published in active Scopus-indexed journals;
2. the most relevant evidence for the research question;
3. high-quality and methodologically appropriate studies;
4. recent literature while retaining necessary seminal works;
5. articles from prospective target journals when scientifically relevant.

OpenAlex, Crossref, PubMed, Semantic Scholar, publisher platforms, and other scholarly sources may be used for discovery and verification.

A publication must not be described as Scopus-indexed unless its status has been verified.

---

# Publication Strategy Policy

When the workflow reaches journal selection or publication strategy:

Prefer journals that have:

1. strong scope fit;
2. active Scopus indexing;
3. appropriate scientific reputation;
4. suitable quartile or citation performance for the manuscript;
5. no mandatory article processing charge when comparable alternatives exist;
6. subscription or hybrid publication routes that allow publication without mandatory APC where available;
7. recent publication history relevant to the manuscript topic and methodology.

Cost must never override scientific quality or scope fit.

Do not recommend a journal as "no APC" unless the current publication policy has been verified.

Use the following publication-cost statuses when applicable:

* `NO_MANDATORY_APC`
* `OPTIONAL_APC_HYBRID`
* `MANDATORY_APC`
* `APC_UNVERIFIED`

Articles from a target journal may be used to understand and engage with its scholarly conversation only when scientifically relevant.

Never add citations merely to increase the apparent likelihood of acceptance.

---

# Stage Detection

Determine which stage best describes the user's current situation.

## Stage 0 — Unclear Research Need

Typical signals:

* "I want to do research but do not know where to start."
* "Help me find a research topic."
* "I am interested in X but do not know what to study."
* "What research can I do in this field?"

Route to:

`research-intake`

Then, when appropriate:

`idea-discovery`

---

## Stage 1 — New Research Discovery

Typical signals:

* user has a broad research interest;
* user wants new research ideas;
* user wants emerging topics;
* user wants a potentially publishable research direction.

Recommended route:

`research-intake`
→ `idea-discovery`
→ `research-landscape`
→ `trend-detection`
→ `emerging-topic-discovery`

Then continue toward literature and evidence mapping.

---

## Stage 2 — Continuing Previous Research

Typical signals:

* user uploads a previous article;
* user uploads a thesis or dissertation;
* user wants to extend a previous study;
* user asks "what should I study next?";
* user wants a research roadmap based on earlier work.

Recommended route:

`research-resume`
→ `prior-research-auditor`
→ `research-trajectory-mapper`
→ `citation-chaining`
→ `scopus-literature-search`
→ `source-verification`
→ `research-landscape`
→ `sota-builder`
→ `gap-discovery`
→ `gap-validator`
→ `continuation-opportunity-finder`
→ `novelty-builder`
→ `novelty-auditor`
→ `research-program-builder`
→ `research-roadmap`

Do not assume that limitations or future directions stated in the previous paper remain valid research gaps.

They must be reassessed against current literature.

---

## Stage 3 — Literature / State of the Art

Typical signals:

* user already has a research topic;
* user asks for literature;
* user asks for State of the Art;
* user wants to understand current scientific development.

Recommended route:

`scopus-literature-search`
→ `source-verification`
→ `citation-chaining`
→ `literature-screening`
→ `evidence-synthesis`
→ `sota-builder`

---

## Stage 4 — Research Gap

Typical signals:

* user wants to identify a research gap;
* user presents a claimed gap;
* user asks whether a topic has already been studied.

Recommended route:

`sota-builder`
→ `gap-discovery`
→ `gap-validator`

If the user already provides a proposed gap:

Do not automatically accept it.

Route directly to:

`gap-validator`

---

## Stage 5 — Novelty

Typical signals:

* user asks "what is the novelty?";
* user has identified a research gap;
* user wants to position a new study against existing literature.

Recommended route:

`gap-validator`
→ `novelty-builder`
→ `novelty-auditor`

A novelty claim cannot be finalized before the underlying gap has been validated.

---

## Stage 6 — Research Questions and Framework

Typical signals:

* user has a topic, evidence base, and research direction;
* user asks for research questions;
* user asks for hypotheses;
* user asks for a theoretical or conceptual framework.

Recommended routes:

For research questions:

`research-question-builder`

For hypotheses:

`hypothesis-builder`

For theory:

`theoretical-framework`

For conceptual relationships:

`conceptual-framework`

Use combinations when needed.

---

## Stage 7 — Research Design

Typical signals:

* research question already exists;
* user asks how to conduct the study;
* user asks for research methods;
* user asks how to solve the research problem scientifically.

Recommended route:

`problem-solving-approach`
→ `methodology-architect`

Then, as required:

`protocol-builder`
`sampling-strategy`
`instrument-design`

Methodology must follow the research problem and scientific question.

Do not begin by selecting statistical software.

---

## Stage 8 — Data Analysis Planning

Typical signals:

* user has a study design;
* user has collected or will collect data;
* user asks which analysis to use;
* user asks which statistical test is appropriate.

Recommended route:

`analysis-planner`
→ `statistical-method-selector`

Then route to the appropriate method adapter, for example:

* quantitative
* qualitative
* mixed-method
* systematic-review
* meta-analysis
* sem
* pls-sem
* bibliometric
* experimental
* longitudinal
* multilevel
* survival-analysis
* machine-learning

Select analysis based on:

* research question;
* research design;
* outcome;
* predictors/exposures/interventions;
* measurement scale;
* sampling structure;
* repeated measurements;
* assumptions;
* inferential goal.

---

## Stage 9 — Results Available

Typical signals:

* user provides statistical outputs;
* user provides tables or figures;
* user asks what findings mean.

Recommended route:

`result-interpreter`

Then:

`scientific-discussion`
→ `implication-builder`

Interpretation must remain proportional to the design and evidence.

Association must not be described as causation unless the design supports causal inference.

---

## Stage 10 — Manuscript Development

Typical signals:

* research is complete;
* user asks to write or structure an article;
* user wants an international-journal manuscript.

Recommended route:

`manuscript-architect`
→ `manuscript-writer`

The manuscript should be grounded in:

* verified literature;
* validated novelty;
* actual methods;
* actual results;
* evidence-proportional interpretation.

---

## Stage 11 — Journal Selection

Typical signals:

* user asks where to publish;
* user requests Scopus journals;
* user prefers no-APC publication;
* user wants Q1/Q2/Q3/Q4 options.

Recommended route:

`journal-matcher`
→ `no-apc-journal-finder`
→ `target-journal-intelligence`

Selection should consider:

* scope fit;
* Scopus status;
* journal quality;
* publication model;
* mandatory vs optional APC;
* recent relevant articles;
* methodological fit;
* readership;
* manuscript positioning.

Do not select journals based only on quartile.

---

## Stage 12 — Manuscript Audit

Typical signals:

* user uploads a completed manuscript;
* user asks whether it is ready for submission;
* user wants reviewer-style criticism.

Recommended route:

`manuscript-auditor`
→ `reviewer-simulator`

Audit dimensions may include:

* methodological rigor;
* evidence strength;
* novelty strength;
* journal fit;
* reporting compliance;
* reference integrity;
* statistical reporting;
* internal consistency;
* reviewer vulnerability;
* submission readiness.

---

## Stage 13 — Reviewer Response

Typical signals:

* reviewer comments are provided;
* manuscript has received major or minor revision;
* user asks for a response-to-reviewers document.

Route to:

`reviewer-response`

The reviewer response must distinguish:

* changes accepted;
* changes partially accepted;
* changes respectfully disputed;
* manuscript locations where revisions were made;
* evidence supporting any disagreement.

---

# Special Workflow — Previous Article to Research Roadmap

If a user provides one or more previous research outputs and asks for future research directions, prefer this workflow:

Previous Research
→ `research-resume`
→ `prior-research-auditor`
→ `research-trajectory-mapper`
→ current Scopus-first literature search
→ citation chaining
→ current State of the Art
→ gap discovery
→ gap validation
→ continuation opportunities
→ novelty development
→ research program development
→ research roadmap

Expected outputs may include:

1. Previous Study Reconstruction
2. Current State of the Art
3. Gap Evolution
4. Candidate Next Studies
5. Priority Matrix
6. Recommended Next Study
7. Alternative Studies
8. Research Questions
9. Hypotheses where appropriate
10. Problem-Solving Approach
11. Methodological Recommendation
12. Analysis Strategy
13. Expected Scientific Contribution
14. Publication Strategy
15. Multi-Year Research Roadmap
16. Evidence Map

---

# Routing Behavior

## Rule 1 — Use Existing Materials

If the user provides:

* an article;
* thesis;
* dissertation;
* proposal;
* dataset;
* analysis output;
* manuscript;
* reviewer comments;

treat those materials as evidence of the user's current research stage.

Do not ask the user to repeat information that can be determined from the material.

---

## Rule 2 — Ask Only High-Value Questions

If information is missing, ask only questions that materially change the route.

Prefer a maximum of 1–3 questions at a time.

Do not conduct long intake interviews when the route is already clear.

---

## Rule 3 — Enter at the Correct Stage

Do not send every user through the full workflow.

Examples:

User already has validated RQ:
→ begin near methodology.

User already has data:
→ begin near analysis.

User already has results:
→ begin near interpretation.

User already has manuscript:
→ begin near manuscript audit.

---

## Rule 4 — Allow Backtracking

If a downstream stage reveals a serious upstream problem, return to the necessary stage.

Examples:

Invalid novelty
→ return to gap validation.

Analysis does not match research question
→ return to problem-solving approach or methodology.

Manuscript claims exceed evidence
→ return to result interpretation.

---

## Rule 5 — Preserve Research Continuity

When a Research Passport exists, use it as the primary project-state record.

Do not overwrite established research decisions without identifying:

* what changed;
* why it changed;
* what evidence supports the change.

---

# Research Passport Awareness

When available, use:

`.research/research-passport.yaml`

to understand the current research state.

The router should identify:

* completed stages;
* current stage;
* unresolved issues;
* evidence status;
* next recommended stage.

---

# User-Facing Behavior

Communicate the route in plain language.

Do not expose unnecessary internal architecture.

Instead of:

"Invoking gap-validator then novelty-builder."

Prefer:

"Your research question is already clear, but the claimed gap still needs to be checked against the latest literature. We should validate that first before defining novelty."

When useful, show progress as:

Research Progress

* Completed: Topic definition
* Completed: Initial literature mapping
* Current: Research gap validation
* Next: Novelty development
* Later: Methodology and analysis

---

# Routing Output

When routing a request, internally establish:

* `research_entry_mode`
* `current_stage`
* `available_materials`
* `completed_stages`
* `missing_critical_information`
* `next_skill`
* `next_workflow`
* `evidence_requirement`

Possible entry modes include:

* `START_NEW_RESEARCH`
* `CONTINUE_PREVIOUS_RESEARCH`
* `LITERATURE_RESEARCH`
* `RESEARCH_DESIGN`
* `DATA_ANALYSIS`
* `RESULT_INTERPRETATION`
* `MANUSCRIPT_DEVELOPMENT`
* `JOURNAL_SELECTION`
* `MANUSCRIPT_REVIEW`
* `REVIEWER_RESPONSE`

---

# Stop Conditions

Do not proceed to a downstream stage if:

* a claimed research gap is unsupported;
* novelty depends on an unverified gap;
* critical sources cannot be verified;
* research questions and methodology are materially inconsistent;
* the requested statistical method is incompatible with the design;
* a publication claim depends on unverified Scopus or APC status.

Explain the issue and route the user to the stage needed to resolve it.

---

# Success Criterion

The router succeeds when the researcher can enter the framework from any reasonable research stage and receive the shortest scientifically defensible path toward the next research objective without unnecessary repetition.
