# Customer Churn Prediction & Model Optimization

**Name:** Abhijith A Kurup

**MUID:** abhijitha-8@mulearn

---

# 📌 Project Summary

Customer churn prediction is an important machine learning classification problem that helps businesses identify customers who are likely to discontinue using their services. Early identification of potential churn enables organizations to take proactive measures to improve customer retention, enhance customer satisfaction, and reduce revenue loss.

In this project, a machine learning classification model was developed to predict customer churn. A baseline classification model was first created and then optimized using **GridSearchCV** for hyperparameter tuning. The performance of both models was evaluated and compared using standard classification metrics. Feature importance analysis was also performed to identify the factors that contribute most to customer churn.

---

# 🛠️ Optimization Approach & Workflow

The project follows a complete machine learning pipeline from data preparation to model optimization.

## 1. Data Loading

- Imported the customer churn training and testing datasets.
- Explored dataset dimensions and feature information.
- Verified data quality before preprocessing.

## 2. Data Preprocessing

The following preprocessing steps were performed:

- Checked for missing values.
- Handled missing values using suitable imputation techniques.
- Encoded categorical variables using Label Encoding.
- Applied StandardScaler for feature scaling.
- Prepared training and testing datasets for model building.

## 3. Baseline Model

A **Random Forest Classifier** was trained using default parameters to establish the baseline performance.

The baseline model was evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Classification Report
- Confusion Matrix

## 4. Model Optimization

To improve model performance, **GridSearchCV** was applied for hyperparameter optimization.

The following parameters were tuned:

- Number of Estimators (`n_estimators`)
- Maximum Tree Depth (`max_depth`)
- Minimum Samples Split (`min_samples_split`)
- Minimum Samples Leaf (`min_samples_leaf`)

A **3-Fold Cross Validation** strategy was used to determine the best parameter combination. The optimized model was then retrained using the best hyperparameters obtained from GridSearchCV.

---

# 📊 Key Findings & Model Improvements

## Performance Comparison

| Metric | Baseline Model | Optimized Model |
|---------|---------------:|----------------:|
| Accuracy | Improved | Higher than Baseline |
| Precision | Improved | Higher than Baseline |
| Recall | Improved | Higher than Baseline |
| F1 Score | Improved | Higher than Baseline |

### Model Improvements

- GridSearchCV successfully identified improved hyperparameter values.
- The optimized model achieved better prediction performance.
- Classification accuracy increased after optimization.
- Precision and Recall improved compared to the baseline model.
- The optimized model produced a better F1 Score, resulting in improved overall classification performance.

---

# 🔍 Important Observations & Feature Importance

Feature importance analysis using the optimized Random Forest model identified the major factors influencing customer churn.

The most important features include:

1. Customer Support Calls
2. Payment Delay
3. Total Spend
4. Contract Length
5. Age
6. Subscription Type

These features have the greatest impact on predicting whether a customer is likely to churn.

---

# 💡 Business Recommendations

Based on the model analysis, the following recommendations can improve customer retention:

- Improve customer support services to reduce repeated customer complaints.
- Monitor customers with frequent payment delays and provide timely reminders.
- Encourage customers to subscribe to long-term plans through promotional offers.
- Introduce loyalty programs for high-value customers.
- Identify customers with high churn probability and implement personalized retention strategies.

---

# 🏁 Final Conclusions

This project demonstrates the complete workflow of building and optimizing a machine learning classification model for customer churn prediction.

A baseline Random Forest classifier was initially developed and later optimized using **GridSearchCV**. Hyperparameter tuning improved the predictive performance of the model, resulting in better Accuracy, Precision, Recall, and F1 Score than the baseline model.

The optimized model successfully identifies customers who are at risk of churning, while feature importance analysis provides valuable insights into the key factors affecting customer retention. These findings can support data-driven business decisions and effective customer retention strategies.

---

# 🛠️ Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

# 📂 Repository Structure

```text
.
├── model_optimization.ipynb    # Complete implementation of customer churn prediction and model optimization
└── README.md                   # Project documentation
```

---

# 🚀 Future Improvements

- Experiment with XGBoost and LightGBM classifiers.
- Apply SMOTE to handle class imbalance.
- Perform additional feature engineering.
- Explore RandomizedSearchCV and Bayesian Optimization techniques.
- Deploy the optimized model as a web application using Streamlit or Flask.

---

# 👨‍💻 Author

**Abhijith A Kurup**

**MUID:** abhijitha-8@mulearn
