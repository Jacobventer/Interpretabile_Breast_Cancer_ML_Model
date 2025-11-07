# Interpretable Breast Cancer Prediction Model

This repository contains the implementation of a transparent and interpretable machine learning model designed to predict whether a breast tumour is benign (B) or malignant (M) based on diagnostic features from the UCI Breast Cancer Wisconsin Dataset.

The project was completed as part of the Model Engineering  module for the BSc Data Science degree program.

---

## Project Overview
- **Objective:** Develop an interpretable, high-performing classification model for breast cancer detection.  
- **Goal:** Achieve F1-score ≥ 0.95 and provide feature-level interpretability to support oncologist decision-making.  
- **Methodology:** Follows the **CRISP-DM** process (Business Understanding → Data Understanding → Preparation → Modeling → Evaluation → Deployment).  

---

## CRISP-DM Framework

This project followed the CRISP-DM (Cross Industry Standard Process for Data Mining) methodology:
1. Business Understanding: Define project goals and success criteria
2. Data Understanding: Load and explore data for patterns and bias
3. Data Preparation: Clean, encode, and scale features
4. Modeling: Train and compare six ML algorithms
5. Evaluation: Assess accuracy, precision, recall, F1, and ROC-AUC
6. Deployment: Save optimized model and propose a GUI for clinical use

---

## Repository Structure
```bash
breast-cancer-ml-interpretability/
│
├── data/
│   ├── raw/                
│   ├── processed/          
│   └── external/           
│
├── notebooks/
│   ├── 01_EDAv3.ipynb        
│   └── 02_Model_Trainingv2.ipynb  
│
├── src/
│   ├── data_preprocessing.py   
│   ├── model_training.py       
│   └── visualization.py        
│
├── models/
│   ├── saved_model/           
│   └── model_results/          
│
├── reports/
│   ├── figures/                
│   └── final_report.pdf        
│
├── requirements.txt
└── README.md

```

<p align="center">
  <img src="report/figures/Class_distribution_of_benign_and_malignant_diagnoses.png" alt="ROC Curve" width="500"/>
</p>


## EDA graphs
# Diagnosis Distribution
![ROC Curve](report/figures/Class_distribution_of_benign_and_malignant_diagnoses.png)

# Hist & KDE
![ROC Curve](report/figures/Feuture_distribution.png)

# Boxplots
![ROC Curve](report/figures/boxplots_outlier_detection.png)

# Pair plots
![ROC Curve](report/figures/pairwise_relationship_Top4_features.png)
![ROC Curve](report/figures/feature_relationships_scatter_radius_mean.png)

# Correlation Heatmap
![ROC Curve](report/figures/Feature_correlation_heatmap.png)

# Model Results
![ROC Curve](report/figures/6_Models_results.png)
![ROC Curve](report/figures/test_results.png)

# Top 10 Import features
![ROC Curve](report/figures/Top10_important_features.png)


## Detailed Error analysis
# Confusion Matrix
![ROC Curve](report/figures/confusion_matrix_logreg.png)

# ROC AUC
![ROC Curve](report/figures/roc_curve_logreg.png)

# FP & FN distribution
![ROC Curve](report/figures/error_analysis_combined.png)


---

## Model Interpretability
The Logistic Regression coefficients were used to rank feature importance.
The top predictive features included:
- radius_se
- texture_worst
- concavity_worst
- area_worst

These correspond to known medical indicators of tumour irregularity and malignancy, reinforcing the model’s reliability and transparency.

---

## License

This repository is released for educational and academic purposes only.
It must not be used for clinical or diagnostic decision-making.

