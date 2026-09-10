# Chapter 2: Literature Review #

## Overview

This chapter reviews previous studies related to privacy-preserving techniques used in big data systems. The review is based on recent publications from 2022 to 2026 and focuses on three commonly used approaches:

- Data Anonymization
- Differential Privacy
- Federated Learning

The purpose of this review is to understand how each technique protects sensitive data, what evaluation metrics are commonly used, and the strengths and limitations reported by previous researchers. The findings are later used to support the comparative framework proposed in this research.

---

## Data Anonymization

Data anonymization is one of the earliest techniques for protecting personal information before data is shared or analyzed. Most studies use k-anonymity and its extensions, such as l-diversity and Mondrian k-anonymity, to reduce the risk of re-identification.

Previous research shows that anonymization can preserve useful information while providing an acceptable level of privacy. However, higher levels of anonymization usually increase information loss and may reduce data quality.

Recent work also combines anonymization with synthetic data generation to improve privacy while maintaining better data utility.

---

## Differential Privacy

Differential Privacy (DP) protects sensitive information by adding controlled noise to the dataset or query results. Compared with traditional anonymization, DP generally provides stronger privacy guarantees.

Several studies reported that although DP reduces re-identification risk significantly, the additional noise may decrease model accuracy and overall data utility.

Researchers have also introduced personalized DP methods that protect only selected sensitive attributes, improving utility while maintaining privacy.

---

## Federated Learning

Federated Learning (FL) allows machine learning models to be trained without transferring raw data to a central server. Instead, only model updates are exchanged.

Many recent studies combine FL with additional technologies such as Differential Privacy, encryption, blockchain, or functional encryption to improve security.

Although FL reduces direct data exposure, researchers have identified challenges such as communication overhead, gradient leakage, and handling non-IID datasets.

---

## Comparison of Existing Studies

The reviewed literature shows that each privacy-preserving technique has different strengths and weaknesses.

| Technique | Main Strength | Main Limitation |
|-----------|---------------|-----------------|
| Data Anonymization | Simple implementation and good data utility | Re-identification risk may remain |
| Differential Privacy | Strong mathematical privacy guarantee | Reduced accuracy due to injected noise |
| Federated Learning | Raw data remains on local devices | Higher communication cost and possible gradient leakage |

Most studies evaluate their techniques using benchmark datasets such as the UCI Adult Census Income dataset together with metrics including:

- Classification Accuracy
- Re-identification Risk
- Privacy Budget (ε)
- Information Loss
- Processing Time
- Communication Cost

---

## Research Gap

The literature indicates that privacy protection and data utility must be balanced. Stronger privacy often results in lower model accuracy or higher computational cost.

Another important observation is that many studies evaluate only one technique or a specific hybrid approach. Very few studies compare Data Anonymization, Differential Privacy, and Federated Learning using the same dataset and evaluation criteria.

This research addresses that gap by applying the three techniques to a common benchmark dataset and comparing them using consistent evaluation metrics. The results are intended to provide a clearer understanding of the privacy–utility trade-off and support future decision-making when selecting privacy-preserving techniques.

---
