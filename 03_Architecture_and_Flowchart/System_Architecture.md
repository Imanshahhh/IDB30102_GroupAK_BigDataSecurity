# System Architecture #

The proposed system starts with the UCI Adult Census Income dataset as the main input.

The dataset is processed using the custom Python implementation `anonymization_framework.py`. Three privacy-preserving techniques are applied:

- k-Anonymity Anonymization
- Differential Privacy
- Federated-learning-inspired Anonymization

Each technique produces a processed dataset and evaluation results.

The results are compared based on:

- Privacy protection
- Data utility
- Re-identification risk
- Execution time
- Computational performance
- Scalability

The final output is a comparative framework showing the differences between the three techniques.

## System Architecture Diagram

**Figure 3.1. System Architecture Diagram**

<img width="1029" height="1156" alt="System Architecture Diagram" src="https://github.com/user-attachments/assets/1c7b8ae5-b8ac-4562-b9db-eeb0e9860534" />
