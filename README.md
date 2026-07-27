# Customer Churn Prediction using Machine Learning

## Participant Details

**Name:** Abhijith A Kurup

**MUID:** abhijitha-8@mulearn

---

# Business Objective

Customer churn is one of the major challenges faced by businesses, especially in industries such as telecommunications, banking, and subscription-based services. Losing existing customers can significantly impact revenue and business growth.

The objective of this project is to build machine learning classification models that can accurately predict whether a customer is likely to churn. Early prediction enables businesses to implement targeted retention strategies, improve customer satisfaction, reduce churn rates, and maximize profitability.

---

# Dataset Overview

The project uses the **Customer Churn Dataset**, which contains customer demographic information, account details, service usage patterns, and churn status.

The dataset is divided into:

- **Training Dataset:** Used for training machine learning models.
- **Testing Dataset:** Used for evaluating model performance.

Each record represents a single customer along with various attributes that influence churn behavior.

---

# Features & Target Variable

### Input Features

The dataset contains a mixture of numerical and categorical features such as:

- Customer Age
- Gender
- Location
- Subscription Details
- Account Information
- Usage Statistics
- Customer Tenure
- Service Type
- Payment Information
- Other customer-related attributes

*(Feature names may vary depending on the dataset version.)*

### Target Variable

**Churn**

- **0** → Customer is retained
- **1** → Customer has churned

This is a **binary classification problem**.

---

# Preprocessing Pipeline

The following preprocessing steps were performed before training the models:

### 1. Missing Value Handling

- Numerical features were filled using the **median**.
- Categorical features were filled using the **mode**.

### 2. Categorical Encoding

- Label Encoding was applied to convert categorical variables into numerical values.

### 3. Feature Scaling

- StandardScaler was applied to numerical features to standardize the data.

### 4. Dataset Preparation

- The provided training and testing datasets were used directly for model training and evaluation.

---

# Models Implemented

The following machine learning classification models were developed:

## 1. Logistic Regression

- Linear classification algorithm
- Fast and interpretable
- Suitable for binary classification problems

---

## 2. Decision Tree Classifier

- Tree-based supervised learning algorithm
- Easy to interpret
- Captures nonlinear relationships

---

## 3. Random Forest Classifier

- Ensemble learning algorithm
- Combines multiple decision trees
- Reduces overfitting
- Generally provides better prediction accuracy

---

# Performance Comparison

Each model was evaluated using the following metrics:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

A comparison table was generated after evaluating all three models to identify the best-performing classifier.

---

# Best Model with Justification

The model with the highest **Accuracy** and **F1-Score** was selected as the best-performing model.

In this project, the **Random Forest Classifier** performed the best because:

- It achieved the highest overall prediction accuracy.
- It balanced Precision and Recall effectively.
- It handled complex feature interactions efficiently.
- It reduced overfitting through ensemble learning.
- It produced reliable predictions on unseen test data.

Therefore, Random Forest was selected as the final model for customer churn prediction.

---

# Key Observations

- Proper preprocessing significantly improved model performance.
- Encoding categorical variables enabled machine learning algorithms to process customer information effectively.
- Feature scaling improved the convergence of Logistic Regression.
- Decision Tree was simple and interpretable but more prone to overfitting.
- Random Forest delivered the most balanced and accurate predictions among the implemented models.
- Confusion matrices helped visualize correct and incorrect classifications for each model.

---

# Business Recommendations

Based on the model predictions, businesses should:

- Identify customers with a high probability of churn.
- Launch personalized retention campaigns.
- Offer loyalty rewards and promotional discounts.
- Improve customer support for at-risk customers.
- Monitor customer engagement regularly.
- Develop targeted marketing strategies based on customer behavior.
- Use predictive analytics to make proactive business decisions.

These actions can help reduce customer attrition and improve long-term customer retention.

---

# Future Improvements

The project can be enhanced further by:

- Performing hyperparameter tuning using GridSearchCV or RandomizedSearchCV.
- Applying feature selection techniques.
- Using One-Hot Encoding for high-cardinality categorical variables.
- Handling class imbalance using SMOTE.
- Testing advanced ensemble models such as XGBoost, LightGBM, or CatBoost.
- Performing cross-validation for more reliable performance estimates.
- Deploying the model as a web application using Flask or Streamlit.
- Monitoring model performance with real-time customer data.

---

# Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

# Project Workflow

1. Data Loading
2. Data Understanding
3. Data Preprocessing
4. Missing Value Handling
5. Label Encoding
6. Feature Scaling
7. Model Training
8. Model Evaluation
9. Model Comparison
10. Best Model Selection
11. Business Recommendations

---

# Conclusion

This project successfully developed and evaluated three machine learning classification models for customer churn prediction.

After preprocessing the dataset and comparing Logistic Regression, Decision Tree, and Random Forest classifiers, the **Random Forest Classifier** emerged as the best-performing model due to its superior predictive performance and balanced evaluation metrics.

The developed model can assist organizations in identifying customers at risk of leaving, enabling proactive retention strategies and data-driven decision-making to improve customer satisfaction and business profitability.
