# Interpretable Breast Cancer Prediction Model

This repository contains the implementation of a transparent and interpretable machine learning model designed to predict whether a breast tumour is benign (B) or malignant (M) based on diagnostic features from the UCI Breast Cancer Wisconsin Dataset.

The project was completed as part of the Model Engineering  module for the BSc Data Science degree program.

---

## Project Overview
- **Objective:** Develop an interpretable, high-performing classification model for breast cancer detection.  
- **Goal:** Achieve F1-score ≥ 0.95 and provide feature-level interpretability to support oncologist decision-making.  
- **Methodology:** Follows the **CRISP-DM** process (Business Understanding → Data Understanding → Preparation → Modeling → Evaluation → Deployment).  

---

## Repository Structure
```bash
breast-cancer-ml-interpretability/
│
├── data/
│   ├── raw/                # Original dataset (not uploaded)
│   ├── processed/          # Cleaned & encoded data for model input
│   └── external/           # Placeholder for external datasets
│
├── notebooks/
│   ├── 01_EDA.ipynb        # Exploratory Data Analysis
│   └── 02_Model_Training.ipynb  # Model training, tuning, evaluation
│
├── src/
│   ├── data_preprocessing.py   # Cleaning, encoding, scaling
│   ├── model_training.py       # Model training & optimization pipeline
│   └── visualization.py        # All plots & charts
│
├── models/
│   ├── saved_models/           # logistic_regression_final_20251106.joblib
│   └── model_results/          # final_model_result_metrics.csv
│
├── reports/
│   ├── figures/                # All generated plots
│   └── final_report.pdf        # Final written report
│
├── requirements.txt
└── README.md

```
| Metric   | Score  |
| :------- | :----- |
| Accuracy | 0.9737 |
| F1-Score | 0.9639 |
| ROC-AUC  | 0.996  |



