# Evaluation Plan #

This research compares the original UCI Adult dataset with k-Anonymity and Differential Privacy.

## Evaluation Metrics

Three metrics are used in the experiment:

- Classification Accuracy (%)
- Uniqueness-Based Risk Indicator (%)
- Execution Time (ms)

These metrics are used to compare the results of the three cases.

## Baseline

- The original UCI Adult dataset is used as the baseline. No privacy technique is applied to the baseline dataset.

- The results from Anoop et al. (2025) are only used as a reference for the results.

## Test Setup

- The UCI Adult Census Income dataset is processed locally using the custom Python script `anonymization_framework.py`.

- The two techniques tested are:

- k-Anonymity (`k = 3`)
- Differential Privacy (`ε = 1.0`)

## Preliminary Results

| Technique / Treatment | Accuracy (%) | Uniqueness-Based Risk Indicator (%) | Execution Time (ms) |
|---|---:|---:|---:|
| Baseline (Raw Data) | 84.04% | 0.12% | 0.00 ms |
| k-Anonymity (`k = 3`) | 84.67% | 0.00% | 18.00 ms |
| Differential Privacy (`ε = 1.0`) | 80.63% | 36.99% | 15.00 ms |

## Observation

- The raw dataset gives 84.04% accuracy. k-Anonymity gives a slightly higher accuracy of 84.67%, while Differential Privacy gives 80.63%.

- For the uniqueness-based risk indicator, the raw dataset gives 0.12%. k-Anonymity gives 0.00%, while Differential Privacy gives 36.99%.

- For execution time, k-Anonymity takes 18.00 ms and Differential Privacy takes 15.00 ms.

## Note

- The uniqueness-based risk indicator is only used as a measure in this experiment. It is not a formal privacy guarantee.

## Success Condition

- The evaluation is considered successful when the results show clear differences between k-Anonymity and Differential Privacy based on accuracy, risk indicator, and execution time.
