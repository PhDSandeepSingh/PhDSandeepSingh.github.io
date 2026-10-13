---
title: "Clinical ML Triage: Glioma Histological Grading"
excerpt: "Leakage-free nested cross-validation and minimal mutation panel selection for brain tumor triage.<br/><img src='https://img.shields.io/badge/Python-3.10+-blue.svg'> <img src='https://img.shields.io/badge/Status-Revision_2-green.svg'>"
collection: portfolio
---

## Project Overview
This project presents an end-to-end, methodologically audited machine learning pipeline for classifying histological grades (LGG vs. GBM) using somatic mutation markers and clinical variables from the TCGA cohort ($n=839$).

### Key Methodological Innovations
* **Prevention of Data Leakage:** Preprocessing, imputation, and synthetic oversampling (SMOTE) are strictly confined to training folds inside nested cross-validation loops.
* **Pre-Specified Model Locking:** Evaluated logistic regression, random forests, support vector machines, and XGBoost; locked Logistic Regression by pre-specified cross-validation criteria.
* **Sealed Holdout Evaluation:** Touched once at the final stage, yielding an AUC of **0.931** (95% CI: 0.893–0.963).
* **Parsimonious 4-Feature Panel:** Selected `IDH1`, `Age`, `TP53`, and `PTEN`—retaining over 99% of discriminative capacity compared to the full 23-variable panel.
* **Decision Curve Analysis (DCA):** Quantified clinical net benefit across practical threshold probabilities.

### Repository & Reproducibility
* **Source Code:** [SandeepSinghNk/Glioma-Classification-v2](https://github.com/SandeepSinghNk/Glioma-Classification-v2)
* **Colab Notebook:** Self-contained training and inference notebooks with locked seeds and reproducible environment manifests.
