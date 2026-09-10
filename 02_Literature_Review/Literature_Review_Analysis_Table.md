# Literature Review Analysis Table #

This table summarizes the selected studies reviewed in Chapter 2. The studies are compared based on the technique used, dataset, evaluation metrics, and reported results.

| Study | Technique | Dataset | Key Metrics | Reported Result |
|---|---|---|---|---|
| Anoop et al. (2025) | k-Anonymity | UCI Adult | Accuracy, Re-identification Risk | 82.5% accuracy and 4.2% re-identification risk |
| Anoop et al. (2025) | Differential Privacy | UCI Adult | Accuracy, Re-identification Risk | 70.6% accuracy and 0.8% re-identification risk |
| Shathi et al. (2026) | Anonymization + Generative Methods | UCI Adult | NCP, Privacy Budget (ε) | High utility at ε = 1.0 |
| Chen et al. (2025) | Personalized Differential Privacy | U.S. Census, Graph Data | RMSE, ARE | Up to 14x utility improvement |
| Alvarez and Kim (2026) | Compressed Differential Privacy | Smart Grid Telemetry | Communication Reduction, Privacy Budget | 73% reduction in communication data with ε ≤ 1.5 |
| Wen and Ye (2025) | Differential Privacy + AES | LLM Data | SIRR, Training Time, Latency | 3.8% sensitive information re-identification rate |
| Zhou and Zhang (2025) | Differential Privacy | Financial Data | Accuracy, Privacy Leakage | 93.1% accuracy and 0.85% privacy leakage |

## Main Findings

The reviewed studies show that k-anonymity and Differential Privacy can both be used to reduce privacy risks, but they affect data utility in different ways.

Anoop et al. (2025) reported 82.5% accuracy with 4.2% re-identification risk for k-anonymity. For Differential Privacy, the study reported 70.6% accuracy with a lower re-identification risk of 0.8%.

Other studies also show that different versions of Differential Privacy and anonymization can improve privacy or data utility. However, some approaches may introduce additional processing, communication, or implementation requirements.

The studies reviewed here are used as supporting literature. They are not directly implemented in this research. The proposed experiment only uses standard k-anonymity and standard Differential Privacy on the UCI Adult Census Income dataset.
