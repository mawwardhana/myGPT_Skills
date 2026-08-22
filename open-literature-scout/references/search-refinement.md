# Search Refinement Rules

## Purpose

Use iterative search refinement when the initial search does not
retrieve an adequate pattern of relevant literature.

Search refinement should improve retrieval without changing the
meaning of the user's research question.

Do not refine a query merely to produce more results.

Refinement must be based on an observed retrieval problem.

## General workflow

For literature-search tasks:

1. construct the initial query;
2. run the initial search;
3. inspect the retrieved-result pattern;
4. diagnose whether refinement is needed;
5. modify the query only when there is a clear reason;
6. rerun the search when appropriate;
7. document what changed and why;
8. stop when further refinement is unlikely to materially improve the
   evidence retrieval.

Do not silently replace the initial query with a revised query.

Preserve the search history.

## Search diagnosis labels

Use only these primary diagnosis labels:

### ADEQUATE

Use when:

- the retrieved results substantially match the research question;
- relevant evidence is being retrieved;
- no obvious terminology or concept problem is present;
- further query modification is unlikely to materially improve the
  search.

ADEQUATE does not mean that every retrieved result is relevant.

---

### TOO_BROAD

Use when the search retrieves substantial irrelevant material because
the query does not sufficiently represent the user's research question.

Possible signals include:

- results dominated by unrelated populations;
- results dominated by unrelated disciplines or contexts;
- an ambiguous term retrieving a different meaning;
- one or more essential concepts are missing from the query.

Do not classify a search as TOO_BROAD merely because the database
returns a large number of records.

Relevance matters more than total result count.

---

### TOO_NARROW

Use when the query appears to exclude relevant evidence unnecessarily.

Possible signals include:

- very few directly relevant results despite a topic expected to have
  an established literature;
- known relevant terminology is missing;
- too many independent concept blocks are joined with AND;
- optional comparator, outcome, context, or design terms are being used
  as mandatory restrictions;
- exact phrases are unnecessarily restrictive.

Do not classify a search as TOO_NARROW solely because the number of
results is small.

A genuinely niche topic may appropriately retrieve few studies.

---

### TERMINOLOGY_GAP

Use when relevant literature appears to use terminology not represented
in the current query.

Examples include:

- spelling variants;
- abbreviations;
- historical terminology;
- scientific or common-name variants;
- alternative names for an intervention, exposure, population, or
  phenomenon;
- terminology identified from relevant seed articles.

When appropriate, add such terms using OR within the same concept.

---

### SOURCE_LIMITATION

Use when the main problem is not the Boolean query itself but the
limitations of the source being searched.

Examples include:

- source-specific indexing limitations;
- incomplete metadata;
- inability to search abstracts;
- unsupported Boolean syntax;
- limited result visibility;
- access restrictions that prevent adequate verification.

Do not repeatedly rewrite the scientific query when the problem is
primarily source-related.

Instead, use another appropriate scholarly source when available and
record the reason.

## Refinement actions

### Broadening a search

When a search is TOO_NARROW or has a TERMINOLOGY_GAP, consider:

- adding relevant synonyms using OR;
- adding spelling variants;
- adding abbreviations;
- adding broader or historical terminology;
- removing a nonessential AND concept block;
- removing an unnecessarily restrictive outcome;
- removing an optional comparator;
- removing an overly specific context term;
- replacing an exact phrase with appropriate alternatives.

Do not broaden by adding unrelated concepts.

---

### Narrowing a search

When a search is TOO_BROAD, consider:

- adding an essential missing concept with AND;
- replacing an ambiguous term with a more specific term;
- using a phrase when the phrase represents a stable scientific concept;
- adding a necessary population or context concept;
- removing irrelevant synonyms that introduce systematic noise.

Use NOT cautiously.

Do not use NOT merely because some irrelevant records appear.

A NOT term may unintentionally remove relevant evidence.

## Boolean refinement rule

Remember:

- OR within a concept usually broadens retrieval;
- additional independent AND concept blocks usually narrow retrieval.

Do not describe OR-based synonym expansion as making a search more
restrictive.

Do not add every framework element to the Boolean query automatically.

Continue to follow the Search translation rule in
`question-frameworks.md`.

## Query comparison rule

When a query is revised, compare the revised retrieval pattern with the
previous iteration.

Ask:

- Did direct relevance improve?
- Did obvious noise decrease?
- Were previously relevant concepts preserved?
- Did the revision introduce a new terminology gap?
- Did the revision become unnecessarily restrictive?

Do not claim that a revised query is better merely because it returns
more or fewer records.

## Result-count integrity rule

Do not invent or estimate database result counts.

Report a result count only when the source or search tool explicitly
provides that count.

When only a limited result set is visible, describe the observation as:

"retrieved-result pattern"

or:

"results inspected"

rather than implying that the visible records represent the complete
database result set.

## Search-source rule

Record only sources actually used in each search iteration.

If a query must be adapted because a source uses different search
syntax, distinguish:

- scientific concept refinement; and
- source-specific syntax adaptation.

Do not present source-specific syntax adaptation as a change in the
research question.

## Search stopping rule

For routine literature scouting, stop refinement when one of the
following applies:

### ADEQUATE_RETRIEVAL

The search retrieves a sufficiently relevant evidence pattern for the
user's request and no major terminology or concept problem remains.

### NO_MATERIAL_IMPROVEMENT

A further reasonable refinement does not materially improve relevance
or retrieval quality.

### SOURCE_LIMITATION_REACHED

Further improvement is constrained primarily by the available source
rather than by the query.

### USER_SCOPE_REACHED

The requested scope has been satisfied.

Do not continue iterative searching indefinitely.

For routine scouting, prefer a small number of purposeful iterations
rather than repeated minor query changes.

Systematic or protocol-driven searches may require additional
iterations when the user's methodology requires them.

## Search-history integrity rule

For every search iteration, preserve:

- iteration number;
- query used;
- source actually searched;
- diagnosis;
- change from the previous query;
- reason for the change.

If the initial query is ADEQUATE and no refinement is needed, record
one iteration and state:

"No refinement required."

## Evidence integrity rule

Search refinement affects retrieval strategy only.

It does not determine:

- evidence status;
- study quality;
- primary-study status;
- DOI verification;
- inclusion or exclusion.

Those decisions must continue to follow `SKILL.md` and any relevant
domain-specific reference rules.

## Counter-evidence retrieval check

For claim-focused searches, iterative refinement must include a deliberate
attempt to retrieve evidence that may oppose, fail to support, or
materially limit the claim.

Retrieval adequacy must not be judged only from the successful discovery
of supporting studies.

### When this check is required

Perform the counter-evidence retrieval check when:

- `Synthesis mode` is `CLAIM_SUPPORT`; or
- the user asks whether evidence supports, contradicts, weakens, limits,
  or qualifies a specific claim.

The check must occur before the final search is classified as adequate
and before a stopping reason is applied.

### Minimum counter-evidence pass

Conduct at least one retrieval iteration whose purpose is specifically
to detect contrary, null, inconclusive, or claim-limiting evidence.

The pass should use one or more of the following strategies as
appropriate.

#### 1. Remove positive-effect terminology

Run a broader query that retains the intervention/material and target
population, organism, or phenomenon but does not require terms such as:

- antibacterial;
- effective;
- inhibition;
- improved;
- beneficial;
- positive response.

This reduces the risk that retrieval logic itself filters out studies
whose findings are null or contrary.

#### 2. Add negative or null-result terminology

Where useful, test terms such as:

- `"no inhibition"`
- `"no effect"`
- `"not effective"`
- ineffective
- resistant
- `"no antibacterial activity"`
- `"failed to inhibit"`
- `"lack of activity"`

These terms are retrieval aids, not evidence labels.

Do not assume that all contrary studies will use explicit negative-result
terminology.

#### 3. Check title-mismatch risk

A relevant study must not be excluded only because the title emphasizes:

- another organism;
- another population;
- another outcome;
- another comparator;
- another intervention arm;
- a broader or narrower experimental purpose.

The target evidence may appear only in the abstract, methods, results,
tables, figures, supplementary material, or a separately reported study
arm.

When a candidate record is otherwise relevant, screen beyond the title
when accessible evidence permits.

For example, a paper whose title emphasizes Gram-negative bacteria may
still report direct experimental results for `Staphylococcus aureus`.

#### 4. Re-screen useful seed records

Relevant records discovered during earlier iterations may reveal:

- additional organisms;
- comparison arms;
- cited primary studies;
- terminology not represented in the initial query;
- null or contrary findings embedded in a broader study.

Use those observations for targeted refinement when they could
materially affect claim-level retrieval.

### Independent counter-evidence discovery

For claim-focused retrieval, the counter-evidence check must use at
least two complementary discovery strategies when title-mismatch risk is
plausible.

Minor variations of the original supporting query are not sufficient.

#### Strategy A — target-preserving, effect-neutral retrieval

Retain:

- the intervention, material, exposure, or phenomenon; and
- the target organism, population, or relevant outcome context.

Remove any requirement for a positive-effect term.

For example:

`chitosan AND "Staphylococcus aureus"`

may be used without requiring:

`antibacterial`

`effective`

`inhibition`

or equivalent positive-effect terminology.

This strategy reduces effect-direction retrieval bias while preserving
the target.

#### Strategy B — target-relaxed title-mismatch retrieval

Retain the intervention, material, exposure, or phenomenon, but remove
the target organism or population from at least one query.

Use broader domain or experimental terms as appropriate.

Examples may include:

`chitosan AND antimicrobial`

`chitosan AND bacteria`

`"native chitosan" AND microorganisms`

or another domain-appropriate broad query.

The purpose is not to treat all retrieved studies as relevant.

The purpose is to discover studies whose title or primary emphasis does
not foreground the target organism or population.

Candidates identified through this strategy must then be screened for
the target evidence in available:

- abstract;
- keywords;
- methods;
- results;
- tables;
- figures;
- supplementary material;
- full text.

For example, a paper whose title emphasizes Gram-negative bacteria may
still contain direct experimental evidence for `Staphylococcus aureus`.

#### Retrieval-channel diversity

When feasible, use more than one retrieval channel for counter-evidence
discovery.

Prefer a combination such as:

- bibliographic index or scholarly database; and
- publisher, journal, institutional repository, or scholarly full-text
  discovery.

Do not describe repeated searches through the same retrieval channel as
independent discovery merely because query terms changed.

If only one meaningful retrieval channel is available, state the source
limitation explicitly.

### Counter-evidence candidate ledger

Maintain a temporary candidate ledger across search iterations for any
record that may contain:

- contrary evidence;
- null findings;
- inconclusive findings;
- claim-limiting evidence;
- title-mismatch evidence.

A candidate entered into this ledger must not disappear merely because a
later search iteration returns a different evidence set.

Each candidate must eventually be resolved as one of:

- retained for normal evidence screening;
- `EXCLUDED` with a documented reason;
- `UNVERIFIED` when verification cannot be completed;
- duplicate or overlapping record;
- outside the claim scope after screening.

Do not silently discard a plausible counter-evidence candidate.

The ledger is a retrieval-integrity device, not an additional evidence
state.

### Candidate-resolution handoff

Candidate-ledger resolution must remain traceable into the downstream
evidence set.

When a candidate is marked:

`retained as evidence`

the same scholarly study must appear in selected literature or another
explicit downstream evidence record.

If a candidate is retained as:

- contrary evidence;
- claim-limiting evidence;
- inconclusive evidence; or
- another synthesis-relevant evidence unit,

it must not disappear after the retrieval stage.

A candidate may be omitted from the downstream selected evidence set
only when its resolution is explicitly recorded as:

- `EXCLUDED` with reason;
- `UNVERIFIED`;
- duplicate or overlapping record;
- outside claim scope after screening.

Do not silently change:

`retained as evidence`

into an omitted record.

If a candidate's screening decision changes after further verification,
update the candidate ledger and report the revised resolution.

The required traceability path is:

candidate ledger
→ screening resolution
→ selected literature
→ extraction when performed
→ synthesis when performed.

### Unique evidence-unit deduplication

Before finalizing selected literature, deduplicate scholarly records into
unique evidence units.

Multiple discovery, verification, or access records for the same article
must not be counted as separate evidence units.

Use available identifiers to identify duplicates, including:

- DOI;
- PMID;
- PMCID;
- exact article title;
- other stable scholarly identifiers.

Examples of records that normally represent one evidence unit include:

- publisher record + PubMed record;
- publisher record + repository full text;
- PubMed record + PMC full text;
- Crossref metadata + publisher record;
- multiple access routes to the same DOI.

Do not create an additional selected-literature row solely because the
same study was:

- verified through another scholarly source;
- found through another search strategy;
- accessed through another full-text location;
- re-screened during counter-evidence retrieval.

Instead, consolidate those verification and access details into the
single selected-literature record.

A study may be represented as more than one evidence unit only when the
source itself contains genuinely separable studies, datasets, cohorts,
experiments, or evidence units and the workflow explicitly documents why
they are being treated separately.

After deduplication, evidence counts must refer to unique evidence units,
not the number of discovery or verification records.

### Counter-evidence completion rule

A claim-focused search may be considered ready for final adequacy
assessment only when:

1. a target-preserving, effect-neutral pass has been completed;
2. a target-relaxed title-mismatch pass has been completed when
   applicable;
3. plausible counter-evidence candidates have been resolved or explicitly
   retained as unresolved;
4. the material effect of those passes on the evidence set has been
   reported.

Finding condition-dependent limitations alone does not prove that a
counter-evidence search was complete.

Likewise, technically testing negative terminology alone does not satisfy
this requirement if the discovery pathway remains effectively identical
to the supporting search.

### Interpretation of the check

Finding contrary evidence does not automatically mean the overall
evidence is `MIXED_EVIDENCE`.

The retrieved study must still proceed through:

screening
→ extraction
→ appraisal when applicable
→ comparability assessment
→ study-contribution classification
→ synthesis.

Likewise, failure to retrieve contrary evidence does not establish that
no contrary evidence exists.

Report only that no directly relevant contrary evidence was identified
in the counter-evidence retrieval performed.

### Relationship to search diagnosis

For a claim-focused search, do not assign final:

`ADEQUATE`

until the counter-evidence retrieval check has been completed.

If supporting evidence has been retrieved but the counter-evidence check
has not yet been performed, the search remains incomplete for
claim-support synthesis.

### Relationship to stopping rules

Do not apply:

- `ADEQUATE_RETRIEVAL`
- `NO_MATERIAL_IMPROVEMENT`
- `USER_SCOPE_REACHED`

as the final stopping reason for a claim-focused search before the
counter-evidence retrieval check.

`SOURCE_LIMITATION_REACHED` may still apply when source access prevents
a meaningful counter-evidence check, but the limitation must be stated
explicitly.

### Reporting requirement

In the search-iteration record, identify which iteration served as the
counter-evidence retrieval pass and report:

- query or search logic used;
- source actually searched;
- whether positive-effect terminology was removed;
- whether negative/null terminology was tested;
- whether title-mismatch candidates were screened;
- what material change, if any, resulted from the pass.

Do not invent retrieval counts when exact counts are unavailable.