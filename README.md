# customer-churn-prediction
End-to-end customer churn prediction using machine learning, class imbalance handling, and SHAP explainability.
# Customer Churn Prediction with Explainable AI

## 📌 Project Overview

Customer churn prediction is a machine learning problem where the goal is to identify customers who are likely to leave a telecom service.

In this project, machine learning models are trained on the Telco Customer Churn dataset to predict customer churn. The project also addresses class imbalance and uses SHAP (SHapley Additive exPlanations) to understand why the model makes its predictions.

## 🎯 Objectives

* Predict whether a customer is likely to churn.
* Handle class imbalance in the target variable.
* Compare multiple machine learning classification models.
* Evaluate models using precision, recall, F1-score and ROC-AUC.
* Explain model predictions using SHAP.
* Generate individual customer churn predictions.

## 🗂️ Dataset

The project uses the Telco Customer Churn dataset containing telecom customer information such as:

* Customer demographics
* Tenure
* Contract type
* Internet services
* Payment method
* Monthly charges
* Total charges
* Churn status

The target variable is:

* `0` → No Churn
* `1` → Churn

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* SHAP
* Joblib
* Google Colab

## 🤖 Machine Learning Models

The following classification models were implemented and compared:

1. Logistic Regression
2. Decision Tree
3. Random Forest

## ⚙️ Machine Learning Workflow

```text
Dataset
   ↓
Data Understanding
   ↓
Data Cleaning
   ↓
Exploratory Data Analysis
   ↓
Train/Test Split
   ↓
Feature Preprocessing
   ↓
Class Imbalance Handling
   ↓
Model Training
   ↓
Model Evaluation
   ↓
Model Comparison
   ↓
Final Model
   ↓
SHAP Explainability
   ↓
Customer Churn Prediction
```

## ⚖️ Class Imbalance

The dataset contains more customers who did not churn than customers who churned.

Because of this imbalance, accuracy alone can be misleading.

The project therefore evaluates the models using:

* Precision
* Recall
* F1-score
* ROC-AUC
* Confusion Matrix

Class weighting was also used during model training to give greater importance to the minority churn class.

## 📊 Model Evaluation

The models were evaluated using multiple classification metrics rather than relying only on accuracy.

The comparison includes:

| Model               |   Accuracy |  Precision |     Recall |   F1 Score |    ROC-AUC |
| ------------------- | ---------: | ---------: | ---------: | ---------: | ---------: |
| Logistic Regression | See output | See output | See output | See output | See output |
| Decision Tree       | See output | See output | See output | See output | See output |
| Random Forest       | See output | See output | See output | See output | See output |

The exact results are available in:

`outputs/model_comparison.csv`

## 🔍 SHAP Explainability

SHAP was used to understand the contribution of individual features to the model's predictions.

SHAP provides two important types of explanations:

### Global Explanation

Identifies features that have a large average contribution across the test dataset.

### Individual Explanation

Shows how individual features contribute to a specific customer's prediction.

This makes the model more interpretable than treating it as a black box.

## 📈 Project Outputs

The repository contains:

* Model comparison results
* Final confusion matrix
* SHAP feature importance visualization
* Saved machine learning model
* Final evaluation metrics

## 📁 Project Structure

```text
customer-churn-prediction/
│
├── README.md
├── requirements.txt
│
├── notebooks/
│   └── Customer_Churn_Prediction_SHAP.ipynb
│
└── outputs/
    ├── model_comparison.csv
    ├── final_confusion_matrix.png
    ├── shap_feature_importance.png
    └── final_metrics.txt
```

## 🚀 Future Improvements

Possible future improvements include:

* Hyperparameter optimization
* Cross-validation
* Threshold optimization
* Deployment using Streamlit
* Customer risk dashboard
* Automated churn alerts
* Integration with a CRM system


## 👨‍💻 Author

**Bhavesh Srimalla**

B.Tech — Artificial Intelligence & Data Science
D. Y. Patil Deemed to be University / Ramrao Adik Institute of Technology
