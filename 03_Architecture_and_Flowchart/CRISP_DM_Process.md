# CRISP-DM Process

This research uses CRISP-DM to organize the steps of the study. There are six phases used in this research.

## 1. Business Understanding

The first phase focuses on the research problem. In this study, the problem is the lack of a direct comparison between k-Anonymity and Differential Privacy.

The comparison uses three main criteria:

- Accuracy
- Uniqueness-Based Risk Indicator
- Execution Time

## 2. Data Understanding

This phase focuses on the UCI Adult Census Income dataset. The dataset is studied to understand its attributes and identify the attributes needed for the privacy comparison.

## 3. Data Preparation

The dataset is prepared before applying the two privacy-preserving techniques.

- For k-Anonymity, generalization and suppression are applied using a `k = 3` configuration.
- For Differential Privacy, Laplace noise is added using `ε = 1.0`.

## 4. Modelling

- k-Anonymity and Differential Privacy are applied separately to the same dataset.
- Each technique produces a processed version of the dataset for comparison.

## 5. Evaluation

The processed datasets are evaluated against the original, unprotected dataset.

The main evaluation metrics are:

- Classification Accuracy
- Uniqueness-Based Risk Indicator
- Execution Time

## 6. Deployment

The final results are organised and presented as a comparative evaluation of k-Anonymity and Differential Privacy.

The findings are documented in the research report and supported by the group's GitHub repository.

## CRISP-DM Process Flowchart

**Figure 3.2 CRISP-DM Process Flowchart**

<img width="525" height="618" alt="image" src="https://github.com/user-attachments/assets/9bb9de0d-d4ef-43f4-a043-28b68fe26bd1" />

