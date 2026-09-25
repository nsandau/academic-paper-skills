---
name: ai-disclosure
description: "Prepare an accurate venue-specific disclosure of AI use based on the actual use described by the author and current verified publisher or journal policy, without inventing compliance requirements."
---

# ai-disclosure

## Purpose

Extract the repo's disclosure mode while keeping it small and standalone.

## Inputs

- Target journal, conference, publisher, institution, or policy text
- Actual AI tools used
- What the tools were used for
- Whether AI-generated text, analysis, code, images, translation, editing, or literature assistance entered the work
- Any author verification or editing performed

## Process

1. Verify the applicable policy from an official source when current rules matter.
2. Distinguish mandatory disclosure from recommended disclosure and from actions that are prohibited or restricted.
3. Map the user's actual use to the policy language.
4. Do not imply that using AI makes it an author.
5. Do not conceal use that the policy requires authors to disclose.
6. Do not over-disclose irrelevant internal assistance if the policy does not require it, unless the user wants a broader transparency statement.

## Output

### Policy status
- Venue and policy source
- Date checked
- Applicability
- Required elements
- Unknown or ambiguous points

### Disclosure text
Produce a concise statement that accurately describes the user's actual AI use and does not claim compliance beyond what was verified.

## General guardrails

- Do not invent sources, citations, quotations, data, results, reviewer comments, or journal requirements.
- Distinguish what is supplied by the user, what is directly verified, what is inferred, and what remains unknown.
- Do not claim a search was exhaustive unless the search process justifies that claim.
- Do not treat source existence as proof that a source supports a particular claim.
- Do not silently strengthen association into causation, a local result into a universal claim, or exploratory evidence into confirmatory evidence.
- If required material is missing, identify the gap and continue with the parts that can be assessed.
- Prefer traceable reasoning. Important findings should point to the exact claim, section, source, table, figure, or reviewer comment that triggered them.
