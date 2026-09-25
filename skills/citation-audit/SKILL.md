---
name: citation-audit
description: "Audit in-text citations and reference lists for correspondence, metadata accuracy, identifier validity, cross-index agreement, version-family consistency, duplication, retractions or corrections, and citation-style consistency."
---

# citation-audit

## Purpose

Perform mechanical and bibliographic checks extracted from the upstream citation-compliance, citation-existence, triangulation, and integrity components.

## Audit layers

### 1. Correspondence
- Every in-text citation has a reference-list entry.
- Every reference-list entry is cited unless the venue permits uncited bibliography items.
- Author and year information correspond.
- Disambiguation suffixes and abbreviated author forms are internally consistent.

### 2. Metadata identity
Where tools permit, verify:
- title
- authors
- year
- journal or publisher
- volume, issue, pages, or article number
- DOI or other stable identifier
- publication type

Do not promote a DOI-looking string to `verified` unless it resolves or is confirmed by an authoritative source.

### 3. Cross-index verification
For references expected to be indexed, compare more than one source when practical. Record whether the reference is:
- verified by multiple independent metadata sources
- verified by one authoritative source
- conflicting across sources
- unresolved

Index mismatch is a warning signal. It is not automatically a fabricated-reference verdict.

### 4. Version-family consistency
Detect cases where the citation surface mixes a preprint, conference paper, accepted manuscript, and final journal version.

Check that:
- DOI belongs to the cited title/version
- year matches the cited version
- authorship matches that version
- quoted or paraphrased material was inspected in the version actually cited
- page or section locators exist in that version

Prefer the version of record when appropriate, while preserving a preprint citation when that is the version actually relied upon or when venue norms require it.

### 5. Retraction and correction status
Flag retracted items, expressions of concern, withdrawals, and relevant corrections. A correction does not automatically invalidate every use of a source.

### 6. Duplicates
Identify exact duplicates and version-family duplicates. Do not count a preprint and journal article as two independent studies when they report the same underlying work.

### 7. Citation style
Apply the requested style or target-venue rules. Keep style errors separate from verification errors. Do not assume Latin-alphabet ordering conventions apply to every language or venue.

## Important boundary

Citation audit confirms bibliographic correctness. It does not prove that a reference supports the surrounding claim. Use `claim-evidence-audit` for that.

## Output

### Citation Audit Summary
Counts of:
- missing references
- orphan references
- metadata mismatches
- unresolved identifiers
- cross-index conflicts
- version-family mismatches
- duplicates
- retraction or correction flags
- style errors

### Detailed Findings
For each issue include:
- manuscript or bibliography location
- current form
- issue class
- verification evidence
- verified or unresolved information
- recommended correction

### Verification Coverage
State how many references were checked, which indexes or first-party sources were used, and which references remain unresolved.

## General guardrails

- Do not invent sources or metadata.
- Do not claim a resolver was checked when it was not.
- Treat source existence, citation style, and claim support as separate questions.
