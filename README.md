# Transposable Elements Identifier using Novel Statistical Moments Descriptors and Machine Learning Approach
# Overview
Transposable elements (TEs), often known as jumping genes, are DNA sequences capable of moving within genomes and generating multiple dispersed copies of themselves. Accurate identification and classification of TEs are critical for understanding their biological roles and evolutionary impacts.
This repository contains the dataset, feature extraction scripts, and machine learning models developed in our study for the classification of transposable elements (TEs). The project introduces a machine learning–driven pipeline (CTE-ML) based on a 4-step rule, designed to assist experimental scientists in achieving reliable and interpretable classification results.
Key Features
## Comprehensive Dataset
A benchmark dataset of 98,042 samples (49,042 positive and 49,000 negative) was used to classify TEs into their respective orders and superfamilies.
## Feature Extraction
Statistical moment–based, position-based, and composition-related features were computed to generate feature vectors for downstream analysis.
## Machine Learning Models
Four models were trained and evaluated:
Random Forest (RF)
XGBoost (XGB)
LightGBM (LGBM)
Decision Tree (DT)
## Evaluation Protocols
Self-Consistency Testing
Independent Set Testing
Cross-Validation Testing
These were applied rigorously to ensure robustness and generalization of results.
## Results Summary
The XGBoost (CTE-XGB) model achieved the most consistent and accurate results across all experiments.
Accuracy up to 96.81% (Independent Testing)
MCC up to 0.96 (Cross-Validation)
Perfect 100% Sensitivity and Specificity in some self-consistency experiments
These outcomes demonstrate that the combination of the proposed feature extraction technique and XGB classifier effectively captures hidden patterns within the genomic data, enabling precise classification of TEs.
