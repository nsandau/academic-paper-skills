# Standalone Academic Research Skills

A practical extraction and reorganization of useful academic-research workflows from `https://github.com/Imbad0202/academic-research-skills`.

The upstream repository contains strong academic reasoning prompts inside a much larger research-to-publication orchestration system. This package keeps the useful standalone capabilities and removes pipeline state, Material Passports, phase directories, model routing, cross-agent handoff schemas, hooks, hashes, hard gates, and other framework-specific machinery.

This revision was capability-audited against the current upstream `main` on 2026-09-24, including current modes, core agents, specialist protocols, integrity layers, and recent release changes through the v3.22.1 release surface.

## Design goals

- Every skill can be called independently.
- Skills accept ordinary artifacts such as a topic, RQ, paper, notes, bibliography, reviewer comments, results, or target journal.
- Missing upstream artifacts never prevent a skill from doing the part it can do.
- Overlapping source prompts are merged rather than copied as duplicate skills.
- Fact checking, claim support, citation correctness, and manuscript consistency remain separate because they answer different questions.
- Specialist evidence synthesis remains available without cluttering ordinary paper writing.
- Provenance, source version, read scope, and uncertainty remain visible when they affect confidence.

## Install

Install every skill globally for Pi:

```bash
pi-skills add nsandau/academic-paper-skills --global --skill '*' --yes
```

Install selected skills by replacing `'*'` with one or more skill names:

```bash
pi-skills add nsandau/academic-paper-skills --global --skill literature-search evidence-synthesis --yes
```

The repository uses the standard `skills/<skill-name>/SKILL.md` layout, so it can also be installed by other Agent Skills-compatible tools.

## Skills

### Research
- `socratic-research`
- `research-question`
- `research-design`
- `research-brief`

### Evidence
- `literature-search`
- `literature-monitoring`
- `source-evaluator`
- `fact-check`
- `claim-evidence-audit`
- `literature-synthesis`
- `research-gap`
- `evidence-synthesis`

### Planning
- `paper-planner`
- `paper-outline`
- `argument-builder`

### Writing
- `style-calibration`
- `section-writer`
- `academic-writing`
- `figure-table-planner`

### Review
- `argument-stress-test`
- `methodology-review`
- `peer-review`
- `journal-fit`
- `review-synthesis`

### Verification
- `citation-audit`
- `manuscript-integrity-audit`
- `reporting-guidelines`

### Revision
- `revision`

### Submission
- `submission-check`
- `ai-disclosure`

## What was deliberately dropped

### Explicit user exclusions
- Generic format conversion
- Preregistration skill
- Research-ethics skill

### Infrastructure rather than standalone academic reasoning
- Full pipeline orchestrator
- State tracker
- Material Passport and schema machinery
- Phase-number enforcement
- Model tiering
- Cross-model transport machinery
- Hash and replay infrastructure
- Write-scope hooks
- Collaboration-depth scoring
- Agent transport and context plumbing
- Simulated accept or reject verdict as a default workflow

## Audit and source mapping

- `docs/SOURCE_MAP.md` maps each extracted skill to upstream source material.
- `docs/COMPLETENESS_AUDIT.md` records additions, merges, and intentional exclusions from the capability audit.
- `docs/WORKFLOW.md` provides an optional workflow.
- `docs/EXTRACTION_NOTES.md` explains the main design transformations.
