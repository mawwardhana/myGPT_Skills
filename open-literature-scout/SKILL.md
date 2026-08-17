---
name: open-literature-scout
description: >
  Search, screen, verify, and summarize scientific literature using
  publicly accessible scholarly sources. Use this skill when the user
  asks to find scientific papers, primary studies, systematic reviews,
  DOI information, or evidence supporting a research question.
---

# Open Literature Scout
Version: 0.2

## Purpose

Help identify relevant and credible scientific literature using
a transparent and reproducible workflow.

## When to use

Use this skill when the user asks to:

- find scientific papers;
- identify primary research articles;
- find supporting literature for a research topic;
- verify DOI or bibliographic information;
- distinguish primary and secondary literature;
- identify recent evidence;
- find open-access scientific sources.

Do not use this skill for:

- general news;
- casual web searches;
- non-academic information requests.

## Required inputs

Identify when available:

1. Research topic or question
2. Population or object of study
3. Main variables or concepts
4. Publication year range
5. Preferred study design
6. Language restriction
7. Open-access requirement

If information is incomplete, derive reasonable search concepts
from the research question.

## Workflow

### Step 1 — Understand the research question

Identify:

- population;
- intervention or exposure;
- outcome;
- context;
- key concepts;
- synonyms.

### Step 2 — Generate search terms

Create:

- main keywords;
- synonyms;
- scientific terminology;
- Boolean combinations when useful.

## Search transparency

Before presenting the selected literature, report:

1. Core search concepts
2. Main keywords and synonyms
3. At least one Boolean search string
4. Scholarly sources actually used

Do not silently perform the literature search without reporting
the search strategy.

The search strategy should be concise but sufficiently transparent
for the user to understand how the literature was identified.

### Step 3 — Search scholarly sources

Prefer:

1. Publisher or journal website
2. PubMed
3. Crossref
4. OpenAlex
5. DOAJ
6. Institutional repositories
7. Other credible scholarly databases

Avoid relying on blogs or commercial aggregator pages when
the original scholarly source is available.

### Step 4 — Screen results

Assess:

- relevance;
- article type;
- population or sample;
- methods;
- variables;
- outcomes;
- publication year;
- journal;
- DOI;
- full-text availability.

### Step 5 — Classify evidence

Classify each article as:

- Primary research
- Systematic review
- Meta-analysis
- Narrative review
- Guideline
- Other

Never classify a review article as primary research.

## Primary-study enforcement

When the user explicitly requests primary research:

Include an article in the confirmed primary-research results only when
there is sufficient evidence that the authors generated or analyzed
original empirical data.

Primary research may include:

- experimental laboratory studies;
- clinical studies;
- observational studies;
- in vivo studies;
- in vitro studies;
- original quantitative or qualitative studies.

Do not include as confirmed primary research:

- narrative reviews;
- systematic reviews;
- meta-analyses;
- editorials;
- perspectives;
- commentaries;
- protocols without results.

If article type cannot be verified, label it:

"Primary status not verified"

and do not mix it with confirmed primary studies.


### Step 6 — Verify bibliographic information

For every article recommended as a confirmed result, verify whenever possible:

- exact title;
- authors;
- publication year;
- journal;
- DOI;
- article type;
- relevance to the requested research topic.

### DOI verification rule

A DOI should be treated as verified only when the DOI can be matched
to the same article title through a reliable scholarly source.

Preferred verification sources:

1. Original publisher or journal
2. Crossref
3. PubMed
4. Other authoritative bibliographic database

Do not infer a DOI from citations found on unrelated webpages.

If the DOI cannot be independently matched to the article title,
report:

"DOI not verified."

### Link rule

When providing a DOI, prefer the canonical DOI format:

https://doi.org/[DOI]

Avoid tracking parameters such as:

utm_source
utm_campaign
utm_medium

when a clean canonical identifier is available.

### Step 7 — Mandatory output contract

For every literature-search task, use the structure defined in:

assets/output-template.md

The output template is mandatory.

Do not create an alternative response structure.

Do not skip, rename, merge, or reorder the following sections:

1. Research question
2. Search strategy
3. Screening criteria
4. Selected literature
5. Screening notes
6. Search quality

All required fields in the selected-literature table must be included.

If information for a required field cannot be verified, write:

"Not verified"

Do not omit the field.