# Telco-Customer-Churn-Classification-Metrics-Analysis
# Classification Metrics Analysis

## Project Overview

This project focuses on evaluating the performance of a Logistic Regression model using different classification metrics. The analysis is performed on the **Telco Customer Churn** dataset to measure the effectiveness of the trained model.

The project demonstrates both manual metric calculations and Scikit-learn implementations to validate the evaluation results.

---

## Dataset

**Dataset:** Telco Customer Churn

Target Variable:

- 0 → No Churn
- 1 → Churn

---

## Project Workflow

### 1. Data Preparation
- Load dataset
- Data cleaning
- Missing value handling
- Label Encoding
- Feature Scaling
- Train-Test Split

### 2. Logistic Regression Prediction
Generated:
- Predicted classes
- Predicted probabilities

### 3. Confusion Matrix
Computed the Confusion Matrix and visualized it using a Seaborn heatmap.

The matrix includes:
- True Positive (TP)
- True Negative (TN)
- False Positive (FP)
- False Negative (FN)

### 4. Manual Metric Calculation
Calculated manually:
- Precision
- Recall
- F1 Score

### 5. Scikit-learn Evaluation
Compared manual calculations with:
- classification_report
- precision_score
- recall_score
- f1_score

### 6. ROC Curve
Generated the Receiver Operating Characteristic (ROC) Curve and evaluated the Area Under the Curve (AUC).

### 7. Threshold Analysis
Compared different classification thresholds:

- Threshold = 0.3
- Threshold = 0.5
- Threshold = 0.7

This comparison illustrates how changing the threshold affects model performance.

---

## Threshold Analysis Summary

Threshold = **0.3** increases Recall because more samples are classified as positive. However, this may reduce Precision due to an increase in false positives.

Threshold = **0.7** increases Precision by making the model more selective when predicting positive cases. However, this may reduce Recall because more positive cases are missed.

Threshold = **0.5** provides a balanced trade-off between Precision and Recall and is commonly used as the default threshold.

The optimal threshold depends on the application. For example, applications that prioritize detecting all positive cases may prefer a lower threshold, while applications requiring fewer false positives may benefit from a higher threshold.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## Evaluation Metrics

- Confusion Matrix
- Precision
- Recall
- F1 Score
- ROC Curve
- AUC Score
- Threshold Analysis

---

## Key Learning Outcomes

- Binary classification evaluation
- Manual metric calculations
- Performance comparison
- ROC analysis
- Threshold optimization
- Model evaluation techniques
