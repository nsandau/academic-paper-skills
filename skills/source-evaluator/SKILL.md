---
name: source-evaluator
description: "Evaluate whether an academic source is real, correctly identified, methodologically adequate, relevant, current enough, and suitable for supporting a specific claim, with explicit version, provenance, and read-scope tracking."
---

# source-evaluator

## Purpose

Answer a narrower question than fact checking: Is this source trustworthy enough and relevant enough for the intended use?

## Evaluation dimensions

### Identity and publication status
Verify, when tools permit:
- title
- authors
- year
- venue
- DOI or stable identifier
- source type and venue type
- version status such as preprint, accepted manuscript, or version of record
- corrections, expressions of concern, or retractions

### Cross-index triangulation
For conventional journal and conference literature, use multiple bibliographic indexes when practical, such as Crossref, OpenAlex, Semantic Scholar, PubMed, arXiv, or a first-party publisher page.

Treat resolver disagreement as a risk signal, not automatic proof of fabrication. Humanities sources, books, dissertations, local journals, reports, and non-English literature can have uneven index coverage.

Prefer first-party identifiers and publisher metadata when resolver records conflict.

### Version consistency
Do not accidentally combine metadata from different members of a version family. Check that title, authors, year, DOI, quoted text, and page or section locators belong to the same version being cited.

If evidence came from a preprint but the bibliography cites the version of record, verify that the relevant claim remains present in the cited version.

### Read scope
State how much of the source was actually inspected:
- `full_text`
- `sections`
- `abstract_only`
- `toc_only`
- `metadata_only`
- `unknown`

Never promote an abstract-only evaluation into a full-text claim-support judgment.

### Evidence type
Identify the actual study or document design. Avoid universal evidence hierarchies across disciplines. A randomized trial may be strong for an intervention effect but irrelevant for an interpretive or theoretical claim.

### Methodological adequacy
Inspect, when the source text permits:
- sample or corpus
- design
- measurement or coding
- analysis
- missing data
- confounding or bias
- transparency and reproducibility
- limitations acknowledged by the authors

### Relevance to intended claim
Distinguish:
- direct support
- indirect or contextual support
- mechanistic support
- background support
- no meaningful support

### Currency and version relevance
Ask whether age matters for the claim. Foundational theory and current prevalence estimates have different freshness requirements.

### Conflicts and provenance
When material, note funding, declared conflicts, unusual publication practices, or venue concerns. Do not label a journal predatory without evidence.

## Output

### Source Evaluation Card
- Bibliographic identity
- Identity verification sources
- Cross-index agreement or disagreement
- Version used
- Read scope
- Source type
- Research design
- Population or corpus
- Main finding relevant to the user's purpose
- Methodological strengths
- Methodological limitations
- Retraction or correction status
- Relevance to intended claim
- Suitable use in paper
- Claims this source should not be used to support
- Confidence and unresolved verification gaps

## General guardrails

- Do not invent source metadata or resolve ambiguous identities by guesswork.
- A failed resolver lookup is not sufficient evidence that a source is fake.
- Source existence does not establish claim support.
- Full-text methodological judgments require access to the relevant source text.
