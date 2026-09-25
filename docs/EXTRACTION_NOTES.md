# Extraction notes

## What was preserved

The extraction prioritizes reusable intellectual operations:
- Intent-aware Socratic questioning and convergence cues
- Research-question refinement
- RQ-method alignment
- Rapid evidence briefs
- Reproducible literature searching
- Post-search literature monitoring
- Source verification, cross-index triangulation, version tracking, and read-scope honesty
- Claim-level factual and support verification
- Cross-source synthesis and contradiction analysis
- Research-gap discipline
- Systematic-review specialist workflows
- Paper story and contribution planning
- Evidence-mapped outlining
- Claim-evidence-reasoning argument maps
- Author style calibration
- Section-level academic drafting
- Introduction, discussion, abstract, and prose diagnostics
- Publication-quality figure and table planning
- Devil's Advocate stress testing with concession discipline
- Methodology and multi-perspective peer review
- Quick and guided review modes
- Bounded reviewer calibration
- Journal-fit analysis
- Review synthesis
- Citation, temporal, originality, and whole-manuscript integrity audits
- Reporting-guideline compliance
- Reviewer-response revision workflows
- Scoped revision and claim-drift safeguards
- Submission preflight and AI disclosure

## What was removed

The following were treated as implementation infrastructure rather than academic skills:
- Orchestrator stages
- Mandatory pipeline checkpoints
- State persistence
- Material Passport contracts
- Schema registries
- Cross-model envelopes and transport plumbing
- Tool hooks
- Hash and replay controls
- Phase file-write restrictions
- Model tiers
- Reviewer identity plumbing
- CI and release-discipline machinery
- Collaboration-depth scoring
- Simulated editorial authority

## Explicit user exclusions

The user asked not to include:
- preregistration
- research ethics as a standalone skill
- format conversion

Research reporting statements that venues require can still be checked by `submission-check` and `reporting-guidelines` without recreating a general research-ethics skill.

## Important transformations

### Source quality and triangulation
The upstream repo contains evidence hierarchies and deterministic citation-index checks. The extracted `source-evaluator` uses evidence strength relative to the claim and treats index disagreement as a risk signal rather than a universal hierarchy or automatic fabrication verdict.

### Read scope
The package now preserves the useful upstream distinction between full-text, section, abstract-only, TOC-only, metadata-only, and unknown inspection. Claim-support judgments must not exceed the material actually read.

### Source versions
Citation and source checks now distinguish preprints, accepted manuscripts, conference versions, and versions of record. Metadata and quoted support should come from the same version family member unless the difference is explicitly handled.

### Socratic convergence
The upstream mentor tracks intent and convergence. The extracted skill keeps exploratory versus goal-oriented behavior, reading probes, and dialogue-health checks without fixed round counts.

### Paper planning
The original plan mode requires repeated chapter rounds. The extracted `paper-planner` asks questions only when decisions are unresolved and begins with an explicit paper-configuration step before producing a Paper Blueprint.

### Integrity verification
The upstream pipeline uses registered populations, deterministic checks, and hard gates. The extracted audit skills keep the substantive checks while dropping certification language and infrastructure-dependent PASS states.

### Temporal integrity
The extracted integrity and fact-check skills preserve five useful failure classes from the upstream temporal layer: impossible date arithmetic, anachronistic citation use, unmaterialized comparators, causal inversion, and unanchored current/latest wording.

### Originality
The extracted integrity skill supports evidence-based overlap and self-reuse checks. It explicitly does not claim reliable AI-authorship detection and does not treat textual similarity alone as proof of misconduct.

### Peer review
The original reviewer simulates a journal panel. The extracted version keeps full, quick, guided, methodology, domain, argument, perspective, adversarial, and bounded calibration behaviors without default publication verdicts or false independence claims.

### Revision
The extracted revision skill keeps coach, rebuttal, rebuttal-audit, and verification modes. It also adds patch-scoped editing, claim-strength drift checks, and numeric/citation conservation for touched text.

### Reporting guidelines
The upstream repo contains an EQUATOR mapping. The extracted skill does not freeze old guideline versions. It requires current official verification when the exact checklist or version matters.
