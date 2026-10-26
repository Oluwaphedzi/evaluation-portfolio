# Evaluation Portfolio

**Oluwafeyikemi Dahunsi**
AI Data Evaluator | LLM Response Reviewer | Yoruba, English, Korean & Nigerian Pidgin

Lagos, Nigeria | [Email](mailto:dahunsioluwafeyikemi@gmail.com) | [LinkedIn](https://linkedin.com/in/oluwafeyikemi-dahunsi)

---

## Project Overview

This repository is the hub for my evaluation work. It holds my rubrics, a reusable evaluation template, my review workflow and an anonymization checklist for LLM evaluation in Yoruba, English, Korean and Nigerian Pidgin. It also links to three sample projects that apply them.

> **Sample work:** Everything here was created for this portfolio to demonstrate my method. It contains no client data, names, or proprietary guidelines.

---

## Project Pages

| Project | What it shows |
| --- | --- |
| [Multilingual LLM Evaluation](https://github.com/Oluwaphedzi/multilingual-llm-evaluation) | Four-dimension scoring of responses in Yoruba, English, Korean and Pidgin. |
| [Pidgin and Yoruba Dataset Annotation](https://github.com/Oluwaphedzi/pidgin-yoruba-annotation) | Label schema, rules and fourteen labeled rows. |
| [Search Quality and Prompt Review](https://github.com/Oluwaphedzi/search-quality-prompt-review) | Search result ratings across four intent types and A/B answer comparison. |

---

## Rubrics

### Rubric 1 · Language response quality

Scores of 2 and 4 sit between the anchors below.

| Dimension | 1 | 3 | 5 |
| --- | --- | --- | --- |
| **Fluency** | Meaning-changing errors | Understandable, some unnatural phrasing | Native-like |
| **Cultural accuracy** | Foreign assumptions | Mostly fits, one slip | Fully fits community |
| **Task accuracy** | Wrong or false | Partly correct | Correct and complete |
| **Register fit** | Wrong formality | Mixed | Matches relationship |

**Scoring rules**

- **Overall:** mean of the four scores.
- **Cap rule:** if Cultural or Task accuracy is 2 or below, the overall score is capped at 3.0.
- **One error, one dimension:** score each error under its primary dimension only.
- **Fix rule:** every score of 3 or below gets a written rationale and a suggested fix. A score of 2 or below is flagged as a major issue.

The full rubric, with worked cases, is in [Multilingual LLM Evaluation](https://github.com/Oluwaphedzi/multilingual-llm-evaluation).

### Rubric 2 · Pairwise preference

- **Safety first:** Safety failures decide the comparison first. A harmful answer loses regardless of style, and is rated 1.
- **Accuracy:** Then compare accuracy.
- **Instruction:** Then compare how exactly each answer follows the instruction, including the audience. An answer that fails the instruction is capped at 2.
- **Clarity and tone:** Last, compare clarity and tone.
- **Ties:** If both answers are equal, mark a tie and say what would break it.
- **Justification:** Always write the reason in one or two sentences that point to specific text.

---

## Evaluation Template

Copy this block for each task:

```text
Task ID: EV-0001
Language and domain: yo / etiquette
Prompt and response: [paste here, with names and numbers removed]
Scores: Fluency _ | Cultural _ | Task _ | Register _
Overall: [mean of four; apply the cap rule if Cultural or Task is 2 or below]
Rationale: [two to four sentences quoting the exact words that drove each score]
Suggested fix: [the corrected sentence in the target language]
Flags: none / sensitive / needs second review
```

### Filled example

This is Case 4 from the Multilingual LLM Evaluation project.

```text
Task ID: EV-0004
Language and domain: pcm / slang explanation
Prompt and response: "Explain wetin 'japa' mean for Pidgin, make e simple." + sample response
Scores: Fluency 5 | Cultural 5 | Task 5 | Register 4
Overall: 4.8
Rationale: The meaning of "japa" is correct and the Pidgin is natural. "Furthermore"
is a formal English connector that breaks the spoken feel, so it is scored once, under Register.
Suggested fix: Replace "Furthermore" with "And", or "Even so".
Flags: none
```

---

## My Review Workflow

1. Read the prompt first and decide what a good answer would contain before reading the response.
2. Score each dimension separately, then write the rationale before the overall judgment.
3. Quote the exact words behind every low score.
4. Re-check a sample of my own scores later to catch drift.
5. Escalate anything sensitive, ambiguous, or possibly harmful instead of guessing.

---

## Anonymization Checklist

A checklist for turning real evaluation work into shareable samples.

| Remove or replace | Replace with |
| --- | --- |
| Personal names | Role words such as "the tenant" |
| Phone numbers, emails, addresses | `[removed]` |
| Client or platform names | "the platform" |
| Names of real models or their outputs | "the model" |
| Internal guideline wording | My own paraphrase of the criterion |

---
*Sample portfolio. Rubrics and templates created for demonstration.*
