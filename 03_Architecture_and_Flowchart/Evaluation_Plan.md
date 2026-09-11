## Evaluation Plan

The project evaluates k-Anonymity and Differential Privacy using the same UCI Adult Census Income Dataset and consistent evaluation criteria.

### Evaluation Metrics

| **Metric** | **Purpose** |
|---|---|
| Classification Accuracy (%) | Measures the data utility retained after applying each privacy-preserving technique. |
| Uniqueness-Based Risk Indicator (%) | Measures the proportion of records belonging to singleton equivalence classes based on the selected quasi-identifiers. |
| Execution Time (ms) | Measures the processing time required by each technique. |

### Baseline

The original, unprotected UCI Adult Census Income Dataset is used as the baseline for comparison.

### Comparison

The results of k-Anonymity and Differential Privacy are compared against the baseline to evaluate their differences in:

- Privacy-related uniqueness
- Data utility
- Computational performance

The evaluation aims to provide a consistent comparison of the strengths and limitations of k-Anonymity and Differential Privacy under the same experimental conditions.
