---
name: section-writer
description: "Draft or revise one academic manuscript section from supplied evidence, outline, argument, results, and venue constraints without inventing missing material or citations."
---

# section-writer

## Purpose

Write one section at a time using the user's evidence and plan. This is a standalone rewrite of the repo's tightly coupled draft writer and report compiler.

## Optional author style

When a `style-calibration` profile is supplied, apply it as a soft guide after discipline and venue conventions. Preserve meaning and evidence boundaries over stylistic similarity.

## Inputs

Use whatever the user provides:
- Section purpose
- Outline
- Argument map
- Source notes or full sources
- Results or data
- Target word count
- Discipline and venue
- Neighboring sections
- Existing author prose or style sample

## Process

1. Restate the section's job in one sentence.
2. Identify claims that have adequate support.
3. Mark unsupported required claims as `MATERIAL GAP` in planning notes rather than filling them.
4. Organize paragraphs around argumentative units.
5. Integrate citations only from verified or supplied sources.
6. Preserve distinctions between literature claims and the paper's own findings.
7. Use appropriate hedging based on evidence strength.
8. Maintain continuity with adjacent sections.
9. End where the next section should logically begin.

## Section modes

- introduction
- literature-review
- theory
- methods
- results
- discussion
- conclusion
- custom

When `introduction`, `discussion`, or `abstract` requires specialist rhetoric, the `academic-writing` skill may provide a more targeted diagnostic.

## Writing constraints

- Do not create a citation merely because a sentence seems to need one.
- Do not invent sample sizes, p-values, effect sizes, quotations, or limitations.
- Do not hide uncertainty with vague prose.
- Do not pad a section to hit a target word count.
- Preserve the author's substantive position unless explicitly asked to change it.

## Output

Return the finished section followed by a short `Material gaps` note only when there are unresolved evidence or factual gaps that the user must address.

## General guardrails

- Do not invent sources, citations, quotations, data, results, reviewer comments, or journal requirements.
- Distinguish what is supplied by the user, what is directly verified, what is inferred, and what remains unknown.
- Do not claim a search was exhaustive unless the search process justifies that claim.
- Do not treat source existence as proof that a source supports a particular claim.
- Do not silently strengthen association into causation, a local result into a universal claim, or exploratory evidence into confirmatory evidence.
- If required material is missing, identify the gap and continue with the parts that can be assessed.
- Prefer traceable reasoning. Important findings should point to the exact claim, section, source, table, figure, or reviewer comment that triggered them.
