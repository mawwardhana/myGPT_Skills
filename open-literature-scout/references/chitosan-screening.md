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

### Derivative inclusion rule

"Outside the core native-chitosan evidence set" does not automatically
mean "EXCLUDED from the literature search."

When a derivative-only study is otherwise relevant primary research:

- classify it as "Chitosan derivative";
- keep it outside the core native-chitosan evidence set when the user
  asks generally about chitosan;
- retain it as relevant secondary evidence when appropriate;
- label its role clearly so it is not interpreted as direct evidence
  for native chitosan.

Use EXCLUDED only when:

- the user's question explicitly restricts eligibility to native or
  unmodified chitosan;
- the derivative study is irrelevant to the requested organism,
  outcome, or context;
- the study fails another explicit inclusion criterion.

Do not use EXCLUDED merely because the intervention is a chitosan
derivative.


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

### Formulation inclusion rule

A study must not be EXCLUDED solely because chitosan is presented as a
film, gel, membrane, nanoparticle, coating, composite, or other
formulation.

For a chitosan formulation/composite study:

1. classify the intervention as "Chitosan formulation/composite";
2. verify whether the study contains original empirical antibacterial
   data relevant to the user's question;
3. identify any additional antimicrobial active agents;
4. assess whether the antibacterial effect can reasonably be evaluated
   as an effect of chitosan within the formulation.

If no additional antimicrobial active agent creates a major attribution
problem, the study may remain eligible as CONFIRMED evidence.

Such a study should be distinguished from native-chitosan evidence, but
it should not be automatically moved to EXCLUDED.

When the study includes chitosan-only controls, chitosan solution,
chitosan-only film, or appropriate carrier controls, use those
comparisons to assess attribution.

Use EXCLUDED only when:

- the formulation does not provide empirical data relevant to the
  research question;
- another antimicrobial active agent prevents meaningful attribution
  to chitosan;
- chitosan is only an inactive carrier or incidental component; or
- another explicit exclusion criterion is met.

"Outside the core native-chitosan evidence set" does not automatically
mean "EXCLUDED from the literature search."


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