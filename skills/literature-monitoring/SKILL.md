---
name: literature-monitoring
description: "Update an existing evidence base after a defined cutoff date by finding consequential new publications, corrections, retractions, contradictory findings, terminology shifts, and citation developments, then recommend what needs attention."
---

# literature-monitoring

## Purpose

Maintain an existing research evidence base after the original search or manuscript was completed.

This is not a fresh literature review. Start from the user's existing research question, bibliography, search strategy, major claims, and last-search date. The core question is: what has appeared since the baseline that is important enough to change, strengthen, weaken, or update the research?

## Inputs

Use whatever is available:
- Research question or topic
- Existing bibliography or included-study set
- Original search terms or database queries
- Key authors, journals, datasets, theories, or standards
- Existing synthesis or manuscript
- Last-search or evidence-cutoff date
- Areas the user considers especially decision-relevant

If the cutoff date is unknown, state the assumed boundary rather than silently inventing one.

## Modes

- `update-scan`: find consequential literature since the cutoff
- `retraction-correction`: check cited sources for retractions, expressions of concern, or material corrections
- `contradictions`: focus on new findings that materially challenge the existing synthesis
- `author-journal`: track activity from important authors and venues
- `keyword-evolution`: detect terminology or framing that could make the old search strategy stale
- `alert-plan`: design practical alerts the user can configure in external databases or services

## Workflow

### 1. Reconstruct the baseline
Summarize the original RQ, evidence cutoff, key claims, important sources, and search concepts. Separate what is documented from what is inferred.

### 2. Search only the update window
Use the original concepts plus newly emerged terms. Reuse database-specific logic where possible. Record the date boundary and any search coverage limitations.

### 3. Verify candidate sources
For consequential candidates, verify bibliographic identity, version, publication status, and read scope. Use multiple bibliographic indexes when practical. Do not treat one failed lookup as proof a source is fabricated.

### 4. Compare new evidence with the baseline
Classify each important item by how it relates to the existing evidence base:
- strengthens
- weakens
- contradicts
- narrows or adds a boundary condition
- updates a method, measure, dataset, standard, or policy
- corrects or retracts prior evidence
- introduces a new terminology or research direction
- relevant but does not materially change the synthesis

### 5. Prioritize signal over volume
High priority items include:
- Retractions or material corrections affecting cited work
- Stronger evidence that reverses or substantially qualifies a central conclusion
- Direct replications or failures to replicate
- Major new systematic reviews, trials, datasets, standards, or methods
- New work that invalidates a novelty claim or closes an identified gap

Routine publications should not crowd out consequential changes.

### 6. Recommend an action
Every high or medium priority item should have an action such as:
- read full text
- add citation
- revise a claim
- update a table or figure
- rerun a synthesis or meta-analysis
- replace a retracted source
- expand the search vocabulary
- no manuscript change needed

## Output

### Monitoring Baseline
- Topic / RQ
- Evidence cutoff
- Existing evidence base used
- Search concepts reused
- Coverage limitations

### High-Priority Developments
For each item:
- Citation and verification status
- Development type
- Relation to existing claim or source
- Evidence strength and read scope
- Likely impact
- Recommended action

### Other Relevant Updates
Summarize lower-impact publications without implying they materially change the paper.

### Search-Strategy Drift
List new terms, authors, journals, methods, or indexing changes that suggest the original search should be updated.

### Retraction and Correction Status
List any affected sources and which manuscript claims depend on them.

### Monitoring Recommendation
Suggest a reasonable future cadence only when the user wants continuing monitoring. Do not pretend background monitoring is running unless the environment actually supports scheduled tasks.

## Boundaries

- A monitoring scan is not automatically exhaustive.
- Abstract-only evidence must be labeled as such.
- Newer does not automatically mean stronger.
- A contradictory paper is not automatically decisive. Compare design, population, measures, and evidence quality.
- Do not claim a cited source has been retracted or corrected without verification.
- Do not silently replace the original search strategy. Report material changes.
