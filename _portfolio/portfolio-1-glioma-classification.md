---
title: "Clinical ML Triage & Cost-Matrix Threshold Optimization: Glioma Histological Grading"
excerpt: "Leakage-free nested cross-validation, SHAP explainability, and clinical cost-matrix threshold optimization ($\tau^* = 0.200$, 97.1% GBM sensitivity) on the UCI/TCGA Glioma Dataset ($n=839$).<br/><img src='https://img.shields.io/badge/Python-3.10+-blue.svg'> <img src='https://img.shields.io/badge/Springer-svjour3-green.svg'> <img src='https://img.shields.io/badge/ROC--AUC-0.931-brightgreen.svg'>"
collection: portfolio
---

## Project Overview
An end-to-end, methodologically audited machine learning diagnostic pipeline classifying Low-Grade Glioma (LGG) vs. Glioblastoma Multiforme (GBM) using 20 somatic mutation markers and 3 clinical variables from the UCI/TCGA cohort ($n=839$ patients).

### Key Methodological & Clinical Innovations
* **Leakage-Free Training Partitioning:** Implemented SMOTE strictly within training folds to prevent data leakage; tuned Logistic Regression, Random Forest, SVM, and XGBoost alongside Voting and Stacking ensembles.
* **Rigorous Multi-Metric Evaluation:** Achieved **ROC-AUC = 0.931** (95% CI: 0.893–0.963) on sealed holdout evaluation under locked nested cross-validation, and **ROC-AUC = 0.926**, **MCC = 0.738**, **Brier = 0.102** across ten benchmark metrics.
* **SHAP Biological Alignment:** Confirmed `IDH1` ($\bar{\phi} = 0.207$) and `Age` as dominant predictors via SHAP TreeExplainer, with a parsimonious 4-feature panel (`IDH1`, `Age`, `TP53`, `PTEN`) retaining over 99% of discriminative capacity in alignment with WHO 2021 CNS classification.
* **Clinical Cost-Matrix Threshold Optimization:** Designed an asymmetric cost-matrix framework ($C_{\text{FN}} = 10, C_{\text{FP}} = 2$) shifting the deployment threshold from $0.5$ to $\tau^* = 0.200$, achieving **97.1% GBM sensitivity** and a **24% reduction in total clinical cost**.

### Repository & Manuscript
* **Source Code:** [SandeepSinghNk/Glioma-Classification-v2](https://github.com/SandeepSinghNk/Glioma-Classification-v2)
* **Manuscript:** 15-page peer-reviewed paper (73 citations, Springer `svjour3` format).
