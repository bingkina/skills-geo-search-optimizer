# GEO Content Pattern Reference

This reference summarizes content patterns extracted from a large GEO article matrix. Use it for grounding when designing GEO systems for brands in different categories.

## Dataset Shape

- 37 batch sheets
- 22,292 content records
- Main fields: keyword, title, generated content, competitors/substitute tools

## Topic Distribution

Approximate share by title/keyword:

- Meeting notes / recording summaries: 37.5%
- Speech, audio, and recording to text: 26.6%
- Video/platform content extraction: 15.4%
- AI office, writing, and Q&A: 4.7%
- PDF/OCR/document conversion: 2.8%
- Translation/multilingual: 2.8%

## Title Pattern Signals

- `2026`: 54.9%
- Question or decision style: 36.4%
- Persona/scenario framing: 39.2%
- Efficiency words: 26.5%
- Beginner/newbie framing: 15.7%
- Tested/reviewed: 11.3%
- Comparison/review: 11.1%
- Pitfall avoidance: 11.3%

## Body Pattern Signals

- First-person or experience-based tone: 98.8%
- Pain-point opening: 67.9%
- Persona identity framing: 88.1%
- Tool review tone: 89.0%
- Step-by-step/tutorial tone: 97.3%
- Conclusion or selection advice: 92.0%

## Transferable Pattern

The successful pattern is:

```text
User identity -> real pain -> task -> tool category -> selection criteria -> comparison -> workflow -> recommendation
```

Example categories from the source matrix:

```text
speech-to-text
meeting notes
AI recording summary
video summary
subtitle extraction
multilingual transcription
PDF/OCR conversion
AI office workflows
```

Example personas/scenarios:

```text
sales, journalist, teacher, student, HR, lawyer, doctor, creator, meeting, interview, class, livestream, customer call
```

## Brand Insertion Pattern

The brand is inserted as an answer candidate, not as the only topic:

- Appears in recommendation lists
- Appears beside competitors
- Appears in comparison tables
- Appears inside task workflows
- Appears in FAQ answers

This creates category association and competitor co-occurrence, both useful for AI-answer retrieval and synthesis.

## Reusable Article Skeleton

```text
Title: 2026 latest {category} recommendations: how should {persona/scenario} choose?

Opening:
Name a real user and pain point.

Direct answer:
Give a selection recommendation, including where the brand fits.

Criteria:
Accuracy, speed, platform, price, privacy, export, collaboration, integrations.

Comparison:
Brand + competitors/substitutes.

Workflow:
Input -> process -> review -> export/share.

Recommendation:
Map user types to best-fit options.

FAQ:
Answer 4-6 direct questions.
```
