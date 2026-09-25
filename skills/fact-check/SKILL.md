---
name: fact-check
description: "Verify academic claims, numbers, references, temporal assertions, or manuscript statements against appropriate evidence and classify each as supported, partially supported, unsupported, contradicted, or unverifiable."
---

# fact-check

## Purpose

Perform claim-by-claim verification. Merge the upstream fact-check mode, source verification, integrity verification, temporal checks, and claim verification ideas without pipeline state or hard gates.

## Modes

- `claims`: factual and scholarly claims
- `numbers`: dates, sample sizes, effect sizes, rates, totals, and other quantitative statements
- `references`: existence and metadata checks
- `temporal`: chronology, date arithmetic, current/latest wording, and causal ordering
- `manuscript`: extract and verify high-impact claims throughout a document

## Process

### 1. Extract atomic claims
Split compound sentences into independently verifiable assertions. Preserve exact wording and location.

### 2. Classify claim type
Examples:
- descriptive fact
- quantitative claim
- causal claim
- historical or temporal claim
- literature-state claim
- novelty or absence claim
- methodological claim
- policy or guideline claim

### 3. Identify the evidence burden
A routine descriptive claim may need one authoritative source. A contested or high-impact claim should use multiple independent sources when feasible. A novelty or absence claim requires documented searching and careful wording.

### 4. Verify source identity separately
Check whether cited sources exist and whether metadata match. For consequential sources, record version and read scope. A real citation can still fail to support the claim.

### 5. Verify claim support
Compare the exact scope of the claim with the evidence:
- population
- geography
- time period
- outcome definition
- direction and magnitude
- association versus causation
- primary versus secondary analysis
- source version

### 6. Check temporal integrity when relevant
For claims using wording such as current, latest, recently, enabled, caused, superseded, or followed:
- identify dates or date ranges for the relevant entities
- confirm a cited source existed at the time it is being used to evidence, unless the sentence clearly describes later retrospective evidence
- verify causal or enabling events precede the outcomes attributed to them
- materialize the comparator when saying something is latest or newer
- replace deictic wording with an anchored date or version when precision matters

### 7. Assign a verdict
- `SUPPORTED`: evidence directly supports the claim at the stated strength and scope
- `PARTIALLY_SUPPORTED`: core idea is supported but wording, scope, magnitude, or certainty exceeds evidence
- `UNSUPPORTED`: available cited or verified evidence does not support the claim
- `CONTRADICTED`: stronger or directly relevant evidence conflicts with the claim
- `UNVERIFIABLE`: verification cannot be completed with available material

Do not force uncertainty into a false binary.

## Output

### Fact Check Table
For every checked claim include:
- location
- exact claim
- claim type
- evidence checked
- source version and read scope when relevant
- verdict
- scope, inference, or temporal mismatch
- corrected wording if needed
- better or additional evidence if identified
- verification limitations

### Summary
Report counts by verdict and highlight the highest-consequence errors first.

## General guardrails

- Do not invent sources, citations, quotations, data, results, or journal requirements.
- Distinguish user material, verified information, inference, and unknowns.
- Do not call a search exhaustive without evidence.
- Keep `unverifiable` distinct from `unsupported`.
