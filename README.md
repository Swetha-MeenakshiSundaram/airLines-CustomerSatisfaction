# ✈️ Airline Customer Prediction using AdaBoost

## 📌 Project Objective

This project aims to predict customer satisfaction in the airline industry based on various factors such as inflight experience, service quality, and flight-related attributes. The goal is to develop a machine learning model that can classify whether a customer is satisfied (`1`) or not satisfied (`0`) with their flight experience.

---

## 📂 Dataset Overview

- **Source**: CSV file (manually collected or provided)
- **Target Variable**: Customer satisfaction (`0` = Not Satisfied, `1` = Satisfied)
- **Features**: Includes demographic, service, and flight-related attributes

### 🔧 Preprocessing and Feature Engineering

- Handled missing/null values
- Applied label encoding or one-hot encoding where needed
- Standardized numerical features for uniform scaling
- Evaluated feature importance at the end using AdaBoost

---

## 🤖 Model Used: AdaBoost Classifier

- **Base Estimator**: Decision Tree (depth = 1)
- **Number of Estimators**: 100

### ❓ Why AdaBoost?

- Tried traditional classifiers like Decision Tree, Random Forest, and KNN
- Other models either overfitted or gave poor generalization
- AdaBoost gave **significantly better performance** on test data with reduced overfitting

---

## 📊 Evaluation Metrics

- **Training Accuracy**: 92.43%
- **Testing Accuracy**: 92.0%
- **Precision/Recall/F1 Score**: High performance for both satisfied and unsatisfied classes
- **Confusion Matrix**: Visualized using `ConfusionMatrixDisplay` for better interpretability

| Metric         | Class 0 | Class 1 |
|----------------|---------|---------|
| Precision      | 0.93    | 0.92    |
| Recall         | 0.94    | 0.90    |
| F1-score       | 0.93    | 0.91    |

---

## 🔍 Insights

- Balanced and high performance across both classes
- AdaBoost helped mitigate overfitting observed in other models
- Feature importance analysis provided useful insights into key drivers of customer satisfaction

---

## 🚫 Deployment

This model is not intended for deployment at the current stage. The main goal was exploratory modeling and performance benchmarking.

---

## 🚀 Future Improvements

- Hyperparameter tuning with cross-validation
- Try other ensemble models like Gradient Boosting, XGBoost
- Incorporate SHAP/LIME for model explainability
- Explore advanced feature engineering (e.g., interaction terms, PCA)

---
