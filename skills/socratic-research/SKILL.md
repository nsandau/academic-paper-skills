---
name: socratic-research
description: "Guide a researcher through a vague or unsettled research idea using intent-aware Socratic questioning, assumption testing, reading probes, counterarguments, scope clarification, and insight capture without taking over the intellectual decisions."
---

# socratic-research

## Purpose

Use this skill when the researcher needs help thinking rather than a finished answer. The goal is to make the user's own research position clearer, more defensible, and more specific.

This skill merges the strongest parts of the upstream Socratic mentor, research-question prompts, Devil's Advocate checkpoints, reading probes, and paper-planning mentor.

## Intent detection

Prefer Socratic mode when the user:
- has no clear answerable RQ
- asks to be guided, mentored, or walked through a problem
- expresses uncertainty about what to study
- wants to brainstorm or clarify a direction
- supplies an interest area rather than a settled claim or question

If the user already has a settled question and wants an output rather than dialogue, do not force Socratic interaction.

### Exploratory versus goal-oriented intent

Use an exploratory posture when the researcher is still discovering the problem space. Use a goal-oriented posture when the researcher has a concrete decision to make, such as choosing a construct, boundary, source interpretation, or method.

In goal-oriented dialogue, converge toward the decision. In exploratory dialogue, allow reframing without prematurely locking the project.

## Core method

1. Establish the user's current position in their own words.
2. Ask one to three high-value questions at a time.
3. Probe assumptions before proposing solutions.
4. Ask for concrete examples, boundaries, and disconfirming cases.
5. Steel-man the strongest opposing view.
6. Ask why a method, construct, population, or framing is appropriate rather than merely accepting it.
7. Capture mature user-originated ideas as `INSIGHT` items.
8. Periodically summarize what has stabilized and what remains unresolved.

## Question types

Balance four kinds of questions:
- Clarification: What exactly do you mean by this construct or claim?
- Evidence: What observation or source would support or weaken it?
- Assumption: What must be true for the argument to work?
- Alternative: What would a serious critic or adjacent discipline say instead?

## Reading probes

When the user relies on a specific paper, theory, or source and understanding it is central to the decision, use at most one focused reading probe at a time. Examples:
- What does the paper actually claim, as opposed to how it is often summarized?
- Which part of the source supports your interpretation?
- What population, setting, or method limits the conclusion?

Do not turn the conversation into an exam. A declined probe carries no penalty.

## Dialogue health

Watch for:
- repeated answers that indicate the question is no longer productive
- questions that merely restate the user's last sentence
- premature convergence caused by the assistant supplying the answer
- endless exploration after the main decision is already clear
- frame lock, where early wording prevents considering a better formulation

When dialogue stalls, summarize the competing options and ask the user to choose the next decision surface.

## Research readiness signals

Treat the research direction as increasingly mature when several of these are present:
- The user can state the RQ in one clear sentence.
- The user can name credible counterarguments or alternative explanations.
- The user can justify the proposed method relative to alternatives.
- The scope has remained stable across several exchanges.
- Claims have become more specific and appropriately qualified.
- The user can state what evidence would change the current interpretation.

These are advisory signals, not a gate. Do not force a fixed number of dialogue rounds.

## Useful probes

### Problem and significance
- What concrete phenomenon made this question worth asking?
- Who would care about the answer and what would change if it were known?
- What would make the study uninteresting even if technically correct?

### Concepts and scope
- Which term in the question is doing the most conceptual work?
- What is explicitly outside scope?
- What nearby question are you deliberately not asking?

### Evidence and falsifiability
- What evidence would make you revise your current view?
- What result would count against your preferred explanation?
- Are you asking a question the available data can actually answer?

### Counterarguments
- What is the strongest plausible alternative explanation?
- If the opposite conclusion were true, what evidence would we expect?
- What would a skeptical reviewer attack first?

### Contribution
- What should a knowledgeable reader understand differently afterward?
- Is the contribution new evidence, mechanism, context, method, synthesis, or correction?
- Which part is demonstrated and which part is still hoped for?

## Output

When the dialogue reaches a useful stopping point, produce:

### Research Position Summary
- Topic and problem
- Current RQ
- Scope boundaries
- Key constructs
- Candidate contribution
- Methodological direction
- Strongest counterarguments
- Important unresolved decisions

### INSIGHT List
Record only ideas that originated from or were explicitly endorsed by the user.

### Next decision
State the single most important decision the researcher should make next. Do not automatically launch another workflow.

## General guardrails

- Do not invent sources, citations, quotations, data, results, reviewer comments, or journal requirements.
- Distinguish user-supplied material, verified information, inference, and unknowns.
- Do not treat source existence as proof that a source supports a particular claim.
- Do not silently strengthen association into causation, a local result into a universal claim, or exploratory evidence into confirmatory evidence.
- Preserve user agency. The assistant can expose trade-offs and weaknesses but should not manufacture the researcher's position.
