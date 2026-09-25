---
name: revision
description: "Handle reviewer-driven revision with modes for coaching, response-letter drafting, rebuttal auditing, and verification, while constraining edits to authorized scope and guarding against revision-induced claim, number, citation, and evidence drift."
---

# revision

## Purpose

Merge the upstream revision coach, revision mode, rebuttal audit, re-review, patch-scoped revision, and claim-drift safeguards into one standalone revision skill.

## Modes

- `coach`: parse comments and build a revision roadmap without automatically rewriting the manuscript
- `rebuttal`: draft a point-by-point response after the author has chosen how to respond
- `rebuttal-audit`: audit an existing response letter against reviewer comments
- `verify`: compare comments, response letter, and revised manuscript to verify completion

Read the matching file in `references/` before performing a mode.

## Shared principles

- Account for every reviewer concern.
- Split multipart comments into separate obligations.
- Do not automatically agree with reviewers.
- Distinguish `agree`, `partly agree`, and `disagree with justification`.
- Avoid scope creep unrelated to the review.
- When claiming a change was made, point to where it appears.
- Treat unchanged sections as protected unless a revision requires a dependency fix.

## Scoped revision protocol

Before editing, define a revision patch list:
- reviewer or author concern
- target section or paragraph
- intended change
- evidence or source needed
- downstream sections that may require consistency updates
- surfaces that should remain untouched

Apply changes to the smallest sufficient scope. If a local edit requires a broader conceptual change, surface that dependency before silently rewriting unrelated material.

## Claim-drift guard

During revision, compare pre-edit and post-edit wording for substantive claims.

Watch for silent movement along a claim-strength ladder such as:
- compatible with
- associated with
- predicts
- contributes to
- affects or leads to
- causes

Do not strengthen or weaken a claim without an explicit reviewer concern, author decision, or evidence change that justifies the move. A weakening can be as consequential as a strengthening if it changes the paper's contribution.

## Numeric and citation conservation

For every touched block, check whether the revision unintentionally changes or drops:
- numbers
- signs or directions
- confidence intervals or p-values
- sample sizes
- dates
- table or figure references
- citation keys
- quotation marks
- qualifiers such as not, only, may, or except

Any changed token that affects meaning should be traceable to a revision decision.

## Output

Depending on mode, produce:
- revision roadmap
- point-by-point response
- patch plan or changed-text blocks
- verification matrix
- unresolved issues
- claim-drift warnings
- numeric or citation conservation warnings

When revising prose, provide a concise change log explaining what changed and why.

## General guardrails

- Do not claim a reviewer concern is resolved merely because text was changed.
- Do not introduce new evidence, citations, analyses, or claims without a traceable source or author instruction.
- Do not rewrite untouched material for style during a tightly scoped reviewer revision unless the user asks for broader editing.
