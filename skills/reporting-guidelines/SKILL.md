---
name: reporting-guidelines
description: "Identify the reporting guideline appropriate to a study or review, verify the current official checklist when possible, and audit a manuscript for transparent reporting without conflating reporting completeness with study quality."
---

# reporting-guidelines

## Purpose

Help researchers select and apply discipline-appropriate reporting guidance, especially established checklists indexed by the EQUATOR Network or maintained by the relevant guideline organization.

This skill audits reporting completeness. It does not certify that a study is methodologically sound, ethical, or publishable.

## Common guideline families

Examples include:
- PRISMA and relevant extensions for systematic and scoping reviews
- CONSORT and relevant extensions for randomized trials
- STROBE for observational epidemiological studies
- COREQ or SRQR for qualitative research
- STARD for diagnostic accuracy studies
- TRIPOD-family guidance for prediction models, including AI-specific extensions where applicable
- CARE for case reports
- SQUIRE for quality-improvement studies
- CHEERS for economic evaluations
- ARRIVE for animal research

Do not assume this list is complete or that a remembered version is current. Reporting standards change. When current compliance matters and external access is available, verify the official guideline, extension, version, and checklist before auditing.

### AI-assisted evidence synthesis

When AI or automation materially participates in a systematic review, scoping review, rapid review, evidence map, or meta-analysis, also consider AI-specific transparency frameworks. The upstream repository includes PRISMA-trAIce and RAISE logic. Preserve their maturity boundaries:
- PRISMA-trAIce should be described according to its current published status and official source. Do not silently present a preliminary or living proposal as a mature consensus standard.
- RAISE is scoped to evidence synthesis. Applying its principles to ordinary primary-research manuscripts is an extension, not official RAISE compliance.

For AI-assisted synthesis, check transparency about tool identity and version, purpose and stage, input and output handling, prompts or relevant configuration, human oversight, performance evaluation, reproducibility, fit for purpose, study-selection handling, and limitations. Verify the current framework before claiming compliance.

## Workflow

### 1. Identify study type
Determine the actual design, not merely the manuscript label. Mixed or hybrid designs may require more than one checklist.

### 2. Select the guideline
State:
- primary guideline
- applicable extension if any
- why it applies
- official source and current version when verified
- any uncertainty about applicability

### 3. Build an item-level checklist
Use the official checklist where accessible. Preserve item numbering when practical so the author can trace findings back to the source guideline.

### 4. Audit the manuscript
For each applicable item use:
- `present`
- `partial`
- `missing`
- `not applicable`
- `cannot verify`

Point to the manuscript location for present items and the missing information for deficient items.

### 5. Distinguish reporting from methodological quality
A manuscript can fully report a weak design. A strong study can be poorly reported. Do not convert checklist completion into an overall quality score.

## Output

### Guideline Selection
- Study design
- Guideline and extension
- Version / date if verified
- Applicability rationale
- Verification source

### Compliance Matrix
For each item:
- checklist item
- status
- manuscript location
- missing or ambiguous information
- suggested action

### Priority Repairs
Separate omissions that materially affect reproducibility or interpretation from lower-impact formatting and disclosure omissions.

### Unverified Requirements
List guideline items or venue-specific requirements that could not be confirmed.

## Boundaries

- Use official or authoritative guideline sources when verifying current requirements.
- Do not invent checklist items or current versions.
- Do not mark `not applicable` merely because information is inconvenient to report.
- Do not treat reporting-guideline compliance as a substitute for `methodology-review`.
