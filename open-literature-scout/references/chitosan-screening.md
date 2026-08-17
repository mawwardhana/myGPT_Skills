# Chitosan Screening Rules

## Chitosan intervention classification

For each article, classify the tested chitosan intervention as one of:

- Native chitosan
- Chitosan derivative
- Chitosan formulation/composite
- Chitooligosaccharide
- Mixed comparison
- Not clearly reported

### Native-chitosan rule

When the user asks generally about "chitosan" and does not explicitly
request derivatives:

Prioritize studies testing native or unmodified chitosan.

### Derivative rule

A study using only chemically modified or derivatized chitosan should
not automatically be treated as direct evidence for native chitosan.

If only a derivative is tested:

- classify it as "Chitosan derivative";
- keep it outside the core native-chitosan evidence set unless the
  user's question includes derivatives.

### Mixed-comparison rule

If a study tests native chitosan and a derivative in separate groups:

- the study may remain in the core evidence set;
- identify it as "Mixed comparison";
- report findings for native chitosan separately from the derivative.

### Formulation rule

If chitosan is incorporated into a film, gel, membrane, nanoparticle,
composite, or other formulation:

- classify the intervention as "Chitosan formulation/composite";
- determine whether antibacterial activity can reasonably be attributed
  to chitosan alone;
- if additional active antimicrobial substances are present, do not
  attribute the total antibacterial effect solely to chitosan.

## Output integration

When this reference file is active, add the following column to the
`Selected literature` table in `assets/output-template.md`:

`Chitosan type`

Place it immediately after:

`Evidence status`

Use only these labels:

- Native chitosan
- Chitosan derivative
- Chitosan formulation/composite
- Chitooligosaccharide
- Mixed comparison
- Not clearly reported

In the `Domain-specific summary` under `Search quality`, report when
applicable:

- Native-chitosan studies:
- Derivative-only studies:
- Formulation/composite studies:
- Chitooligosaccharide studies:
- Mixed-comparison studies:
- Not-clearly-reported studies: