# Plasma mNGS and Antimicrobial Stewardship in Critically Ill Patients

This repository contains the analysis code, statistical workflows, and figure-generation scripts associated with the manuscript evaluating plasma metagenomic next-generation sequencing (mNGS), blood cultures, biomarker kinetics, antimicrobial stewardship decisions, and clinical outcomes in critically ill patients.

## Study Overview

The study evaluates paired plasma mNGS and blood-culture sampling episodes in an ICU cohort, with particular focus on:

* Microbiological findings from mNGS and blood cultures
* Baseline antibiotic exposure
* Longitudinal biomarker kinetics
* Antimicrobial treatment adaptations
* Hospital and ICU mortality
* Survival outcomes
* Sequential multivariable modeling across predefined clinical phases

The analyses are observational and exploratory.

---

## Statistical Analyses

The repository includes code for:

* Descriptive statistics and group comparisons
* Standardized mean differences
* Sequential multivariable logistic regression
* Firth penalized logistic regression
* Biomarker kinetics and change-from-baseline analyses
* Receiver operating characteristic (ROC) analysis
* Kaplan–Meier survival analysis
* Cox proportional-hazards regression
* Stewardship-decision modeling
* Manuscript tables and figures

The sequential regression framework follows the predefined study phases:

* **Phase A:** admission/baseline variables
* **Phase B:** early biomarker kinetics and blood-culture information
* **Phase C:** later clinical information including mNGS results

Absolute biomarker values and changes from baseline are analyzed separately.

---

## Repository Structure

```text
├── scripts/
├── figures/
├── results/
├── supplementary/
├── manuscript/
└── README.md
```

---

## Reproducibility

The analysis scripts document cohort definitions, variable transformations, model specifications, statistical procedures, and generation of manuscript figures and tables.

Missing data are handled by complete-case analysis within the respective models unless otherwise specified. No imputation is performed.

Because the underlying dataset contains protected clinical information, patient-level data are not publicly distributed through this repository.

---

## Software

Analyses were performed in **R version 4.5.3**.

Principal packages include:

* tidyverse
* pROC
* survival
* survminer
* logistf

Additional packages used for data handling, visualization, and export are specified within the individual scripts.

---

## AI-Assisted Code Development

OpenAI tools were used selectively for code debugging, syntax refinement, code organization.

All cohort definitions, analytical decisions, variable definitions, model specifications, statistical interpretations, and final results were reviewed and verified by the authors. AI tools were not used to generate or modify the underlying clinical study data.

---

## Research Status

This repository accompanies an observational clinical research manuscript. The analyses are exploratory and should not be interpreted as a prospectively validated clinical decision-support system.

---

## Disclaimer

The code and analytical workflows are provided for research and reproducibility purposes only. They are not intended to replace clinical judgment or serve as a validated medical decision-support tool.
