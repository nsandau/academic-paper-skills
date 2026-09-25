---
name: evidence-synthesis
description: "Plan and conduct systematic evidence synthesis with modes for systematic review, risk of bias, meta-analysis, and certainty of evidence, while keeping each specialist operation independently callable."
---

# evidence-synthesis

## Purpose

Provide specialist evidence-synthesis workflows without forcing them into ordinary paper writing.

## Modes

- `systematic-review`: protocol, search, screening, extraction, synthesis, PRISMA-style reporting
- `risk-of-bias`: structured study-level bias assessment using the correct instrument for the study design
- `meta-analysis`: feasibility, effect sizes, pooling, heterogeneity, sensitivity, subgroup analysis, and publication-bias assessment
- `evidence-certainty`: outcome-level certainty assessment such as GRADE where appropriate

Read the matching file in `references/` before performing a mode.

## Shared principles

- Decide eligibility and analysis rules before looking at pooled results when possible.
- Keep the study-selection denominator visible.
- Use study-design appropriate bias tools.
- Do not pool studies merely because numerical pooling is possible.
- Investigate clinical, methodological, and statistical heterogeneity.
- Separate pre-specified from post-hoc subgroup analyses.
- Report null and inconvenient findings as well as positive ones.
- Treat certainty of evidence as distinct from effect magnitude.

## Output

The selected mode defines the primary output. When several modes are requested, keep the artifacts distinct so a later user can inspect screening, risk of bias, quantitative synthesis, and certainty judgments separately.

## General guardrails

- Do not invent sources, citations, quotations, data, results, reviewer comments, or journal requirements.
- Distinguish what is supplied by the user, what is directly verified, what is inferred, and what remains unknown.
- Do not claim a search was exhaustive unless the search process justifies that claim.
- Do not treat source existence as proof that a source supports a particular claim.
- Do not silently strengthen association into causation, a local result into a universal claim, or exploratory evidence into confirmatory evidence.
- If required material is missing, identify the gap and continue with the parts that can be assessed.
- Prefer traceable reasoning. Important findings should point to the exact claim, section, source, table, figure, or reviewer comment that triggered them.
