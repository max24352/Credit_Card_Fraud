
#  Credit Card Fraud Detection – ML Project

This project builds a fraud detection model using logistic regression on a highly imbalanced credit card transaction dataset. It demonstrates end-to-end ML techniques, including class imbalance handling, model tuning, and explainability — key for real-world fraud and risk systems. Data gained from https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

---

##  Project Summary

- **Data**: Anonymised credit card transactions (~0.17% fraud rate)
- **Goal**: Prioritise recall while improving real-world precision
- **Techniques**: 
  - SMOTE for oversampling
  - Logistic Regression with class weights
  - Threshold tuning (F1-based)
  - SHAP for model interpretability
  - Stratified 5-fold cross-validation

---

##  Model Performance

| Metric        | Baseline Model | Tuned Model |
|---------------|----------------|-------------|
| ROC AUC       | 0.9808         | 0.9808      |
| PR AUC        | 0.7466         | 0.7466      |
| Precision     | 6.2%           | 60.3%       |
| Recall        | 90.5%          | 79.1%       |
| F1 Score      | 11.7%          | 68.4%       |

---

##  Cross-Validation

| Metric        | Mean ± Std     |
|---------------|----------------|
| ROC AUC       | 0.9620 ± 0.0131 |
| PR AUC        | 0.7402 ± 0.0329 |

 Results consistent across folds, confirming robustness.

---

##  Interpretability

- Top features: `V14`, `V17`, `V12` (via SHAP)
- Visual explanations support model transparency

---

##  Highlights

- End-to-end classification pipeline
- Tackles class imbalance, threshold tuning, and explainability
- Strong baseline for fraud detection or other rare event problems

