## Evaluation Plan

The project evaluates k-anonymity and differential privacy using the same UCI Adult Census Income Dataset and consistent evaluation criteria.

### Evaluation Metrics

| Metric | Purpose |
|---|---|
| Classification Accuracy (%) | Measures the data utility retained after applying each privacy-preserving technique |
| Re-identification Risk (%) | Measures the likelihood of individuals being re-identified from the processed data |
| Execution Time (ms) | Measures the processing time required by each technique |

### Baseline

The original, unprotected UCI Adult Census Income Dataset is used as the baseline for comparison.

### Comparison

The results of k-anonymity and differential privacy are compared against the baseline to evaluate their differences in:

- Privacy protection
- Data utility
- Computational performance

The evaluation aims to provide a clear comparison of the strengths and limitations of k-anonymity and differential privacy under the same experimental conditions.
