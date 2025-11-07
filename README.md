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
## EDA
# Diagnosis Distribution


# Hist & KDE



# Boxplots


# Pair plots


# Correlation Heatmap


# Model Results


# ROC AUC
![ROC Curve](reports/figures/ROC_curve.png)







## Results Summary
| Metric   | Score  |
| :------- | :----- |
| Accuracy | 0.9737 |
| F1-Score | 0.9639 |
| ROC-AUC  | 0.996  |

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

