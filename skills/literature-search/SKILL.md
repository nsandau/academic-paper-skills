---
name: literature-search
description: "Design a reproducible academic literature search, including concept decomposition, keywords, Boolean queries, databases, screening criteria, snowballing, reconnaissance, and search documentation."
---

# literature-search

## Purpose

Create a search strategy that can be explained and repeated. Merge the repo's bibliography agent, literature strategist, corpus-first logic, and three-way WHY/HOW/WHAT scan.

## Modes

- `full`: reproducible search strategy with screening and documentation
- `reconnaissance`: fast field-entry scan organized as WHY, HOW, and WHAT
- `update`: search for material published after an existing review or search date

## Full search workflow

### 1. Decompose the RQ
Extract concept blocks such as population, phenomenon, intervention, outcome, mechanism, context, and method.

### 2. Expand terminology
For each concept, generate:
- Synonyms
- Alternative spellings
- Acronyms
- Broader and narrower terms
- Field-specific terminology
- Historical terminology when relevant

Do not indiscriminately OR every synonym. Keep query precision manageable.

### 3. Select sources
Choose databases based on discipline and evidence type. Distinguish bibliographic databases, citation indexes, preprint servers, trial registries, policy repositories, and grey-literature sources.

### 4. Build search strings
Produce database-adaptable Boolean queries with concept blocks. Note fields searched such as title, abstract, or keywords when known.

### 5. Define eligibility
Specify inclusion and exclusion criteria before screening when possible:
- Population or context
- Study or document type
- Time range
- Language
- Publication status
- Methods
- Outcomes or themes

### 6. Screen consistently
Use the same criteria for user-supplied papers and newly found papers. Never silently skip supplied corpus items. Record why an item was included, excluded, or left unresolved.

### 7. Snowball
Use backward reference checking and forward citation tracking on central sources. Add author, theory, dataset, instrument, and key-term searches when they uncover gaps.

### 8. Document the search
Record databases, dates, exact search strings, filters, search counts when available, screening decisions, and known coverage gaps.

## Reconnaissance mode

Organize a small, high-value set of papers into:
- WHY: establishes the problem, motivation, or theoretical need
- HOW: provides methods, measures, datasets, or analytical approaches
- WHAT: provides current findings, interventions, mechanisms, or solutions

Then synthesize what the three groups imply for the project. Do not present this as a systematic review.

## Output

### Search Strategy
- RQ and concept blocks
- Databases and rationale
- Search strings
- Inclusion criteria
- Exclusion criteria
- Screening process
- Snowballing plan
- Update-search boundary if applicable

### Search Log Template
Provide a compact table for database, date, query, filters, hits, screened, included, and notes.

### Coverage Gaps
Identify concepts, populations, periods, or disciplines that remain weakly covered.

## General guardrails

- Do not invent sources, citations, quotations, data, results, reviewer comments, or journal requirements.
- Distinguish what is supplied by the user, what is directly verified, what is inferred, and what remains unknown.
- Do not claim a search was exhaustive unless the search process justifies that claim.
- Do not treat source existence as proof that a source supports a particular claim.
- Do not silently strengthen association into causation, a local result into a universal claim, or exploratory evidence into confirmatory evidence.
- If required material is missing, identify the gap and continue with the parts that can be assessed.
- Prefer traceable reasoning. Important findings should point to the exact claim, section, source, table, figure, or reviewer comment that triggered them.
