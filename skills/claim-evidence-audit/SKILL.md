---
name: claim-evidence-audit
description: "Audit whether manuscript claims are actually supported by the cited sources, reported data, and study design, with explicit source locators, read scope, negative constraints, scope limits, and uncited-claim checks."
---

# claim-evidence-audit

## Purpose

Evaluate claim faithfulness rather than only factual truth. This skill extracts the useful intellectual core of the upstream claim-reference alignment auditor and integrity gate.

## Audit units

For each important claim identify:
1. Exact claim text and manuscript location
2. Evidence pointer such as citation, table, figure, result, method, or dataset
3. Source locator where available, such as page, section, table, figure, or quoted support span
4. Read scope for each source
5. Strongest inference the evidence justifies
6. Strength and scope of manuscript wording
7. Any mismatch or constraint violation

## Prioritization

When a full manuscript is large, start with all high-impact claims:
- headline conclusions
- numerical claims
- causal claims
- methods-critical claims
- novelty or absence claims
- disputed claims

Then use a transparent sample of lower-impact claims if a complete audit is impractical. Report the denominator and sampling boundary.

## Mismatch classes

- citation does not support claim
- citation only supports part of a compound claim
- population mismatch
- geographic mismatch
- time-period mismatch
- outcome-definition mismatch
- correlation presented as causation
- exploratory analysis presented as confirmatory
- mechanism asserted without evidence
- generalization beyond sampled cases
- numerical mismatch
- uncited externally verifiable assertion
- constraint violation against stated design, data, or scope
- negative-constraint violation, where evidence explicitly rules out the manuscript wording
- absence or novelty claim stronger than the documented search can justify
- source exists but the relevant support cannot be located
- version mismatch between inspected source and cited source

## Evidence discipline

When the cited source text is not available, do not pretend to have checked claim faithfulness. Mark the item `evidence unavailable` or state the actual read scope.

When a sentence cites several references, determine whether support is collective or whether one source is being made to carry a claim it does not support.

A bibliographic match is not a semantic match. Locator evidence should be preferred for consequential claims.

## Output

### Claim-Evidence Audit
For each finding:
- location
- claim
- evidence pointer
- source version and read scope
- locator or support span when available
- support status
- mismatch class
- why current wording is unsafe or weak
- maximum defensible wording
- recommended fix

Use statuses:
- aligned
- partly aligned
- misaligned
- evidence unavailable
- uncited assertion

### Coverage Statement
State:
- claims audited
- high-impact claim denominator if known
- lower-impact sampling method if used
- source-text access limitations

End with the most consequential overclaims and the claims that require new evidence rather than mere rewriting.

## General guardrails

- Do not infer claim support from title, abstract, or citation existence when the relevant source text was not inspected.
- Do not silently weaken contradictory evidence by labeling it merely ambiguous.
- Keep evidence unavailable distinct from unsupported.
