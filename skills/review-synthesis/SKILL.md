---
name: review-synthesis
description: "Synthesize multiple reviewer, supervisor, collaborator, or AI review reports into a deduplicated issue map that distinguishes consensus, disagreement, dependencies, and actionable revision work."
---

# review-synthesis

## Purpose

Extract the useful core of the repo's editorial synthesizer without making an editorial decision.

## Process

### 1. Parse every source separately
Preserve reviewer identity or source label and the exact concern before merging.

### 2. Normalize concerns
Separate multipart comments into distinct issues. Group only comments that share the same underlying problem.

### 3. Identify consensus
Record when multiple reviewers independently identify the same issue.

### 4. Preserve disagreement
Do not flatten conflicting advice into a compromise. State what each reviewer is optimizing for and whether the manuscript can satisfy both.

### 5. Identify dependencies
Some revisions must precede others. For example, changing the RQ may require methods, results framing, discussion, and abstract changes.

### 6. Distinguish revision types
- Clarification
- New analysis
- New evidence or literature
- Structural revision
- Scope reduction
- Methodological repair
- Wording or presentation
- Reviewer disagreement requiring reasoned response

## Output

### Review Synthesis
- Consensus issues
- Unique high-value issues
- Reviewer disagreements
- Duplicate comments merged with source traceability
- Dependency map
- Revision work packages
- Questions requiring author judgment

Do not invent new criticisms during synthesis. If a new issue is noticed, label it separately as a synthesizer observation rather than attributing it to reviewers.

## General guardrails

- Do not invent sources, citations, quotations, data, results, reviewer comments, or journal requirements.
- Distinguish what is supplied by the user, what is directly verified, what is inferred, and what remains unknown.
- Do not claim a search was exhaustive unless the search process justifies that claim.
- Do not treat source existence as proof that a source supports a particular claim.
- Do not silently strengthen association into causation, a local result into a universal claim, or exploratory evidence into confirmatory evidence.
- If required material is missing, identify the gap and continue with the parts that can be assessed.
- Prefer traceable reasoning. Important findings should point to the exact claim, section, source, table, figure, or reviewer comment that triggered them.
