---
title: "Machine learning triage for glioma histological grading using a minimal mutation and age panel"
collection: publications
type: "Manuscript Under Review"
permalink: /publication/2026-glioma-histological-grading-triage
excerpt: "A leakage-free nested cross-validation audit demonstrating that early-available age and IDH1 status capture over 98% of discriminative capacity in glioma triage, challenging the utility of costly multi-gene sequencing panels."
date: 2026-10-12
venue: "Medical Oncology / Bioinformatics Journal (Revision 2)"
paperurl: "https://github.com/SandeepSinghNk/Glioma-Classification-v2"
citation: "Sandeep Singh, Ashok Pal, Nitin Mittal, Jatinder Kaur, Fikreselam Gared. (2026)."
---

**Authors:** Sandeep Singh, Ashok Pal, Nitin Mittal, Jatinder Kaur, Fikreselam Gared

### Abstract
Distinguishing lower-grade glioma (LGG) from glioblastoma (GBM) shapes treatment urgency, but definitive molecular grading is slow and infrastructure dependent, and published machine learning approaches often apply oversampling before the train/test split, evaluate on AUC alone, deploy at an unexamined 0.5 threshold, and report internally inconsistent tables. We address all four using the UCI Glioma Grading Clinical and Mutation Features Dataset (20 somatic mutation markers, 3 clinical variables; $n=839$ after clinical provenance auditing), classifying the legacy histological LGG-versus-GBM label.

Four imbalance-handling strategies were compared on the training partition only; four classifier families were compared under nested cross-validation, locking Logistic Regression as primary by a pre-specified nested-CV rule. On an untouched test set evaluated once, the locked model achieved:
* **ROC-AUC:** 0.931 (95% CI: 0.893–0.963)
* **Operating Point:** $\tau = 0.487$ (Selected via Youden's $J$)
* **Sensitivity:** 0.871
* **Specificity:** 0.837

A four-feature panel (`IDH1`, `age`, `TP53`, `PTEN`), selected via a leakage-free nested procedure, retained over 99% of full-model test-set discrimination. Improvement over an age-plus-IDH1 baseline was modest ($\Delta$ AUC = +0.020, $p=0.049$). These findings demonstrate that early-available clinical and immunohistochemical signals provide reliable initial triage when extensive sequencing panels are pending or unavailable.

### Resources & Links
* **Source Code Repository:** [GitHub - SandeepSinghNk/Glioma-Classification-v2](https://github.com/SandeepSinghNk/Glioma-Classification-v2)
* **Methodology Highlights:** Fold-safe SMOTE, Nested Cross-Validation, Sealed Holdout Test Set, Decision Curve Analysis (DCA), SHAP TreeExplainer.
