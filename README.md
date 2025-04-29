# Fraud Detection Using Machine Learning

# Project Overview
This project focuses on identifying fraudulent financial transactions using a large dataset with over 6.3 million records and 10 features.  
It involves thorough data cleaning, predictive modeling, performance evaluation, and strategic recommendations for infrastructure improvement.

---

# Objectives
- Handle missing values, outliers, and multicollinearity in the dataset.
- Build a machine learning model for fraud detection.
- Identify key predictors of fraud.
- Evaluate the model using best-practice performance metrics.
- Provide actionable fraud prevention strategies.
- Propose methods to monitor the effectiveness of the fraud detection system post-deployment.

---

# Dataset
- **Records:** ~6.3 Million
- **Features:** 10
- **Files included:**
  - `Fraud_Detection.ipynb` (Main analysis and modeling notebook)
  - `sample_dataset.csv` (Subset of the original dataset for demonstration purposes)

> **Note:** The full dataset is not uploaded due to GitHub's 25MB file size limitation. A sample is provided for testing and understanding.

---

# Modeling Approach
- **Data Cleaning:**  
  - Removal of missing values and outliers
  - Addressing multicollinearity using correlation analysis
- **Feature Engineering:**  
  - Focus on transaction types and account balance changes
- **Algorithms Used:**  
  - Logistic Regression
  - Random Forest Classifier
- **Performance Metrics:**  
  - Accuracy
  - Precision, Recall, F1-Score
  - ROC-AUC Curve
  - Confusion Matrix

---

# Key Findings

# Important Features Predicting Fraud:
- **Transaction Amount:** Larger transaction amounts often signal potential fraud.
- **Balance Change at Origin:** A drastic drop in the sender's account balance is suspicious.
- **Old Balance of Origin:** High initial balances are often targeted by fraudsters.
- **Transaction Type:** `TRANSFER` and `CASH_OUT` transactions are more vulnerable.

# Logical Validation:
- These predictors align well with known fraud patterns: sudden large transfers, account balance draining, and cash-out activities.

---

# Model Performance
- The final model achieved high precision and recall values.
- Significant reduction in false positives compared to initial baseline models.
- ROC-AUC scores demonstrated strong separability between fraudulent and legitimate transactions.

---

# Fraud Prevention Recommendations
- **Real-Time Fraud Detection System:** Deploy the model to monitor transactions live.
- **Transaction Limits:** Dynamic thresholds based on risk scoring.
- **Behavioral Monitoring:** Track customer behavior for anomalies.
- **Multi-Factor Authentication (MFA):** Enforce MFA for high-risk transactions.
- **Blacklisting/Whitelisting:** Block accounts involved in known fraudulent activities.
- **Continuous Model Retraining:** Update the model quarterly with new fraud patterns.

---

# Post-Implementation Monitoring

# Metrics to Track:
- Fraud Detection Rate (↑)
- False Positive Rate (↓)
- Financial Losses Saved (↑)
- Precision / Recall / F1-Score stability

# Monitoring Strategies:
- A/B Testing between old and new systems.
- Drift Detection to capture changing fraud behaviors.
- User feedback analysis for customer complaints related to fraud detection.

---

# Credits
Project created and implemented by **Kumar Manik**.
