---
name: submission-check
description: "Run a final pre-submission checklist against a manuscript and target venue, covering required files, anonymization, word limits, figures, tables, reporting statements, references, disclosures, data and code statements, and submission-specific requirements."
---

# submission-check

## Purpose

Perform a practical submission preflight. Verify current venue rules from official sources when they are material and web access is available.

## Checklist areas

### Manuscript identity
- Title page
- Author information
- Corresponding author details
- ORCID if required
- Blinded or anonymized manuscript where required

### Main manuscript
- Correct article type
- Word limit
- Abstract format and limit
- Keywords
- Heading structure
- Tables and figures cited in order
- Figure resolution and file type requirements if specified
- Supplementary material references

### Research reporting
Identify any applicable reporting guideline and use `reporting-guidelines` for item-level compliance. Verify the current official version when material.

As applicable:
- Reporting checklist
- Ethics or approval statement
- Consent statement
- Trial or review registration
- Data availability
- Code availability
- Materials availability
- Funding
- Conflicts of interest
- Author contributions
- Acknowledgements

### References
- Style
- Completeness
- DOI requirements
- Reference limits if any

### Submission package
- Cover letter if needed
- Highlights, graphical abstract, key points, or lay summary if required
- Suggested or opposed reviewers if requested
- Supplementary files
- Reporting checklists

## Output

### Submission Preflight
Use statuses:
- ready
- needs action
- not applicable
- cannot verify

For every `needs action`, state the exact file or manuscript change required. Distinguish verified venue requirements from general best practice.

## General guardrails

- Do not invent sources, citations, quotations, data, results, reviewer comments, or journal requirements.
- Distinguish what is supplied by the user, what is directly verified, what is inferred, and what remains unknown.
- Do not claim a search was exhaustive unless the search process justifies that claim.
- Do not treat source existence as proof that a source supports a particular claim.
- Do not silently strengthen association into causation, a local result into a universal claim, or exploratory evidence into confirmatory evidence.
- If required material is missing, identify the gap and continue with the parts that can be assessed.
- Prefer traceable reasoning. Important findings should point to the exact claim, section, source, table, figure, or reviewer comment that triggered them.
