# Evaluation Plan #

This research compares three cases using the UCI Adult Census Income dataset:

- Raw Dataset
- k-Anonymity
- Differential Privacy

## What is Measured

Three measurements are used:

- Classification Accuracy (%)
- Uniqueness-Based Risk Indicator (%)
- Execution Time (ms)

These measurements are used to see how the two privacy techniques perform compared with the raw dataset.

## Baseline

- The original UCI Adult dataset is used as the baseline. No privacy technique is applied to the baseline dataset.

- The results from Anoop et al. (2025) are only used as a reference from the previous study.

## Test Setup

The dataset is processed locally using the custom Python script `anonymization_framework.py`.

The settings used in the test are:

- k-Anonymity (`k = 3`)
- Differential Privacy (`ε = 1.0`)

## Preliminary Results

| Technique / Treatment | Accuracy (%) | Uniqueness-Based Risk Indicator (%) | Execution Time (ms) |
|---|---:|---:|---:|
| Baseline (Raw Data) | 84.04% | 0.12% | 0.00 ms |
| k-Anonymity (`k = 3`) | 84.67% | 0.00% | 18.00 ms |
| Differential Privacy (`ε = 1.0`) | 80.63% | 36.99% | 15.00 ms |

## Observation

- The raw dataset has 84.04% accuracy. k-Anonymity gives 84.67%, while Differential Privacy gives 80.63%.

- For the risk indicator, the raw dataset gives 0.12%. k-Anonymity gives 0.00%, while Differential Privacy gives 36.99%.

- For execution time, k-Anonymity takes 18.00 ms and Differential Privacy takes 15.00 ms.

- The results show that both techniques give different results when they are applied to the same dataset.

## Note

The uniqueness-based risk indicator is used only for this experiment. It is not a formal privacy guarantee.

## Success Condition

The evaluation is successful when the results show clear differences between the raw dataset, k-Anonymity, and Differential Privacy based on accuracy, risk indicator, and execution time.
