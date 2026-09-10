# Chapter 2: Literature Review #

## Overview

This chapter reviews previous studies on privacy-preserving techniques in big data systems. The review is based on 40 studies published between 2022 and 2026.

The literature is mainly divided into two technique categories:

- k-Anonymity
- Differential Privacy

The studies were reviewed based on the techniques used, datasets, evaluation metrics, and reported results. The review mainly looks at the trade-off between privacy protection and data utility, which is important for the comparison carried out in this research.

## Folder Contents

- Literature Review Analysis Table
- Comparison of Existing Techniques
- Research Gap Analysis
- Summary of Methods and Algorithms
- Relevant Datasets
- Evaluation Metrics
- References Supporting the Proposed Methodology

## k-Anonymity

k-Anonymity is used to reduce the chance of identifying an individual from a dataset. It works by making records less distinguishable based on selected quasi-identifiers.

Previous studies show that k-anonymity is a practical method and can retain useful information in the dataset. However, stronger anonymization may cause information loss and reduce data utility. There may also still be some risk of re-identification.

Other methods such as l-diversity and Mondrian k-anonymity have been studied to improve some limitations of basic k-anonymity. These methods are included in the literature review as supporting studies.

For this research, standard k-anonymity is implemented using generalization and suppression.

## Differential Privacy

Differential Privacy protects sensitive information by adding controlled noise to data or query results. The privacy level is controlled using a privacy budget represented by `ε`.

Previous studies show that differential privacy can provide stronger formal privacy protection. However, more noise can affect data utility and classification accuracy.

Several variations of differential privacy have also been proposed to improve the balance between privacy and utility. These approaches are reviewed as supporting literature.

For this research, standard differential privacy is implemented using Laplace noise with `ε = 1.0`.

## Comparison of Existing Studies

The reviewed studies show that k-anonymity and differential privacy have different strengths and limitations.

| **Technique** | **Main Strength** | **Main Limitation** |
|---|---|---|
| k-Anonymity | Simple and practical for data anonymization | Re-identification risk may still remain |
| Differential Privacy | Provides a formal privacy guarantee | Noise may reduce accuracy and data utility |

Common metrics found in the reviewed studies include:

- Classification Accuracy
- Re-identification Risk
- Information Loss
- Privacy Budget (`ε`)
- Processing Time

The UCI Adult Census Income dataset is especially relevant to this research because it is used in previous studies involving both k-anonymity and differential privacy.

## Research Gap

The literature shows a clear trade-off between privacy protection and data utility. Higher privacy protection may reduce accuracy or increase information loss.

Many studies focus on only one technique, while others use different datasets, experimental conditions, or evaluation metrics. This makes direct comparison between k-anonymity and differential privacy more difficult.

This research addresses the gap by applying **k-anonymity and differential privacy to the same UCI Adult Census Income dataset**. Both techniques are evaluated using the same criteria:

- Classification Accuracy
- Re-identification Risk
- Execution Time

