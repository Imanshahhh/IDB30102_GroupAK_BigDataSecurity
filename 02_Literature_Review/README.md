# Chapter 2: Literature Review

## Overview

This chapter reviews previous studies related to privacy-preserving techniques used in big data systems. The review is based on recent publications from 2022 to 2026 and focuses on two commonly studied privacy-preserving techniques:

- k-Anonymity
- Differential Privacy

The reviewed studies were analyzed based on their approaches, benchmark datasets, evaluation metrics, and reported findings. These analyses support the comparative evaluation conducted in this research.

## Folder Contents

- Literature Review Analysis Table
- Comparison of Existing Techniques
- Research Gap Analysis
- Summary of Methods and Algorithms
- Relevant Datasets
- Evaluation Metrics
- References Supporting the Proposed Methodology

The purpose of this review is to understand how k-anonymity and differential privacy protect sensitive data, what evaluation metrics are commonly used, and the strengths and limitations reported by previous researchers. The findings are used to support the comparative evaluation proposed in this research.

---

## k-Anonymity

k-Anonymity is a privacy-preserving technique that reduces the risk of re-identification by ensuring that each individual record is indistinguishable from at least `k - 1` other records based on selected quasi-identifiers.

Previous research shows that k-anonymity can preserve useful information while providing a practical level of privacy protection. However, stronger anonymization may result in greater information loss and reduced data utility.

Several studies have also proposed extensions such as l-diversity and Mondrian k-anonymity to address limitations of basic k-anonymity, including homogeneity and background-knowledge attacks.

For this research, only standard k-anonymity is implemented using generalization and suppression.

---

## Differential Privacy

Differential Privacy (DP) protects sensitive information by adding controlled statistical noise to data or query results. It provides a formal mathematical privacy guarantee controlled by a privacy budget, commonly represented by `ε`.

Previous studies indicate that DP can provide strong privacy protection and reduce the risk of information disclosure. However, increasing privacy protection may introduce more noise, which can reduce classification accuracy and overall data utility.

Researchers have also proposed variations such as personalized differential privacy to improve utility by applying different privacy requirements to selected data attributes.

For this research, standard differential privacy is implemented using Laplace noise injection with a privacy budget of `ε = 1.0`.

---

## Comparison of Existing Studies

The reviewed literature shows that k-anonymity and differential privacy have different strengths and limitations.

| **Technique** | **Main Strength** | **Main Limitation** |
|---|---|---|
| k-Anonymity | Simple and practical privacy-preserving approach | Re-identification risk may remain |
| Differential Privacy | Provides a formal mathematical privacy guarantee | Added noise may reduce data utility and accuracy |

Studies commonly evaluate these techniques using benchmark datasets and metrics such as:

- Classification Accuracy
- Re-identification Risk
- Information Loss
- Privacy Budget (`ε`)
- Processing Time

The UCI Adult Census Income dataset is particularly relevant because it has been used in previous studies evaluating both k-anonymity and differential privacy.

---

## Research Gap

The literature indicates that privacy protection and data utility involve an important trade-off. Stronger privacy protection can result in lower accuracy, greater information loss, or increased computational requirements.

Another important observation is that many studies evaluate k-anonymity or differential privacy independently, while comparative studies often use different experimental settings, datasets, or evaluation metrics. This makes direct comparison difficult.

This research addresses this gap by applying **k-anonymity and differential privacy to the same UCI Adult Census Income dataset** and evaluating both techniques using consistent criteria:

- Classification Accuracy
- Re-identification Risk
- Execution Time

