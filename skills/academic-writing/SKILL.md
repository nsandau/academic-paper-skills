---
name: academic-writing
description: "Diagnose and improve academic rhetoric and prose with modes for introductions, discussions, abstracts, titles and keywords, and general writing quality."
---

# academic-writing

## Purpose

Provide specialist academic-writing diagnostics and rewriting without becoming a full drafting pipeline.

## Modes

- `introduction`
- `discussion`
- `abstract`
- `title-keywords`
- `prose-check`

Read the matching reference file when using introduction, discussion, abstract, or prose-check mode.

## Optional style profile

If the user supplies a `style-calibration` profile, use it as a soft guide after accuracy, evidence boundaries, discipline conventions, target-venue rules, and clarity. Do not imitate distinctive phrases or preserve poor prose merely to match the profile.

## Shared principles

- Precision beats generic academic-sounding language.
- Paragraph boundaries should follow argumentative turns rather than a fixed length.
- Avoid throat-clearing openings that merely announce what a section will do.
- Match hedging to the strength of evidence.
- Prefer discipline-specific vocabulary over vague intensifiers.
- Preserve necessary technical complexity while removing needless syntactic complexity.
- Treat the user's established writing voice as a soft guide, not a reason to preserve unclear prose.

## Output

For diagnostic requests, identify the problem, why it matters, and a concrete revision. For rewriting requests, preserve meaning and evidence boundaries. Do not introduce new claims merely to make prose sound stronger.

## General guardrails

- Do not invent sources, citations, quotations, data, results, reviewer comments, or journal requirements.
- Distinguish what is supplied by the user, what is directly verified, what is inferred, and what remains unknown.
- Do not claim a search was exhaustive unless the search process justifies that claim.
- Do not treat source existence as proof that a source supports a particular claim.
- Do not silently strengthen association into causation, a local result into a universal claim, or exploratory evidence into confirmatory evidence.
- If required material is missing, identify the gap and continue with the parts that can be assessed.
- Prefer traceable reasoning. Important findings should point to the exact claim, section, source, table, figure, or reviewer comment that triggered them.
