# Capability completeness audit

Audit date: 2026-09-24

Upstream: `https://github.com/Imbad0202/academic-research-skills`

Reference surface: current upstream `main`, root mode registry, the three substantive user-facing skills, pipeline integrity logic, shared protocols, core agents and references, architecture documentation, and recent release notes through the v3.22.1 release surface.

## What this audit means

This is a capability-level audit, not an attempt to reproduce every file or implementation mechanism from the upstream repository.

Every substantive academic workflow identified in the reviewed upstream surfaces was assigned to one of four outcomes:
1. extracted as its own skill
2. merged into a broader standalone skill
3. retained as a mode or reference module
4. deliberately excluded and documented

Implementation-only mechanisms are not considered missing capabilities.

## Additions made after the first extraction

### New standalone skills
- `literature-monitoring`
- `style-calibration`
- `reporting-guidelines`
- `research-brief`

### Strengthened existing skills
- `socratic-research`: intent detection, exploratory versus goal-oriented dialogue, reading probes, dialogue-health checks
- `source-evaluator`: multi-index triangulation, version consistency, read scope
- `citation-audit`: multi-index verification, DOI-resolution honesty, version-family consistency
- `fact-check`: temporal verification and read-scope awareness
- `claim-evidence-audit`: locators, read scope, negative constraints, version mismatches, transparent coverage
- `manuscript-integrity-audit`: temporal integrity and originality / self-reuse checking
- `argument-stress-test`: concession discipline and open-objection ledger
- `peer-review`: quick, guided, and calibration modes with calibration epistemic boundaries
- `paper-planner`: explicit intake and paper configuration
- `academic-writing` and `section-writer`: optional style-profile consumption
- `revision`: patch-scoped edits, claim-strength drift checks, number and citation conservation
- `submission-check`: reporting-guideline integration
- `evidence-synthesis`: current-guideline verification rather than frozen checklist versions
- `reporting-guidelines`: AI-assisted evidence-synthesis transparency using PRISMA-trAIce and RAISE with explicit maturity and scope limits

## Upstream capabilities merged rather than kept as separate skills

- Three-way WHY/HOW/WHAT scan -> `literature-search` reconnaissance mode
- Deep-research quick mode -> `research-brief`
- Deep-research review mode -> distributed across `source-evaluator`, `peer-review`, and `argument-stress-test`
- Academic-paper plan mode -> `paper-planner`, `paper-outline`, `argument-builder`, `socratic-research`
- Academic-paper outline-only -> `paper-outline`
- Academic-paper citation-check -> `citation-audit`
- Academic-paper abstract-only -> `academic-writing` abstract mode
- Academic-paper lit-review -> `literature-search` + `literature-synthesis`
- Reviewer methodology-focus -> `methodology-review` and `peer-review` methodology mode
- Reviewer re-review -> `revision` verify mode
- Editorial synthesis -> `review-synthesis`
- Field-analysis reviewer configuration -> internal logic in `peer-review`
- Integrity-verification phases -> `citation-audit`, `claim-evidence-audit`, `fact-check`, `manuscript-integrity-audit`
- Temporal timeline layer -> `fact-check` temporal mode + `manuscript-integrity-audit` temporal mode
- Style profile consumption -> `style-calibration`, `section-writer`, `academic-writing`
- EQUATOR routing -> `reporting-guidelines`

## Deliberate user-requested exclusions

- preregistration
- standalone research-ethics skill
- format conversion

## Deliberate infrastructure exclusions

- academic-pipeline orchestrator
- pipeline state machine
- Material Passports
- schema and handoff contracts
- hashes and replay validators
- phase and write-scope enforcement
- model tiering
- cross-model transport adapters
- hooks and CI gates
- collaboration-depth scoring
- release engineering and repository-maintenance tooling
- process-summary scoring

## Deliberate epistemic simplifications

### Reviewer calibration
The upstream calibration implementation contains execution-topology and transport controls. The extracted skill keeps the scientifically useful ideas: gold-label isolation, bounded target identity, directional versus full tiers, FNR/FPR/balanced-accuracy boundaries, categorical dimension agreement, and explicit non-transportability. It does not pretend a normal single-context chat can establish independent repeated reviewer errors.

### Citation verification
The upstream repo contains deterministic resolver clients and gate thresholds. The extracted skills preserve cross-index verification and uncertainty semantics without copying resolver-specific CI policy or turning index absence into automatic rejection.

### Originality checking
The upstream integrity agent samples web overlap and prior author publications. The extracted audit retains attribution and self-reuse checks but rejects AI-authorship detection as a reliable integrity test.

### Reporting guidelines
The upstream mapping includes specific checklist versions that can become stale. The extracted skill maps study types but requires current official verification for exact checklist use.

## Residual boundary

The upstream repository changes frequently. This package is complete relative to the capability audit date, not guaranteed to include capabilities added upstream afterward. `literature-monitoring` can help track substantive research changes, but repository feature changes require a future extraction audit.
