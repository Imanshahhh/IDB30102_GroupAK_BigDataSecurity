# Literature Review Analysis Table #

This table summarizes the selected studies reviewed in Chapter 2. The studies are compared based on the technique used, dataset, evaluation metrics, and reported results.

| Technique | Study | Dataset | Key Metric(s) | Reported Result | Limitation for Direct Comparison |
|---|---|---|---|---|---|
| k-Anonymity | Anoop et al. (2025) | UCI Adult | Accuracy, re-identification risk | 82.5% accuracy, 4.2% risk | Different experimental configuration |
| Differential Privacy | Anoop et al. (2025) | UCI Adult | Accuracy, re-identification risk | 70.6% accuracy, 0.8% risk | Different privacy mechanism and settings |
| Anonymization + Generative | Shathi et al. (2026) | UCI Adult | NCP, ε | High utility at ε = 1.0 | Uses generative modelling and different metrics |
| Personalized DP | Chen et al. (2025) | Census, graph data | RMSE, ARE | Up to 14× utility improvement | Different datasets and evaluation metrics |

## Main Findings

- The reviewed studies show that k-anonymity and Differential Privacy can both be used to reduce privacy risks, but they affect data utility in different ways.

- Anoop et al. (2025) reported 82.5% accuracy with 4.2% re-identification risk for k-anonymity. For Differential Privacy, the study reported 70.6% accuracy with a lower re-identification risk of 0.8%.

- Other studies also show that different versions of Differential Privacy and anonymization can improve privacy or data utility. However, some approaches may introduce additional processing, communication, or implementation requirements.

- The studies reviewed here are used as supporting literature. They are not directly implemented in this research. The proposed experiment only uses standard k-anonymity and standard Differential Privacy on the UCI Adult Census Income dataset.
