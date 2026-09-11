# Summary of Methods and Algorithms #

The studies reviewed in Chapter 2 use different methods to protect sensitive data. The methods are mainly based on data anonymization and Differential Privacy.

| Technique | Method / Algorithm | Purpose |
|---|---|---|
| k-Anonymity | Generalization | Makes records less distinguishable |
| k-Anonymity | Suppression | Hides or removes some values |
| k-Anonymity | Mondrian k-Anonymity | Improves the basic k-anonymity approach |
| k-Anonymity | l-Diversity | Gives more protection to sensitive values |
| Anonymization + Generative Methods | DP-CTGAN | Generates private synthetic data |
| Differential Privacy | Laplace Noise | Adds noise to protect sensitive information |
| Differential Privacy | Personalized DP | Allows different privacy requirements for different data |
| Differential Privacy | SSDP | Allows users to select which data needs protection |
| Differential Privacy | Random Quantization | Reduces communication data in compressed DP |

## Methods Used in This Research

- This research only implements two methods: k-Anonymity and Differential Privacy.

### k-Anonymity

- Standard k-anonymity is used with generalization and suppression. The aim is to reduce the chance of identifying individuals from the dataset.

### Differential Privacy

- Standard Differential Privacy is used by adding Laplace noise to the data. The privacy budget used in this research is `ε = 1.0`.

- The other methods are only discussed to support the literature review. They are not implemented in the experiment.
