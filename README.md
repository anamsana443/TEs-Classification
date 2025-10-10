# Transposable Elements Identifier using Novel Statistical Moments Descriptors and Machine Learning Approach
# Overview
Transposable elements (TEs), often known as jumping genes, are DNA sequences capable of moving within genomes and generating multiple dispersed copies of themselves. Accurate identification and classification of TEs are critical for understanding their biological roles and evolutionary impacts.
This repository contains the dataset, feature extraction scripts, and machine learning models developed in our study for the classification of transposable elements (TEs). The project introduces a machine learning–driven pipeline (CTE-ML) based on a 4-step rule, designed to assist experimental scientists in achieving reliable and interpretable classification results.
# Key Features 
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
## Repository Structure 
├── Code/                    # Google Colab notebooks
│   ├── TE_Non_TE_Classification.ipynb
│   ├── TE Orders Classification.ipynb
│   └── TE Superfamilies Classification .ipynb
|    ├── Feature Space Visualization UMAP.ipynb              # 
├── Dataset/                  # Fasta sequence
│   ├── DNA Transposons
│   ├── Retro Transposons 
└── Feature Vectors/   
    ├── Dataset1.csv
    ├── Dataset2.csv
    └── Dataset3.csv

# 🔧 Basic Usage Steps

#### Step 1: Data Preparation

· Access clean, non-redundant FASTA sequences from the Dataset/ folder
· Sequences are already processed using CD-HIT to remove redundancy
· Data is organized by classification level (Order/Superfamily)

#### Step 2: Model Training & Evaluation

1. Open the Colab notebooks in Code/ folder
2. Load feature vectors from Feature Vectors Folder
3. Choose evaluation protocol:
   · Self-Consistency Testing
   · Independent Set Testing
   · Cross-Validation Testing

#### Step 3: Run Classification

· Four models available: RF, XGB, LGBM, DT
· XGBoost (CTE-XGB) recommended as best performer
· Follow the 4-step rule pipeline for interpretable results

## 🚀 Quick Start

For immediate results:

1. Use pre-computed feature vectors from Feature_Vector/
2. Run .ipynb notebooks on Google Colab with default settings
3. Select XGBoost model for optimal performance (96.81% accuracy)

## 📊 Expected Results

· Accuracy: Up to 96.81% (Independent Testing)
· MCC: Up to 0.96 (Cross-Validation)
· Sensitivity/Specificity: Up to 100% in self-consistency tests

This pipeline enables researchers to reliably classify transposable elements using the novel statistical moments approach combined with machine learning.
