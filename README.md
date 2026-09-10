# IDB30102 - Research Methodology
## A Comparative Framework for Data Anonymization Techniques in Big Data Systems

---

### 📌 Course & Project Information
* **Course Code:** IDB30102
* **Course Name:** Research Methodology
* **Project Title:** A Comparative Framework for Data Anonymization Techniques in Big Data Systems
* **Group Name / ID:** GROUP AK
* **Assigned Research Area:** Data Privacy, Big Data Security & Privacy-Preserving Data Mining (PPDM)

---

### 👥 Group Members
| Name | Student ID | Role / Contribution |
| :--- | :---: | :--- |
| **Muhammad Aidil Mukhriz Bin Khairol Afandi** | 52215226072 | Literature Review & Framework Design |
| **Nurul Nadia Binti Khairuddin** | 52215226154 | Methodology & Architecture Diagram |
| **Nadiah Izzati Binti Noor Aziddin** | 52215226024 | Data Preparation & System Evaluation |
| **Haiqal Imanshah Bin Hazmad Balkish** | 52215125083 | Source Code Implementation & Documentation |

---

### 📖 Project Overview

#### **Research Problem**
Modern big data systems process vast amounts of sensitive personal data under strict privacy regulations such as GDPR and PDPA. While data anonymization is essential to prevent user identification, traditional anonymization techniques often cause severe data distortion, severely degrading data utility for machine learning and analytical tasks. Organizations face a critical trade-off between maximizing privacy protection and retaining data usefulness.

#### **Research Aim**
To design, implement, and benchmark a comprehensive comparative framework evaluating traditional and modern privacy-preserving anonymization techniques to determine the optimal trade-off between privacy protection, data utility, and computational efficiency in big data environments.

#### **Research Objectives**
1. **RO1:** To investigate and categorize existing data anonymization paradigms ($k$-Anonymity, Differential Privacy, and Federated Anonymization) through a systematic literature review.
2. **RO2:** To design and implement a standardized Python-based evaluation framework that applies anonymization techniques to tabular datasets.
3. **RO3:** To benchmark and quantitatively evaluate the privacy preservation level, data utility retention, execution performance, and re-identification risk across all candidate algorithms.

#### **Proposed Solution**
The proposed solution is a Python-driven modular benchmark framework that ingests raw tabular datasets and processes them through three anonymization engines:
* **$k$-Anonymity ($k=3$):** Applies quasi-identifier suppression and age-range generalization.
* **Differential Privacy ($\epsilon=1.0$):** Injects calibrated Laplace noise into numerical attributes.
* **Federated Anonymization:** Simulates local edge-node noise addition prior to global aggregation.

---

### 🔬 Methodology & System Architecture

#### **Research Methodology & Development Model**
This research adopts the **CRISP-DM (Cross-Industry Standard Process for Data Mining)** process model, consisting of 6 phases: Business/Research Understanding, Data Understanding, Data Preparation, Modeling (Anonymization Engine), Evaluation, and Deployment/Documentation.

#### **Proposed System Architecture**
1. **Data Ingestion Module:** Loads raw input CSV datasets (e.g., adult census data).
2. **Pre-processing Engine:** Separates Direct Identifiers, Quasi-Identifiers (QIs), and Sensitive Attributes.
3. **Anonymization Execution Pipeline:**
   * Branch A: $k$-Anonymity Pipeline (Generalization & Suppression)
   * Branch B: Differential Privacy Pipeline (Laplace Noise Addition)
   * Branch C: Federated Local Anonymization Pipeline (Distributed Noise Injection)
4. **Evaluation & Metrics Module:** Computes Data Utility, Re-Identification Risk, and Execution Time.
5. **Output Generator:** Exports benchmarked results to summary tables and log outputs.

---

### 🧪 Proposed Evaluation Plan

* **Baseline:** Raw / Unanonymized Dataset (100% Utility, High Re-Identification Risk).
* **Dataset / Test Environment:** 
  * *Dataset:* Sample Census/Adult Tabular Dataset (`adult_sample.csv`).
  * *Environment:* Python 3.8+ on Windows/Linux local runtime.
* **Evaluation Metrics:**
  * **Data Utility (Accuracy):** Measured via mean absolute error (MAE) and accuracy retention rate (%).
  * **Privacy Guarantee:** Formal mathematical guarantees ($\epsilon$-Differential Privacy, $k$-Indistinguishability).
  * **Re-Identification Risk (%):** Percentage of unique records vulnerable to linkage attacks.
  * **Computational Overhead:** Algorithm execution time measured in seconds (s).

---

### 💻 Tools & Technical Stack

* **Programming Language:** Python 3.8+
* **Libraries & Frameworks:** `pandas`, `numpy`, `math`, `time`
* **Datasets:** `adult_sample.csv` (Tabular Demographic Data)
* **Development Environment:** VS Code / Jupyter Notebook / Git & GitHub

---

### 📂 Repository Structure & Technical Components

```text
IDB30102_GROUP_AK_ResearchTopic/
│
├── README.md                           # Comprehensive project overview and instructions
├── 01_Research_Papers/                 # Indexed list and DOIs of primary literature
├── 02_Literature_Review/               # Synthesis matrix & literature review documentation
├── 03_Architecture_and_Flowchart/      # System architecture & CRISP-DM flowcharts
├── 04_Source_Code/                     # Python implementation of anonymization algorithms
├── 05_Data_or_Sample_Input/            # Raw and sample datasets (e.g., adult_sample.csv)
├── 06_Results_or_Expected_Output/      # Benchmarking logs, metric tables & execution outputs
└── 07_References/                      # Full reference list formatted in APA 7th Edition
```

### 🛠️ Key Framework & Anonymization Methods
* **$k$-Anonymity ($k=3$):** Suppresses sensitive identifiers (e.g., Age ranges, Zip Code grouping) to ensure each record is indistinguishable from at least $k-1$ other records.
* **Differential Privacy ($\epsilon=1.0$):** Adds calibrated Laplace noise to numerical attributes (e.g., Income/Age) providing mathematical privacy guarantees against adversary inference.
* **Federated Anonymization:** Simulates decentralized privacy mechanisms through distributed noise addition prior to global aggregation.

---

### 🚀 Getting Started & Running the Code

#### **Prerequisites**
Make sure you have Python 3.8+ installed along with the required libraries:
```bash
pip install pandas numpy
```
#### **Execution**
Navigate to the 04_Source_Code/ directory and run the main anonymization engine:
```bash
python main_anonymizer.py
```

---

### **📊 Summary of Results**
Preliminary benchmarking on the sample input dataset yielded the following performance metrics:

| **Technique** | **Data Utility (Accuracy)** | **Privacy Level** | **Re-ID Risk (%)** | **Execution Time** |
| :--- | :---: | :--- | :---: | :--- |
| k-Anonymity ($k=3$) | Moderate (~33.3%) | Medium | High (~33.3%) | Very Fast (< 0.01s) |
| Differential Privacy ($\epsilon=1.0$) | Low-Moderate | High | Low (~10.0%) | Fast (< 0.01s) |
| Federated Anonymization | Moderate | High | Medium (~20.0%) | Moderate (~0.01s) |

---

### **📜 Acknowledgments & Citation**
This project is submitted in partial fulfillment of the requirements for IDB30102 Research Methodology.
