---
name: style-calibration
description: "Infer a cautious author style profile from the user's own prior academic writing and apply it as a soft guide without overriding disciplinary, venue, clarity, or evidence requirements."
---

# style-calibration

## Purpose

Learn recurring features of the author's academic voice from prior writing samples so later drafting or revision can better match that voice.

This is personalization, not detector evasion. Do not use the skill to make AI-generated text harder to detect or to imitate another identifiable author's style.

## Sample requirements

Prefer at least three samples written substantially by the user. One or two samples can produce only a provisional profile.

Record for each sample:
- language
- discipline or topic
- approximate date
- document type
- whether it was single-authored or co-authored
- which sections are confidently attributable to the user

Prefer recent samples, the same target language, and similar academic genres. If the samples span many years, give more weight to recent work while preserving stable traits.

## Dimensions

### Sentence rhythm
Assess typical sentence length, variability, coordination and subordination patterns, and whether the author alternates concise and complex sentences.

### Paragraph rhythm
Assess typical paragraph size, argumentative density, and section-dependent variation.

### Vocabulary and stance
Identify recurring choices for:
- hedging
- emphasis
- reporting verbs
- transitions
- technical versus general wording
- degree of formality

### Citation integration
Assess patterns such as:
- narrative versus parenthetical citations
- citation density
- where citations typically appear in a paragraph
- how sources are introduced, contrasted, and synthesized

### Modifier and abstraction style
Assess whether prose tends to be lean or highly qualified, concrete or abstract, example-driven or concept-driven.

### Register shifts by section
Note whether Methods, Results, Discussion, and Conclusion use meaningfully different levels of assertiveness, interpretation, or personal voice.

## Profile reliability

Separate:
- stable traits seen across samples
- probable traits
- sample-specific features
- traits that may be imposed by a venue, coauthor, or document type

Do not infer a stable personal preference from a single striking sentence.

## Priority order when applying the profile

1. Accuracy and evidence boundaries
2. Discipline conventions
3. Explicit target-venue requirements
4. Clarity and accessibility
5. Author style profile

If personal style conflicts with a stronger requirement, follow the stronger requirement and note the conflict once when useful.

## Transfer limits

When source samples are in another language, transfer structural traits cautiously. Do not transfer language-specific vocabulary habits.

When samples are co-authored, analyze only sections the user identifies as theirs when possible.

Do not reproduce distinctive phrases merely because they appear repeatedly. Learn patterns, not strings.

## Output

### Style Profile
- Sample basis and reliability
- Sentence rhythm
- Paragraph rhythm
- Vocabulary and stance
- Citation integration
- Modifier and abstraction style
- Register shifts
- Stable traits
- Uncertain traits
- Traits that should not be carried into the target manuscript

### Application Notes
List a short set of practical instructions that `section-writer` or `academic-writing` can use, such as preferred hedging, transition habits, sentence variability, and citation integration.

## Boundaries

- Never claim that the profile proves authorship.
- Never use stylistic similarity as a plagiarism or AI-detection test.
- Do not preserve unclear or incorrect prose merely because it resembles the author's past writing.
