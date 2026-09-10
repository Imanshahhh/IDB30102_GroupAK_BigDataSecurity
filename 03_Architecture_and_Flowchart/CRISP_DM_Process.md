# CRISP-DM Process

The research follows six phases of the CRISP-DM methodology.

## 1. Security Understanding

The research problem and comparison criteria are defined. The study focuses on comparing anonymization, differential privacy, and federated learning.

## 2. Data Understanding

The UCI Adult Census Income dataset is studied to understand its attributes, quasi-identifiers, and sensitive attributes.

## 3. Data Preparation

The dataset is prepared using the custom Python implementation `anonymization_framework.py`.

The implementation applies:

- k-Anonymity
- Differential Privacy
- Federated-learning-inspired anonymization

## 4. Modelling

Each privacy-preserving technique is applied separately to the dataset based on the selected configurations.

## 5. Evaluation

The results are compared using classification accuracy, privacy level, re-identification risk, and execution time.

## 6. Deployment

The final results are organised into a comparative framework and documented in the research report and GitHub repository.

## Process Flowchart

**Figure 3.2. CRISP-DM Process Flowchart**

<img width="1024" height="1245" alt="CRISP_DM Process Flowchart" src="https://github.com/user-attachments/assets/6c7c3bd7-2718-413e-95eb-f671eebbcd43" />
