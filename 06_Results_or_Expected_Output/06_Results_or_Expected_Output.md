# 06. Results / Expected Output

## Preliminary Results

| Technique | Accuracy (%) | Uniqueness-Based Risk Indicator (%) | Execution Time (ms) |
|---|---:|---:|---:|
| Baseline (Raw Data) | 84.04 | 0.12 | 0.00 |
| k-Anonymity (k=3) | 84.67 | 0.00 | 18.00 |
| Differential Privacy (ε=1.0) | 80.63 | 36.99 | 15.00 |

### Findings

- **Baseline:** 84.04% accuracy, 0.12% uniqueness-based risk indicator, and 0.00 ms execution time.
- **k-Anonymity:** 84.67% accuracy, 0.00% uniqueness-based risk indicator, and 18.00 ms execution time.
- **Differential Privacy:** 80.63% accuracy, 36.99% uniqueness-based risk indicator, and 15.00 ms execution time.

The preliminary results indicate that k-anonymity achieved the highest classification accuracy and the lowest measured uniqueness-based risk indicator, while differential privacy provided a different privacy–utility trade-off.

> **Note:** The uniqueness-based risk indicator is an empirical measure based on singleton equivalence classes using the selected quasi-identifiers. It is not a formal measurement of the privacy guarantee provided by Differential Privacy.

## Expected Output

The final study is expected to provide:

1. A comparative evaluation of **k-anonymity** and **Differential Privacy**.
2. Experimental results using the **UCI Adult Census Income dataset**.
3. Comparison based on:
   - Classification accuracy
   - Uniqueness-based risk indicator
   - Execution time
4. Analysis of the **privacy–utility trade-off** between both techniques.
5. A custom Python implementation supporting the comparative evaluation.
6. A final analysis that identifies the practical differences between k-anonymity and Differential Privacy.
