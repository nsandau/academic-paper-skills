---
name: paper-outline
description: "Convert a coherent paper plan into detailed manuscript architecture with sections, subsections, purpose statements, evidence assignments, transitions, and approximate word allocation."
---

# paper-outline

## Purpose

Represent the paper plan as an executable outline. This skill extracts the repo's structure architect and paper-structure patterns without requiring any pipeline artifacts.

## Structure selection

Choose a structure that fits the paper:
- IMRaD for many empirical studies
- Thematic literature review
- Theoretical or conceptual analysis
- Case study
- Policy or practice paper
- Conference-length paper
- Hybrid structure when justified

Do not force standard structure when the discipline or venue uses a different convention.

## Outline process

### 1. Establish top-level sections
For each section state why it exists and what part of the RQ or argument it serves.

### 2. Decompose into subsections
A subsection should represent a real argumentative or informational unit, not merely a place to distribute words.

### 3. Map evidence
Assign sources, data, analyses, quotations, tables, or figures to the lowest useful section. Mark missing evidence as `NEEDS EVIDENCE` rather than inventing it.

### 4. Add transitions
For every major section boundary state the logical bridge. The transition should explain why the next section follows from the previous one.

### 5. Allocate words
Use approximate ranges. Emphasis should follow argumentative importance, not equal section lengths.

### 6. Check coverage
Verify that every material component of the RQ and central argument has a home in the outline. Remove sections that do not advance the paper.

## Output

### Detailed Outline
For every section and subsection:
- Heading
- Purpose
- Core claim or content
- Evidence assigned
- Figure or table if relevant
- Approximate word count
- Transition to next section
- Missing material

### Outline Diagnostics
- RQ coverage
- Argument coverage
- Evidence gaps
- Structural redundancies
- Sections at risk of becoming descriptive rather than analytical

## General guardrails

- Do not invent sources, citations, quotations, data, results, reviewer comments, or journal requirements.
- Distinguish what is supplied by the user, what is directly verified, what is inferred, and what remains unknown.
- Do not claim a search was exhaustive unless the search process justifies that claim.
- Do not treat source existence as proof that a source supports a particular claim.
- Do not silently strengthen association into causation, a local result into a universal claim, or exploratory evidence into confirmatory evidence.
- If required material is missing, identify the gap and continue with the parts that can be assessed.
- Prefer traceable reasoning. Important findings should point to the exact claim, section, source, table, figure, or reviewer comment that triggered them.
