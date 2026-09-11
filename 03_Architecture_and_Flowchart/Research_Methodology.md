# Research Methodology

- This research uses a data-driven approach based on the CRISP-DM methodology.
- The main purpose of this research is to compare k-Anonymity and Differential Privacy using the UCI Adult Census Income dataset.

The research follows six CRISP-DM phases:

1. Business Understanding
2. Data Understanding
3. Data Preparation
4. Modelling
5. Evaluation
6. Deployment

## 1. Business Understanding

- This phase focuses on the research problem and the criteria used to compare k-Anonymity and Differential Privacy.

The main criteria are:

- Classification Accuracy
- Uniqueness-Based Risk Indicator
- Execution Time

## 2. Data Understanding

- The UCI Adult Census Income dataset is studied to understand the data and identify the attributes that are related to the privacy evaluation.
- The dataset is also compared with its use in previous studies.

## 3. Data Preparation

- The dataset is prepared using the custom Python script `anonymization_framework.py`.
- For **k-Anonymity**, generalization and suppression are applied using a `k = 3` configuration:
  - `age` is grouped into 10-year range bins (e.g., 20–29, 30–39).
  - Any equivalence class smaller than `k`, based on `age` and `marital-status` as quasi-identifiers, is suppressed from the dataset.
- For **Differential Privacy**, Laplace noise is added to numeric attributes using a privacy budget of `ε = 1.0`.
- Two processed versions of the dataset are produced for the comparative evaluation, alongside the original unprotected dataset as the baseline.

## 4. Modelling

- k-Anonymity and Differential Privacy are applied separately to the same dataset.
- The configurations used for both techniques are based on the methods discussed in the literature review.

## 5. Evaluation

- The two techniques are compared with the original UCI Adult dataset.

The evaluation uses:

- Classification Accuracy
- Uniqueness-Based Risk Indicator
- Execution Time

The results are also compared with the general direction of the results reported by Anoop et al. (2025).

## 6. Deployment

- The final results are organised into a comparative evaluation.
- The findings are used to show the differences between k-Anonymity and Differential Privacy in terms of privacy-related uniqueness, data utility, and processing time.
