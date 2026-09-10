# System Architecture #

The system architecture shows the main flow of this research.

The process starts with the UCI Adult Census Income dataset. The original dataset is used as the baseline. The same dataset is then used for the two privacy-preserving techniques:

- k-Anonymity
- Differential Privacy

For k-Anonymity, the dataset is processed using generalization with a `k = 3` configuration. For Differential Privacy, Laplace noise is added using a privacy budget of `ε = 1.0`.

The results from the original dataset, k-Anonymity, and Differential Privacy are then evaluated using:

- Accuracy
- Re-identification Risk
- Execution Time

The results are collected and compared to see the differences between the two techniques.

## System Architecture Diagram

**Figure 3.1. System Architecture Diagram**

<img width="1029" height="1044" alt="System Architecture Diagram" src="https://github.com/user-attachments/assets/bfe23398-8ffd-4863-860e-d7304f7df42f" />
