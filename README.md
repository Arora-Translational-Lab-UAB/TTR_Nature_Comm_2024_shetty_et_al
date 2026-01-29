# Determinants of TTR Levels and Clinical Outcomes (UK Biobank)

This repository contains the analysis pipeline and code for the study: **"Determinants of transthyretin levels and their association with adverse clinical outcomes among UK Biobank participants"** (Published in *Nature Communications*, 2024).

## 📌 Project Overview
Transthyretin (TTR) is a transport protein synthesized in the liver. Dissociation and misfolding of TTR lead to cardiac amyloidosis. This study leverages the **UK Biobank (UKB)** to identify clinical correlates of TTR levels and assess how these levels—and specific genetic variants—predict cardiovascular risk.

### Key Research Questions:
1. What clinical and demographic factors determine circulating TTR levels?
2. How does the **V142I TTR** genetic variant influence TTR concentration?
3. Are lower TTR levels associated with incident heart failure and mortality?

---

## 📊 Key Findings

| Category | Findings |
| :--- | :--- |
| **Demographics** | TTR levels are significantly **lower in females** compared to males. |
| **Clinical Correlates** | **Positive associations:** BMI, SBP/DBP, Total Cholesterol, Albumin, Creatinine. <br> **Negative association:** C-reactive protein (CRP). |
| **Genetics** | Carriers of the **V142I variant** (common in individuals of African ancestry) have significantly lower circulating TTR levels. |
| **Outcomes** | Lower TTR levels are linked to a higher risk of **Heart Failure (HF)**, cardiovascular mortality, and all-cause mortality. |

---

## 🛠 Analysis Pipeline
The code in this repository is organized into the following stages:

1.  **Data Cleaning:** Filtering UK Biobank participants (n ≈ 35,000) and handling missingness.
2.  **Cross-sectional Analysis:** Linear regression models to identify clinical determinants of TTR.
3.  **Genetic Association:** Assessing the impact of the V142I variant on TTR concentration.
4.  **Survival Analysis:** Cox Proportional Hazards models to calculate HRs for heart failure and mortality.

---

## 🚀 Getting Started

### Prerequisites
* **R version:** 4.x, SAS
* **Required Libraries:** `survival`, `tidyverse`, `genetics`, `ggplot2`

### Usage
To replicate the main analysis:
1. Ensure you have access to the UK Biobank dataset (Application ID required).
2. Run `01_data_preprocessing.R` to generate the cohort.
3. Run `02_ttr_determinants.R` for the cross-sectional correlates.
4. Run `03_survival_models.R` for the clinical outcome analysis.

---

## 📖 Citation
If you use this code or findings in your research, please cite:
> *Arora, P., et al. (2024). Determinants of transthyretin levels and their association with adverse clinical outcomes among UK Biobank participants. Nature Communications.*

**Contact:** [Your Lab/Office Email]
