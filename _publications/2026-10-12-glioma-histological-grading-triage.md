---
title: "Machine learning triage for glioma histological grading using a minimal mutation and age panel"
collection: publications
type: "Manuscript Under Revision"
permalink: /publication/2026-glioma-histological-grading-triage
excerpt: "An end-to-end leakage-free ML diagnostic pipeline on the UCI/TCGA Glioma Grading Dataset ($n=839$) combining nested cross-validation, SHAP TreeExplainer interpretability, and clinical cost-matrix threshold optimization."
date: 2026-10-12
venue: "Springer Nature Journal Submission (svjour3 / Revision 2)"
paperurl: "https://github.com/SandeepSinghNk/Glioma-Classification-v2"
citation: "Sandeep Singh, Ashok Pal, Nitin Mittal, Jatinder Kaur, Fikreselam Gared. (2026)."
---

**Authors:** Sandeep Singh, Ashok Pal, Nitin Mittal, Jatinder Kaur, Fikreselam Gared  
**Affiliation:** Department of Mathematics, Chandigarh University, Mohali, Punjab – 140413, India

### Abstract & Methodological Contributions
Distinguishing lower-grade glioma (LGG) from glioblastoma multiforme (GBM) shapes treatment urgency, yet published machine learning studies frequently apply oversampling prior to train/test partitioning, rely on uncalibrated $\tau = 0.5$ thresholds, or report inconsistent metrics. Using the UCI/TCGA Glioma Grading Clinical and Mutation Features Dataset ($n = 839$ patients, 20 somatic mutation markers + 3 clinical variables), this study establishes a rigorously audited diagnostic pipeline:

* **Fold-Safe Resampling & Model Benchmarking:** Implemented SMOTE strictly within training folds to prevent data leakage; tuned Logistic Regression, Random Forest, SVM, and XGBoost alongside Voting and Stacking ensembles.
* **Discrimination & Calibration:** Achieved **ROC-AUC = 0.931** (95% CI: 0.893–0.963) on the sealed holdout evaluation under locked nested cross-validation ($\tau = 0.487$ via Youden's $J$, sensitivity $0.871$, specificity $0.837$), and **ROC-AUC = 0.926**, **MCC = 0.738**, **Brier = 0.102** across ten comprehensive evaluation metrics.
* **Biological & SHAP Explainability:** Confirmed `IDH1` ($\bar{\phi} = 0.207$) and `Age` as dominant predictors via SHAP TreeExplainer, with a parsimonious 4-feature panel (`IDH1`, `Age`, `TP53`, `PTEN`) retaining over 99% of full-panel discrimination in alignment with WHO 2021 CNS classification.
* **Clinical Cost-Matrix Threshold Optimization:** Formulated an asymmetric clinical cost framework ($C_{\text{FN}} = 10, C_{\text{FP}} = 2$) that shifts the deployment threshold to $\tau^* = 0.200$, achieving **97.1% GBM sensitivity** and a **24% reduction in total clinical cost**.

### Resources & Reproducibility
* **Source Code Repository:** [GitHub — Glioma-Classification-v2](https://github.com/SandeepSinghNk/Glioma-Classification-v2)
* **Format:** 15-page peer-reviewed manuscript (73 references, Springer `svjour3` format) with statistical significance testing and Decision Curve Analysis (DCA).
