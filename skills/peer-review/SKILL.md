---
name: peer-review
description: "Run evidence-anchored academic peer-review lenses for journal fit, methodology, domain knowledge, argument quality, cross-disciplinary perspective, and adversarial challenge, with full, quick, guided, and bounded calibration modes."
---

# peer-review

## Purpose

Preserve the upstream multi-perspective reviewer concept without agent orchestration, ranking papers, or pretending to have editorial authority.

## Modes

- `full`: run several independent lenses and then synthesize
- `quick`: rapid triage focused on the highest-consequence issues
- `guided`: reveal issues progressively through Socratic dialogue so the author reasons through revisions
- `methodology`: methodological soundness
- `domain`: literature, theory, disciplinary accuracy, contribution
- `argument`: internal logic, claim-evidence reasoning, coherence
- `perspective`: adjacent-discipline, stakeholder, practical, or interpretive blind spots
- `adversarial`: strongest counterarguments and vulnerabilities
- `calibration`: evaluate the reviewer process against a user-adjudicated gold set under strict leakage boundaries

## Reviewer configuration

Infer the primary discipline, paper type, methodological orientation, and manuscript maturity from the manuscript. Use these only to choose relevant criteria and perspective. Do not invent a target journal or pretend to be an actual reviewer.

When a severity judgment depends on a field-specific norm, ground the norm in an applicable external standard or label the grounding as uncertain. Do not use model memory alone to turn a preference into a major flaw.

## Independence rule for full review

When the environment supports separate review contexts, conduct the major lenses independently before synthesis. When all lenses run in one context, do not claim statistical or cognitive independence. Preserve lens separation by evaluating the manuscript afresh under each criterion.

## Core review questions

### Journal fit and contribution
- Is the problem significant for the intended audience?
- Is the contribution stated at a defensible level?
- Are title, abstract, introduction, and conclusion aligned?

### Domain
- Does the literature cover the major relevant conversations?
- Are theories represented accurately?
- Are important counterpositions missing?
- Is the contribution incremental, corrective, synthetic, or otherwise well characterized?

### Methodology
Use `methodology-review` logic for design, sampling, measurement, analysis, validity, robustness, and inference limits.

### Argument
- Are the central claims clear?
- Does each key claim follow from evidence and reasoning?
- Are counterarguments handled fairly?
- Are introduction, results, discussion, and conclusion consistent?

### Perspective
- What would an adjacent discipline notice?
- Which stakeholder or practical perspective is absent?
- Are broader implications claimed without support?

### Adversarial
Use `argument-stress-test` logic and preserve unresolved objections.

## Quick mode

Perform a bounded triage rather than a compressed full review. Focus on:
- one or two genuine strengths
- the three to five issues most likely to affect interpretability, validity, contribution, or readiness for deeper review
- whether a methodology review, fact check, or journal-fit check should follow

State that lower-priority issues were not exhaustively reviewed.

## Guided mode

Start with genuine strengths when present. Introduce one issue or tightly related cluster at a time.

For each issue:
1. point the author to the relevant manuscript passage
2. ask a question that helps them diagnose the problem
3. test the proposed fix against the criterion
4. reveal deeper concerns only after the author has engaged the earlier one

Do not make the author guess an arbitrary hidden answer. The goal is understanding and decision quality, not a puzzle.

## Calibration mode

Read `references/calibration.md` before using this mode.

Calibration never creates a universal quality score or acceptance probability. It measures a bounded decision-error profile only when gold labels are isolated from the review process until judgments are frozen.

If the environment cannot isolate the gold labels from the review context, produce a calibration design and clearly state that a valid measured profile cannot be claimed from that run.

## Output

For each review lens:
- scope of review
- genuine strengths
- critical issues
- major issues
- minor issues
- questions for authors
- concrete revision suggestions
- evidence anchors to manuscript locations

For `full` mode add a synthesis that distinguishes consensus, unique findings, and genuine reviewer disagreement.

Do not issue an acceptance or rejection prediction. If the user wants a simulated editorial decision letter, label it explicitly as a simulation and keep it criterion-bound rather than predictive.

## General guardrails

- Do not invent sources, data, reviewer comments, or venue rules.
- Confidence labels are not calibrated probabilities unless a valid bounded calibration protocol has actually been completed.
- Review severity must track consequence and evidence, not reviewer tone.
