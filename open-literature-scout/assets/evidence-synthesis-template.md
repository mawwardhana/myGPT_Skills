# Evidence Synthesis Template

Use this template only when evidence synthesis is active.

## Output integration rule

When this template is used with the mandatory output contract, do not
emit the file title as an additional report heading.

All synthesis content must remain inside:

`## 4. Selected literature`

The mandatory output template already renders:

`### Evidence synthesis`

Do not emit that heading a second time.

Begin the synthesis-template content beneath that existing subsection
with:

`#### Synthesis control`

Use `####` for headings nested beneath the synthesis subsection.


Do not create any additional top-level `##` section between:

`## 4. Selected literature`

and:

`## 5. Screening notes`

#### Synthesis control

| Field | Value |
|---|---|
| Synthesis mode | |
| Research question / claim | |
| Evidence units considered | |
| Eligible evidence states | |
| Comparability assessed | |
| Appraisal information used | |
| Study overlap checked | |
| Quantitative pooling performed | NO |

Allowed synthesis modes:

- NONE
- NARRATIVE_SYNTHESIS
- CLAIM_SUPPORT

Do not perform quantitative pooling in this narrative synthesis module.

#### Evidence set

| Evidence unit | Study design | Evidence status | Population/Object | Intervention/Exposure/Material | Outcome | Appraisal information | Role in synthesis |
|---|---|---|---|---|---|---|---|
| | | | | | | | |

Do not include an evidence unit without a clear record status.

#### Comparability assessment

Use only:

- DIRECTLY_COMPARABLE
- PARTIALLY_COMPARABLE
- NOT_DIRECTLY_COMPARABLE

| Evidence unit / comparison | Comparability | Basis |
|---|---|---|
| | | |

#### Comparability groups

Create groups only when materially useful.

A comparability group normally requires two or more evidence units.

| Group | Defining characteristics | Evidence units | Within-group comparability |
|---|---|---|---|
| | | | |

Use within-group comparability labels only when two or more evidence
units are actually being compared.

Do not assign DIRECTLY_COMPARABLE, PARTIALLY_COMPARABLE, or
NOT_DIRECTLY_COMPARABLE to a singleton evidence unit compared with
itself.

Do not numerically pool incompatible groups.

#### Unclustered / singleton evidence units

Use this subsection only when one or more eligible evidence units do not
fit a meaningful multi-study comparability group.

| Evidence unit | Reason kept separate | Potential role in later synthesis |
|---|---|---|
| | | |

Do not assign a within-group comparability label to a singleton evidence
unit.

Singleton status does not mean:

- irrelevant evidence;
- weak evidence;
- indirect evidence;
- excluded evidence.

Its contribution must be determined later according to the intended
synthesis question or claim.

#### Cross-study synthesis

Summarize:

- consistent findings;
- condition-dependent findings;
- important heterogeneity;
- genuinely conflicting findings;
- methodological considerations;
- important evidence gaps.

Do not use study counting alone to determine evidential strength.

#### Claim support map

Use this subsection only when:

**Synthesis mode: CLAIM_SUPPORT**

Use only these study-contribution labels:

- DIRECT_SUPPORT
- INDIRECT_SUPPORT
- DIRECT_INCONCLUSIVE_EVIDENCE
- CONTRARY_EVIDENCE
- NO_DIRECT_BEARING

Use `DIRECT_INCONCLUSIVE_EVIDENCE` when a study directly investigates
the claim-relevant outcome but the result is too limited, imprecise, or
inconclusive to materially support or oppose the claim.

Do not use it when the relevant outcome was not measured.

| Evidence unit | Evidence status | Comparability group / context | Study contribution | Key finding | Appraisal consideration | Relevance to claim |
|---|---|---|---|---|---|---|
| | | | | | | |


Comparability labels are relational.

Do not place DIRECTLY_COMPARABLE, PARTIALLY_COMPARABLE, or
NOT_DIRECTLY_COMPARABLE in an individual-study row unless the row
explicitly identifies the comparison relationship.

Use the study-level field to identify the relevant comparability group
or methodological context.

Report the controlled comparability judgment separately at the
pair/group level.

Study-contribution integrity check:

The selected study-contribution label must be supported by the
corresponding extracted finding.

Do not assign `DIRECT_SUPPORT` when the row only establishes that the
study:

- used the requested intervention or material;
- studied the requested organism or population; or
- measured a claim-relevant outcome.

`DIRECT_SUPPORT` requires a verified extracted finding that materially
supports the specific claim.

Before assigning `DIRECT_SUPPORT`, verify that the `Key finding` field
actually contains a claim-supporting result.

If the study is directly relevant but the direction of the finding is
not available or cannot be verified from the extraction basis, use:

`DIRECT_INCONCLUSIVE_EVIDENCE`

Do not infer a positive finding from study relevance, title, objective,
assay type, or evidence status.

Quantitative-summary integrity check:

Before placing a numerical result in the claim-support map, compare the
entry against the detailed extraction for that study.

If the detailed extraction contains multiple context-specific values for
the same nominal outcome, do not select one value as the study-wide
representative result unless the source explicitly identifies it as the
primary, corrected, replacement, or superseding value.

When all relevant values can be displayed without losing context,
preserve them together with their source-location or experimental-context
labels.

When the claim-support map needs a concise representation, use:

`Multiple context-specific values reported; see detailed extraction.`

rather than selecting one context-dependent value.

A study-contribution label may still be assigned from the verified
direction of the finding when appropriate, but the numerical summary
must not collapse materially different reported values.

The claim-support map must remain consistent with the complete
quantitative record in the detailed extraction.

#### Claim assessment

Use this subsection only when:

**Synthesis mode: CLAIM_SUPPORT**

Use only:

- SUPPORTED
- QUALIFIED_SUPPORT
- MIXED_EVIDENCE
- INSUFFICIENT_EVIDENCE
- NOT_SUPPORTED

**Claim assessment:**  

**Reason:**  

Do not translate the claim assessment into a formal certainty grade.

#### Study-overlap note

State whether evidence units appear independent.

If overlap cannot be verified, use:

`Study overlap: NOT_VERIFIED`

Do not double-count companion publications, shared cohorts, shared
datasets, or systematic reviews and their included studies.

#### Synthesis limitations

- 

Report only limitations materially supported by the evidence set.

#### Bottom-line synthesis

State:

1. what the evidence supports;
2. the scope and conditions of that support;
3. major qualifications;
4. what remains unestablished.

Do not provide:

- a universal quality score;
- a certainty grade unless a separate formal certainty framework was
  applied;
- a pooled effect;
- an informal meta-analysis;
- an unsupported generalization.