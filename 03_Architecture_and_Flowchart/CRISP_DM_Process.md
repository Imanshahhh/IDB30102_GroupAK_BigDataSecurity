# CRISP-DM Process #

This research uses CRISP-DM to organize the research process. The methodology has six phases.

## 1. Business Understanding

This phase is about understanding the research problem. In this study, the main problem is the lack of a direct comparison between k-Anonymity and Differential Privacy.

The comparison uses three main metrics:

- Accuracy
- Re-identification Risk
- Execution Time

## 2. Data Understanding

This phase focuses on the UCI Adult Census Income dataset. The dataset is checked to understand its attributes and identify the attributes that are related to privacy.

## 3. Data Preparation

The dataset is prepared before applying the privacy techniques.

For k-Anonymity, generalization is used with `k = 3`. For Differential Privacy, Laplace noise is added using `ε = 1.0`.

## 4. Modelling

In this phase, k-Anonymity and Differential Privacy are applied separately to the same dataset.

The two methods are used as separate approaches so their results can be compared.

## 5. Evaluation

The results from both techniques are compared with the original dataset.

The comparison is based on:

- Accuracy
- Re-identification Risk
- Execution Time

The results are also compared with the findings from previous studies.

## 6. Deployment

The final results are organised into the comparative evaluation. The findings are used to show the differences between k-Anonymity and Differential Privacy.

## CRISP-DM Flow

The research follows this order:

**Business Understanding → Data Understanding → Data Preparation → Modelling → Evaluation → Deployment**

If the results are not suitable, the data preparation stage can be reviewed and the process can be repeated.
