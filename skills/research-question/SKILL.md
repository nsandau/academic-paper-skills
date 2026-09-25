---
name: research-question
description: "Refine a topic or rough research question into a precise, bounded, answerable research question with subquestions, construct definitions, scope boundaries, feasibility checks, and alternative formulations."
---

# research-question

## Purpose

Turn an initial topic, problem statement, or rough RQ into a researchable question. This skill extracts the repo's FINER-oriented research-question logic while removing pipeline dependencies.

## Process

### 1. Classify the question
Identify whether the main intent is descriptive, comparative, correlational, causal, explanatory, interpretive, evaluative, design-oriented, or evidence-synthesis oriented.

### 2. Define the units
Clarify, where relevant:
- Population or cases
- Context or setting
- Exposure, intervention, phenomenon, or independent variable
- Outcome, response, or dependent variable
- Time period
- Level of analysis

### 3. Test FINER-style quality
Assess:
- Feasible: Can the question be answered with realistic data, access, time, and methods?
- Interesting: Is there a substantive reason to answer it?
- Novel: What would be added relative to nearby work?
- Ethical or permissible: Are there obvious constraints that change feasibility?
- Relevant: Who or what would the answer matter to?

Do not turn this into a numeric score unless the user asks.

### 4. Bound the scope
Produce explicit `in scope` and `out of scope` statements. Flag hidden scope expansion caused by broad terms such as effectiveness, impact, quality, success, or adoption.

### 5. Check answerability
Ask:
- Does the wording imply causation that the likely design cannot establish?
- Are the constructs observable or operationalizable?
- Is the question too broad for one paper?
- Is the question merely a topic with a question mark added?
- Does it bundle multiple questions that should be separated?

### 6. Generate alternatives
Provide two to four formulations that make materially different choices, such as narrower population, mechanism focus, comparative framing, or association rather than causation. Explain the tradeoff of each.

## Output

### Research Question Brief
- Primary RQ
- Question type
- Key constructs and working definitions
- Unit of analysis
- Population or cases
- Context and time boundary
- In scope
- Out of scope
- Two to four subquestions if useful
- Feasibility concerns
- Novelty or contribution hypothesis
- Alternative formulations and tradeoffs
- Open decisions

## General guardrails

- Do not invent sources, citations, quotations, data, results, reviewer comments, or journal requirements.
- Distinguish what is supplied by the user, what is directly verified, what is inferred, and what remains unknown.
- Do not claim a search was exhaustive unless the search process justifies that claim.
- Do not treat source existence as proof that a source supports a particular claim.
- Do not silently strengthen association into causation, a local result into a universal claim, or exploratory evidence into confirmatory evidence.
- If required material is missing, identify the gap and continue with the parts that can be assessed.
- Prefer traceable reasoning. Important findings should point to the exact claim, section, source, table, figure, or reviewer comment that triggered them.
