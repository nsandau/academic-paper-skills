# Peer-review calibration

Use this mode only when the user has an adjudicated comparison set and wants to measure the reviewer process, not when they merely want a review.

## Epistemic boundary

Ordinary review is `NOT_CALIBRATED`.

A measured result applies only to the tested domain, article type, venue criteria or rubric, review mode, and execution setup. It must not be generalized to unrelated papers or treated as an acceptance probability.

## Gold-label isolation

The adjudicated verdicts and rationales must be hidden from the reviewing process until each review judgment is frozen. If they have already been exposed to the reviewer context, the run is contaminated and cannot support a valid error profile.

## Tiers

### Directional
Use exactly three adjudicated manuscripts spanning the Minor versus Major boundary and one more extreme case. Run one bounded review per manuscript. Report only raw agreement direction such as lenient, exact, or harsh. Do not report FNR, FPR, stability, or calibration claims.

### Full
Prefer 5 to 20 adjudicated manuscripts, ideally with examples on both sides of a predefined decision boundary. Repeated runs can help characterize variability only if the execution contexts are appropriately separated. Do not call repeated runs independent merely because they are separate calls.

For a binary boundary defined in advance, report:
- false-negative rate for acceptable-side papers judged on the reject side
- false-positive rate for reject-side papers judged on the acceptable side
- balanced accuracy
- exact categorical agreement
- uncertainty intervals where the sample permits them

Do not report AUC unless there is a genuine continuous score, and do not manufacture one from categorical review labels.

## Dimension-level judgments

Where human gold annotations exist for a criterion, report categorical agreement counts. If there is no gold annotation for a dimension, report `NOT COMPUTABLE` rather than inferring correctness.

## Severity grounding

Separately track findings whose claimed severity depends on an external field norm. Mark grounding risk high when a major judgment depends on an unverified norm.

## Output warning

Every measured result must state that it is target-set local and does not establish universal calibration, reviewer independence, or publication outcome probability.
