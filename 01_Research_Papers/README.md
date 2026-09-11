# 01 - Key Research Papers & Publications

This directory contains the structured breakdown of primary research articles supporting Chapter 2 (Literature Review) for the comparative study between **k-Anonymity** and **Differential Privacy**.

> 📌 **Note on Copyright Compliance:** Direct PDF distribution for copyrighted articles is restricted due to publisher access policies (e.g., IEEE Xplore paywalls). Official DOI links and direct IEEE Xplore source links are provided for all cited materials alongside extracted research metadata.

---

## 📌 Primary Papers Summary Matrix

### Paper 1: Anoop et al. (2025) - Core Benchmark Reference
* **Paper Title:** Privacy-preserving data mining techniques in big data environments
* **Author(s):** Anoop, M., Michael, G., & RC, J. G.
* **Year:** 2025
* **IEEE / DOI Link:** [DOI: 10.1109/ICSCDS65426.2025.11167481](https://doi.org/10.1109/ICSCDS65426.2025.11167481)

| Item | Details / Information |
| :--- | :--- |
| **Research Problem** | Traditional PPDM techniques lack direct comparative benchmarking under identical dataset and metric conditions. |
| **Method / Technique** | $k$-Anonymity (generalization & suppression) vs. Differential Privacy (Laplace noise addition). |
| **Dataset / Tools** | UCI Adult Census Income Dataset. |
| **Main Findings** | $k$-Anonymity achieved 82.5% accuracy with 4.2% Re-ID risk; Differential Privacy achieved 0.8% Re-ID risk with significant utility loss (70.6% accuracy loss). |
| **Limitation** | Evaluated under static parameters without dynamic runtime performance comparisons. |
| **Relevance to Proposed Research** | Serves as the primary reference baseline for defining comparison metrics (accuracy, Re-ID risk, execution time). |

---

### Paper 2: Shathi et al. (2026) - Anonymization & Hybrid Benchmark
* **Paper Title:** Enhanced privacy for big data: A hybrid approach using K-anonymity, L-diversity, and DP-CTGAN
* **Author(s):** Shathi, A. H., Ahmed, B., Bakchy, S. C., Rahaman, M. S., Zohra, F. T., & Al Hasan, M.
* **Year:** 2026
* **IEEE / DOI Link:** [DOI: 10.1109/ICECTE69292.2026.11429368](https://doi.org/10.1109/ICECTE69292.2026.11429368)

| Item | Details / Information |
| :--- | :--- |
| **Research Problem** | Vulnerability of $k$-Anonymity to homogeneity and background-knowledge attacks in high-dimensional tabular datasets. |
| **Method / Technique** | Mondrian $k$-Anonymity, $l$-Diversity, and DP-CTGAN generative models. |
| **Dataset / Tools** | UCI Adult Census Income Dataset. |
| **Main Findings** | Hybrid DP-CTGAN retained high synthetic data utility at $\epsilon=1.0$ while eliminating homogeneity attack risks. |
| **Limitation** | High computational training overhead and model instability during early training epochs. |
| **Relevance to Proposed Research** | Validates the selection of UCI Adult dataset and establishes the standard privacy budget ($\epsilon=1.0$). |

---

### Paper 3: Chen et al. (2025) - Differential Privacy Trade-offs
* **Paper Title:** Secret specification based personalized privacy-preserving analysis in big data
* **Author(s):** Chen, J., Hu, C., Liu, Z., Xiang, T., Hu, P., & Yu, J.
* **Year:** 2025
* **IEEE / DOI Link:** [DOI: 10.1109/TBDATA.2024.3433433](https://doi.org/10.1109/TBDATA.2024.3433433)

| Item | Details / Information |
| :--- | :--- |
| **Research Problem** | Standard Differential Privacy applies uniform noise across all features, leading to severe utility degradation. |
| **Method / Technique** | Secret Specification Based Differential Privacy (SSDP). |
| **Dataset / Tools** | U.S. Census Dataset and Graph Datasets. |
| **Main Findings** | Selective protection improved query accuracy up to 14x compared to global Laplace noise injection. |
| **Limitation** | Requires prior knowledge of sensitive attributes and fails when sensitive/non-sensitive features are correlated. |
| **Relevance to Proposed Research** | Provides theoretical backing for analyzing utility loss caused by standard Laplace Differential Privacy. |

---

### Paper 4: Aswal et al. (2022) - Big Data Privacy Foundations
* **Paper Title:** An analysis of big data privacy and safety
* **Author(s):** Aswal, U. S., Dumka, A., & Pokhariyal, R.
* **Year:** 2022
* **IEEE / DOI Link:** [DOI: 10.1109/ICFIRTP56122.2022.10059410](https://doi.org/10.1109/ICFIRTP56122.2022.10059410)

| Item | Details / Information |
| :--- | :--- |
| **Research Problem** | Transmission vulnerabilities and re-identification threats in centralized big data processing architectures. |
| **Method / Technique** | Systematic Analysis of Anonymization and Cryptographic Controls. |
| **Dataset / Tools** | Theoretical & Enterprise Big Data Architectural Frameworks. |
| **Main Findings** | Identified $k$-Anonymity and Differential Privacy as core mechanisms required to meet regulatory standards like GDPR. |
| **Limitation** | Lacks quantitative empirical benchmark testing on standard open-source datasets. |
| **Relevance to Proposed Research** | Supports Problem Statement 1 (PS1) regarding centralized big data security risks. |

---

## 📚 Complete Reference List 
For the full reference citations formatted in **APA 7th Edition**, please refer to the main reference directory:
👉 **[07_References/](../07_References/)**
