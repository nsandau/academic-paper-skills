---
name: argument-builder
description: "Construct or inspect the argumentative backbone of a paper using thesis, subclaims, claim-evidence-reasoning chains, assumptions, counterarguments, responses, and logical dependencies."
---

# argument-builder

## Purpose

Create an argument map before or during drafting. Merge the repo's Argument Builder with useful Devil's Advocate logic.

## Argument hierarchy

Build:
central thesis -> major claims -> subclaims -> evidence -> reasoning -> assumptions -> counterarguments -> responses

## CER test

For each claim:
- Claim: What exactly is being asserted?
- Evidence: What data, source, or analysis supports it?
- Reasoning: Why does that evidence justify the claim?

Then add:
- Assumptions: What must be true for the reasoning to work?
- Counterargument: What is the strongest credible objection?
- Response: Is there evidence or logic that addresses it?
- Limit: Where should the claim stop?

## Logic checks

Flag:
- Unsupported assertion
- Evidence that is relevant but insufficient
- Circular reasoning
- Non sequitur
- Hidden premise
- False dichotomy
- Causal leap
- Generalization beyond evidence
- Duplicate claims presented as separate contributions
- Subclaim that does not support the thesis
- Counterargument ignored rather than answered

## Output

### Argument Map
For each major claim show:
- Claim
- Role in central thesis
- Evidence
- Reasoning
- Assumptions
- Counterargument
- Response
- Confidence or weakness
- Evidence still needed

### Dependency Map
State which claims must be established before later claims can stand.

### Argument Risks
List the weakest links in order of consequence.

## General guardrails

- Do not invent sources, citations, quotations, data, results, reviewer comments, or journal requirements.
- Distinguish what is supplied by the user, what is directly verified, what is inferred, and what remains unknown.
- Do not claim a search was exhaustive unless the search process justifies that claim.
- Do not treat source existence as proof that a source supports a particular claim.
- Do not silently strengthen association into causation, a local result into a universal claim, or exploratory evidence into confirmatory evidence.
- If required material is missing, identify the gap and continue with the parts that can be assessed.
- Prefer traceable reasoning. Important findings should point to the exact claim, section, source, table, figure, or reviewer comment that triggered them.
