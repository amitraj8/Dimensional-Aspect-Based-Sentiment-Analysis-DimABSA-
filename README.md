# Dimensional Aspect-Based Sentiment Analysis (DimABSA) – SemEval 2026

This repository contains the implementation, experiments, and thesis-related work for the **SemEval-2026 Task 3: Dimensional Aspect-Based Sentiment Analysis (DimABSA)**.

The project focuses on predicting fine-grained emotional representations using the **Valence-Arousal (VA)** framework instead of traditional categorical sentiment labels such as positive, negative, and neutral.

The work covers:

- **Subtask 1:** Dimensional Aspect Sentiment Regression (DimASR)
- **Subtask 2:** Dimensional Aspect Sentiment Triplet Extraction (DimASTE)
- **Subtask 3:** Dimensional Aspect Sentiment Quadruplet Extraction (DimASQP)

---

# Task Description

## Subtask 1 – Dimensional Aspect Sentiment Regression (DimASR)

Given:
- A sentence
- One or more aspect terms

Predict:
- Valence-Arousal (VA) scores for each aspect.

### Example

### Input
```json
{
  "ID": "R001",
  "Text": "average to good thai food, but terrible delivery.",
  "Aspect": [
    "thai food",
    "delivery"
  ]
}

### Output
{
  "ID": "R001",
  "Aspect_VA": [
    {
      "Aspect": "thai food",
      "VA": "6.75#6.38"
    },
    {
      "Aspect": "delivery",
      "VA": "2.88#6.62"
    }
  ]
}
