---
name: figure-table-planner
description: "Decide what should be shown in text, table, or figure, select an appropriate visualization, specify data and caption requirements, and check publication-quality clarity and data consistency."
---

# figure-table-planner

## Purpose

Extract the decision logic from the repo's visualization agent and statistical visualization references while making planning the primary task.

## First question

Does this information need a visual at all?

Use:
- Text for one or two values or a simple qualitative point
- Table for exact values, many variables, or multidimensional comparison
- Figure for patterns, distributions, relationships, trajectories, or effect-size comparison

## Figure selection

Typical mappings:
- Category comparison: bar or dot plot
- Distribution: box, violin, histogram, or density
- Time trend: line plot
- Relationship: scatter plot with appropriate fit or uncertainty
- Many-variable association: heatmap when interpretable
- Meta-analysis: forest plot
- Publication-bias exploration: funnel plot where appropriate
- Conceptual relationships: conceptual diagram, not a fake quantitative chart

Avoid decorative 3D effects and charts that make area or angle comparisons harder than necessary.

## Planning checklist

For each visual specify:
- Analytical question
- Data source
- Variables and units
- Inclusion and filtering rules
- Statistic or transformation
- Uncertainty display
- Ordering
- Labels
- Caption
- Accessibility requirements
- Location in manuscript

## Consistency audit

Before finalizing, compare plotted values with the manuscript's reported values. Flag discrepancies in sample size, effect direction, units, labels, or confidence intervals.

## Output

### Visual Plan
For each proposed table or figure:
- Type
- Purpose
- Data required
- Mapping of variables to visual elements
- Statistical summary
- Caption draft
- Accessibility notes
- Potential misleading choices to avoid
- Manuscript claim it supports

Generate plotting code only when the user asks or provides adequate data.

## General guardrails

- Do not invent sources, citations, quotations, data, results, reviewer comments, or journal requirements.
- Distinguish what is supplied by the user, what is directly verified, what is inferred, and what remains unknown.
- Do not claim a search was exhaustive unless the search process justifies that claim.
- Do not treat source existence as proof that a source supports a particular claim.
- Do not silently strengthen association into causation, a local result into a universal claim, or exploratory evidence into confirmatory evidence.
- If required material is missing, identify the gap and continue with the parts that can be assessed.
- Prefer traceable reasoning. Important findings should point to the exact claim, section, source, table, figure, or reviewer comment that triggered them.
