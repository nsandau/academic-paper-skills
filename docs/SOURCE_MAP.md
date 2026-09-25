# Source map

This file documents which parts of the original repository were used as source material for each standalone skill. The extraction is a reorganization and rewrite, not a claim that any original file maps one-to-one to the new skill.

## `academic-writing`
- `academic-paper/references/writing_quality_check.md`
- `academic-paper/references/writing_judgment_framework.md`
- `academic-paper/references/intro_title_rhetoric_guide.md`
- `academic-paper/agents/abstract_bilingual_agent.md`
- `academic-paper/agents/draft_writer_agent.md`
- `shared/style_calibration_protocol.md` for style-profile consumption rules

## `ai-disclosure`
- academic-paper disclosure mode
- `academic-paper/references/disclosure_mode_protocol.md`
- `academic-paper/references/venue_disclosure_policies.md`
- `academic-paper/references/policy_anchor_disclosure_protocol.md`

## `argument-builder`
- `academic-paper/agents/argument_builder_agent.md`
- `deep-research/agents/devils_advocate_agent.md`
- `academic-paper-reviewer/agents/devils_advocate_reviewer_agent.md`

## `argument-stress-test`
- `deep-research/agents/devils_advocate_agent.md`
- `academic-paper-reviewer/agents/devils_advocate_reviewer_agent.md`
- upstream logical-fallacy references
- reviewer concession-threshold and anti-sycophancy logic summarized in `docs/ARCHITECTURE.md`

## `citation-audit`
- `academic-paper/agents/citation_compliance_agent.md`
- `academic-pipeline/agents/integrity_verification_agent.md`
- deterministic citation-existence and triangulation work documented in upstream release history and architecture
- citation version-drift / version-family work represented by upstream issue and PR #754/#763
- `deep-research/references/semantic_scholar_api_protocol.md`

## `claim-evidence-audit`
- `academic-pipeline/agents/claim_ref_alignment_audit_agent.md`
- `academic-pipeline/references/claim_verification_protocol.md`
- `academic-pipeline/agents/integrity_verification_agent.md`
- locator and read-scope provenance features documented in upstream release notes

## `evidence-synthesis`
- deep-research systematic-review mode
- `deep-research/agents/risk_of_bias_agent.md`
- `deep-research/agents/meta_analysis_agent.md`
- `deep-research/references/systematic_review_toolkit.md`
- `deep-research/references/equator_reporting_guidelines.md`

## `fact-check`
- deep-research fact-check mode
- `deep-research/agents/source_verification_agent.md`
- `academic-pipeline/agents/integrity_verification_agent.md`
- `academic-pipeline/references/claim_verification_protocol.md`
- temporal-integrity rules from `academic-paper/agents/draft_writer_agent.md`, `agents/report_compiler_agent.md`, and upstream v3.9.4 release documentation

## `figure-table-planner`
- `academic-paper/agents/visualization_agent.md`
- `academic-paper/references/statistical_visualization_standards.md`
- `academic-paper/references/vlm_figure_verification.md`

## `journal-fit`
- `academic-paper-reviewer/agents/eic_agent.md`
- `academic-paper-reviewer/agents/field_analyst_agent.md`
- `academic-paper-reviewer/references/top_journals_by_field.md`
- `academic-paper/references/journal_submission_guide.md`

## `literature-monitoring`
- `deep-research/agents/monitoring_agent.md`
- `deep-research/references/literature_monitoring_strategies.md`
- source verification and synthesis logic used for prioritizing update findings

## `literature-search`
- `deep-research/agents/bibliography_agent.md`
- `academic-paper/agents/literature_strategist_agent.md`
- deep-research three-way-scan mode
- `academic-pipeline/references/literature_corpus_consumers.md`

## `literature-synthesis`
- `deep-research/agents/synthesis_agent.md`
- deep-research three-way-scan mode

## `manuscript-integrity-audit`
- `academic-pipeline/agents/integrity_verification_agent.md`
- `academic-pipeline/agents/claim_ref_alignment_audit_agent.md`
- `academic-pipeline/references/plagiarism_detection_protocol.md`
- upstream temporal-integrity layer documented in v3.9.4 release notes and architecture
- `academic-paper/references/vlm_figure_verification.md`
- `academic-pipeline/references/ai_research_failure_modes.md`
- shared cross-document consistency protocols

## `methodology-review`
- `academic-paper-reviewer/agents/methodology_reviewer_agent.md`
- `deep-research/agents/research_architect_agent.md`
- `academic-paper-reviewer/references/review_criteria_framework.md`

## `paper-outline`
- `academic-paper/agents/structure_architect_agent.md`
- `academic-paper/references/paper_structure_patterns.md`
- `academic-paper/references/plan_mode_protocol.md`

## `paper-planner`
- `academic-paper/references/plan_mode_protocol.md`
- `academic-paper/agents/intake_agent.md`
- `academic-paper/agents/socratic_mentor_agent.md`
- `deep-research/agents/socratic_mentor_agent.md`
- `academic-paper/agents/structure_architect_agent.md`
- `academic-paper/agents/argument_builder_agent.md`

## `peer-review`
- `academic-paper-reviewer/SKILL.md`
- `academic-paper-reviewer/agents/field_analyst_agent.md`
- `academic-paper-reviewer/agents/eic_agent.md`
- `academic-paper-reviewer/agents/methodology_reviewer_agent.md`
- `academic-paper-reviewer/agents/domain_reviewer_agent.md`
- `academic-paper-reviewer/agents/perspective_reviewer_agent.md`
- `academic-paper-reviewer/agents/devils_advocate_reviewer_agent.md`
- `academic-paper-reviewer/references/guided_mode_protocol.md`
- `academic-paper-reviewer/references/calibration_mode_protocol.md`
- `academic-paper/agents/peer_reviewer_agent.md`

## `reporting-guidelines`
- `deep-research/references/equator_reporting_guidelines.md`
- `deep-research/references/methodology_patterns.md`
- reporting-compliance logic in the upstream integrity and submission layers
- `shared/prisma_trAIce_protocol.md`
- `shared/raise_framework.md`

## `research-brief`
- deep-research `quick` mode
- `deep-research/references/mode_selection_guide.md`
- bibliography, source-verification, and synthesis agents in bounded form

## `research-design`
- `deep-research/agents/research_architect_agent.md`
- `academic-paper-reviewer/agents/methodology_reviewer_agent.md`
- `deep-research/agents/devils_advocate_agent.md`

## `research-gap`
- `deep-research/agents/synthesis_agent.md`
- `academic-paper/agents/literature_strategist_agent.md`
- academic-paper quality rules for novelty and absence claims
- `academic-paper-reviewer/agents/eic_agent.md`

## `research-question`
- `deep-research/agents/research_question_agent.md`
- `deep-research/agents/socratic_mentor_agent.md`

## `review-synthesis`
- `academic-paper-reviewer/agents/editorial_synthesizer_agent.md`
- `academic-paper/agents/revision_coach_agent.md`

## `revision`
- `academic-paper/agents/revision_coach_agent.md`
- academic-paper revision mode
- academic-paper rebuttal-audit mode
- academic-paper-reviewer re-review mode
- `academic-paper-reviewer/agents/editorial_synthesizer_agent.md`
- revision claim-drift and token-conservation safeguards documented in upstream v3.19-v3.20 release notes

## `section-writer`
- `academic-paper/agents/draft_writer_agent.md`
- `deep-research/agents/report_compiler_agent.md`
- `academic-paper/references/academic_writing_style.md`
- `academic-paper/references/writing_quality_check.md`
- `academic-paper/references/anti_leakage_protocol.md`
- `shared/style_calibration_protocol.md` for optional author-style consumption

## `socratic-research`
- `deep-research/agents/socratic_mentor_agent.md`
- deep-research Socratic intent routing in `deep-research/SKILL.md`
- Socratic reading-probe feature documented in setup and current skill references
- `deep-research/agents/research_question_agent.md`
- `deep-research/agents/devils_advocate_agent.md`
- `academic-paper/agents/socratic_mentor_agent.md`
- `academic-paper/references/plan_mode_protocol.md`

## `source-evaluator`
- `deep-research/agents/source_verification_agent.md`
- `deep-research/references/source_quality_hierarchy.md`
- cross-index triangulation and read-scope features documented in current upstream architecture and release notes

## `style-calibration`
- `shared/style_calibration_protocol.md`
- `academic-paper/agents/intake_agent.md`
- `academic-paper/agents/draft_writer_agent.md`
- `deep-research/agents/report_compiler_agent.md`

## `submission-check`
- `academic-paper/agents/formatter_agent.md`
- `academic-paper/references/journal_submission_guide.md`
- `academic-paper/references/credit_authorship_guide.md`
- `academic-paper/references/funding_statement_guide.md`
- reporting-guideline routing from `deep-research/references/equator_reporting_guidelines.md`
