---
name: methodology-review
description: "Review a methods section or full paper for research-question alignment, design validity, sampling, measurement, analysis, assumptions, robustness, reproducibility, and whether conclusions exceed the method."
---

# methodology-review

## Purpose

Provide a focused methodological peer review. Merge the repo's methodology reviewer with the Research Architect's alignment logic.

## Review dimensions

### RQ-design fit
Can the chosen design answer the question as worded? Flag causal questions paired with designs that support only association.

### Sampling and case selection
Assess target population, inclusion and exclusion, sampling frame, selection bias, representativeness where relevant, case-selection logic, and sample-size rationale.

### Measurement and data
Assess construct validity, instrument quality, coding reliability, data provenance, missingness, preprocessing, and whether variables match the conceptual claims.

### Identification and confounding
For causal or explanatory inference, identify assumptions and plausible alternative explanations.

### Analysis
Assess whether methods fit the data and estimand. Check model assumptions, multiple testing, effect sizes, uncertainty, qualitative coding procedures, triangulation, or other field-relevant analytical requirements.

### Robustness
Ask which sensitivity analyses or alternative specifications would materially test the conclusion.

### Reproducibility and transparency
Assess whether another researcher could understand and, where appropriate, reproduce the procedure from the reported information.

### Inference boundary
Compare the strongest conclusion in the paper with the strongest conclusion the design can support.

## Output

### Methodology Review
- Summary of design and intended inference
- Major strengths
- Critical issues
- Major issues
- Minor issues
- Missing reporting needed to evaluate the method
- Robustness analyses that would change confidence
- Claims that exceed the design
- Questions a human reviewer is likely to ask

Anchor every major finding to a specific manuscript location or missing expected information.

## General guardrails

- Do not invent sources, citations, quotations, data, results, reviewer comments, or journal requirements.
- Distinguish what is supplied by the user, what is directly verified, what is inferred, and what remains unknown.
- Do not claim a search was exhaustive unless the search process justifies that claim.
- Do not treat source existence as proof that a source supports a particular claim.
- Do not silently strengthen association into causation, a local result into a universal claim, or exploratory evidence into confirmatory evidence.
- If required material is missing, identify the gap and continue with the parts that can be assessed.
- Prefer traceable reasoning. Important findings should point to the exact claim, section, source, table, figure, or reviewer comment that triggered them.
