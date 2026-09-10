# IDB30102 - Research Methodology
## A Comparative Framework for Privacy-Preserving Techniques in Big Data Systems

### 📌 Course & Project Information
* **Course Code:** IDB30102
* **Course Name:** Research Methodology
* **Project Title:** A Comparative Framework for Data Anonymization Techniques in Big Data Systems
* **Group Name** / ID:GROUP AK

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
Data privacy has become a critical concern in modern big data systems driven by stringent regulations such as GDPR and PDPA. While data anonymization is essential for preserving privacy, traditional techniques often degrade data utility, limiting their applicability for analytical tasks. 

This research introduces a comparative framework evaluating three prominent anonymization paradigms:
1. **$k$-Anonymity** (Generalization & Suppression)
2. **Differential Privacy** (Laplace Noise Injection)
3. **Federated Learning-Inspired Anonymization** (Local Noise Aggregation)

The framework evaluates these techniques across four key dimensions: **Data Utility**, **Privacy Guarantee**, **Computational Overhead**, and **Re-Identification Risk**.

---

### 📂 Repository Structure
```text
IDB30102_GroupX_ResearchTopic/
│
├── README.md                          
├── 01_Research_Papers/               
├── 02_Literature_Review/             
├── 03_Architecture_and_Flowchart/    
├── 04_Source_Code/                   
├── 05_Data_or_Sample_Input/          
├── 06_Results_or_Expected_Output/    
└── 07_References/
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
