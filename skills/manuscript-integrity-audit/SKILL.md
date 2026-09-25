---
name: manuscript-integrity-audit
description: "Perform a whole-manuscript consistency, chronology, originality, provenance, and support audit across references, claims, data, tables, figures, methods, results, abstract, discussion, conclusion, novelty statements, and revision-sensitive surfaces."
---

# manuscript-integrity-audit

## Purpose

Salvage the useful verification logic from the upstream integrity gate while removing passports, schemas, hooks, certification language, and blocking machinery.

This is a final manuscript audit, not a substitute for expert methodological review.

## Modes

- `full`: run all applicable domains
- `numbers`: numerical and table/figure consistency
- `cross-section`: wording, sample, hypothesis, and result consistency across sections
- `temporal`: chronology, version, and date-integrity audit
- `originality`: attribution and suspicious textual-overlap audit

## Audit domains

### References and claims
- citation existence and metadata
- claim-reference alignment for high-impact claims
- uncited externally verifiable assertions
- source version consistency
- retraction or correction issues
- read-scope limitations for evidence relied on heavily

### Numbers and data surfaces
Cross-check:
- sample size
- group sizes
- dates
- percentages and totals
- effect sizes
- confidence intervals
- p-values where reported
- table values
- figure values
- supplementary values

Recalculate simple arithmetic where possible. Flag impossible denominators or totals.

### Cross-section consistency
Compare:
- RQ in abstract, introduction, methods, and conclusion
- hypotheses across introduction, methods, and results
- sample description across abstract, methods, results, and tables
- results described in abstract, Results, Discussion, and Conclusion
- limitation statements against the actual design
- terminology and construct names throughout

### Inference integrity
Flag:
- causal language unsupported by design
- novelty claims stronger than documented search
- results omitted from discussion because they complicate the story
- conclusions not established in Results
- methods or analyses mentioned only after results appear
- revision-induced claim strengthening not authorized by the evidence

### Temporal integrity
Check five recurring failure classes:
1. date arithmetic that yields impossible or misleading retrospective timing
2. anachronistic use of a source as if it existed before the event it is claimed to evidence
3. comparisons such as latest, newer, or superseded where the comparator version is not identified
4. causal or enabling claims where cause occurs after effect
5. unanchored present-tense terms such as current, latest, recently, or last year

Build a small timeline for consequential temporal claims. When date provenance is weak or conflicting, mark the claim unresolved rather than guessing.

### Originality and attribution
This is not an AI-authorship detector.

When source-search tools are available, sample distinctive passages, especially in literature review, background, discussion, and newly revised text. Look for:
- long unattributed verbatim overlap
- close paraphrase without attribution
- reused material from the author's earlier publications without appropriate citation or disclosure
- quotations missing quotation treatment
- standard methods language that may legitimately recur but should be handled transparently

Textual overlap is evidence to inspect, not automatic proof of misconduct. Preserve legitimate common phrasing, technical expressions, and standardized procedures.

### Figures and tables
Check labels, units, captions, denominators, source notes, and whether visual claims match underlying values.

## Output

### Integrity Audit Summary
List the most consequential issues first.

### Findings Table
For each issue:
- domain
- location A
- location B or evidence source
- inconsistency or support problem
- consequence
- recommended correction
- verification status

### Temporal Findings
For each issue include the relevant dates, date provenance, and the corrected temporal wording or ordering.

### Originality Findings
For each overlap concern include the manuscript passage, matched source if found, nature of overlap, attribution status, and recommended action. Do not label misconduct unless the evidence supports that conclusion.

### Unchecked Areas
State what could not be verified because source text, raw data, supplements, full bibliographic access, or search tools were unavailable.

## General guardrails

- Do not certify a manuscript as error-free.
- Do not call absence of a detected overlap proof of originality.
- Do not infer chronology from linguistic plausibility when dates can be checked.
