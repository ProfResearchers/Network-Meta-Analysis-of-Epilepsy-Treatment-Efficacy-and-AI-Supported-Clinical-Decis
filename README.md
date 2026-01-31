***

# Modeling Epilepsy Treatment Efficacy with Network Meta-Analysis & AI
### Development of an AI-Supported Personalized Clinical Decision Support System (CDSS) Prototype

![Support](https://img.shields.io/badge/Support-TÜBİTAK%202209--A-red) ![Status](https://img.shields.io/badge/Status-In%20Progress-blue) ![Language](https://img.shields.io/badge/Language-Python%20%7C%20R-green) ![Domain](https://img.shields.io/badge/Domain-Neurology%20%7C%20AI-purple)

> **Application Number:** 1919B012564493  
> **Program:** TÜBİTAK 2209-A University Students Research Projects Support Program

---

## 📖 Project Overview

This research project aims to develop an **AI-based, evidence-driven Clinical Decision Support System (CDSS) prototype** to assist clinicians in selecting the most appropriate antiepileptic drug (AED) for **focal onset epilepsy**.

Current treatment guidelines often rely on general recommendations, leading to a "trial-and-error" approach in clinical practice. This project bridges the gap between high-level statistical evidence and personalized medicine by combining **Network Meta-Analysis (NMA)** of Randomized Controlled Trials (RCTs) with **Machine Learning (ML)** models.

### 🎯 Key Objectives
1.  **Systematic Review:** Conduct a comprehensive review of RCTs comparing monotherapy AEDs for focal epilepsy.
2.  **Network Meta-Analysis:** Generate quantitative evidence on the relative efficacy (seizure-free rates) and safety (withdrawal rates) of drugs, even those not directly compared in head-to-head trials.
3.  **AI Modeling:** Train a Machine Learning model using the structured NMA data and patient demographics to predict treatment success probabilities.
4.  **Prototype Development:** Build a user-friendly web interface for clinicians to input patient data and receive evidence-based treatment rankings.

---

## 🔬 Scientific Background & Methodology

The project utilizes a hybrid methodology spanning clinical research and medical informatics, divided into three main phases:

### Phase 1: Data Collection & Statistical Analysis
*   **Protocol:** Registration of the review protocol (PICO criteria) in PROSPERO.
*   **Search Strategy:** Systematic search of PubMed, Cochrane CENTRAL, Embase, and Web of Science following **PRISMA** guidelines.
*   **Network Meta-Analysis (NMA):** Using **R** (specifically the `netmeta` package) to synthesize direct and indirect evidence from RCTs.
    *   *Primary Outcome:* Seizure freedom at 6/12 months.
    *   *Secondary Outcome:* Treatment withdrawal due to adverse events.

### Phase 2: Artificial Intelligence (AI) Development
*   **Data Structuring:** Transforming RCT and NMA results into a structured dataset containing patient covariates (age, gender, seizure type, comorbidities).
*   **Model Training:** Developing ML models (e.g., **XGBoost**, **Random Forest**, or **Neural Networks**) using **Python**.
*   **Goal:** To predict the probability of success for specific drugs based on individual patient inputs.

### Phase 3: Software Prototyping
*   **Interface:** Developing a web-based CDSS using **Flask** or **Streamlit**.
*   **Functionality:** The system will accept clinical inputs and output a ranked list of AEDs with their predicted efficacy scores and confidence intervals.

---

## 🗓 Project Roadmap (Timeline)

| Period | Phase | Activities |
| :--- | :--- | :--- |
| **Months 1-2** | Planning | Protocol definition, PICO criteria refinement, and PROSPERO registration. |
| **Months 3-5** | Data Collection | Systematic literature search, study selection (PRISMA), data extraction, and Risk of Bias (RoB 2) assessment. |
| **Months 6-8** | Statistical Analysis | Conducting Network Meta-Analysis (NMA) and creating the structured dataset for AI training. |
| **Months 9-10** | AI Modeling | Machine Learning model selection, training, hyperparameter optimization, and validation. |
| **Months 11-12** | Prototyping | Development of the web-based CDSS interface, integration of the model, and final reporting. |

---

## 🛠 Tech Stack

### Data Analysis & Statistics
*   **R Project:** `netmeta`, `metafor`, `tidyverse`
*   **Tools:** Cochrane Risk of Bias Tool (RoB 2)

### Artificial Intelligence & Engineering
*   **Python:** `Pandas`, `NumPy`, `Scikit-learn`, `XGBoost`
*   **Deep Learning:** `TensorFlow` or `PyTorch` (if applicable)
*   **Web Framework:** `Flask` / `Django` / `Streamlit`

---

## 👥 Project Team

| Role | Name | Institution |
| :--- | :--- | :--- |
| **Project Lead** | **Khaled Jamal Abdelmoeen Hamed** | Ondokuz Mayıs University <br> Faculty of Medicine (4th Year Student) |
| **Academic Advisor** | **Prof. Dr. Murat Terzi** | Ondokuz Mayıs University <br> Dept. of Neurology |

---

## 🚀 Expected Outcomes

1.  **Scientific Publication:** An article published in an SCI/SCI-E indexed journal presenting the updated NMA results.
2.  **Conference Presentation:** Presentation of the methodology and results at a national/international neurology or AI congress.
3.  **CDSS Prototype:** A functional web-based tool for personalized epilepsy management.
4.  **Open Dataset:** A structured, open-access dataset of Epilepsy RCTs for future research.

---

## ⚠️ Disclaimer

This project is supported by **TÜBİTAK (The Scientific and Technological Research Council of Türkiye)** under the 2209-A program.

*   The software and models provided in this repository are for **academic and research purposes only**.
*   They are **not** intended to replace professional medical advice, diagnosis, or treatment.
*   Clinical decisions should always be made by qualified healthcare professionals.

---

## 📞 Contact

For any inquiries, collaboration requests, or issues regarding the code:

*   **Project Lead:** Khaled Hamed
*   **Email:** `cemalhalit03@gmail.com`
*   **GitHub:** [Open an Issue](../../issues)
