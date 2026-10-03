# Bank Customer Churn Prediction & Retention Dashboard

**Overview**
This project builds a predictive machine learning model to identify bank customers who are at high risk of closing their accounts. By flagging these customers in advance, banks can shift from offering expensive, blanket discounts to executing highly targeted retention strategies, ultimately reducing customer acquisition costs.

## 🧠 Core Features & Engineering
* **Algorithm:** Engineered a Random Forest classification model capable of capturing complex, non-linear relationships in customer financial profiles.
* **Metric Optimization:** Addressed class imbalance using `class_weight='balanced'` and mathematically tuned the decision threshold to prioritize **Recall (achieving 83%)**, ensuring the maximum number of true at-risk customers are successfully identified.
* **Interactive Business Logic:** Engineered a lookup interface that calculates exact churn probability and triggers a "Targeted Retention Offer" alert only if the customer's risk exceeds a custom 30% business threshold.

## 📊 The Dataset
The model is trained on a standard dataset of 10,000+ bank customer records. Key features include:
* **Demographics:** Age, Gender, Geography
* **Financial Indicators:** Credit Score, Balance, Estimated Salary
* **Engagement Metrics:** Tenure, Number of Products, Active Member Status

## 📈 Key Findings
Feature importance analysis extracted from the Random Forest model revealed the top three indicators driving customer departure. This allows the bank to optimize retention efforts around the most critical factors:
1. **Age** of the customer
2. **Number of Products** the customer holds with the bank
3. **Total Account Balance**

## 🛠️ Technologies Used
* **Python** (Core programming)
* **Pandas & NumPy** (Data manipulation and synthetic feature engineering)
* **Scikit-Learn** (Random Forest Classifier, Feature Scaling via `StandardScaler`, Evaluation metrics)
* **Matplotlib & Seaborn** (Data visualization and feature importance plotting)

## 🚀 How to Run
1. Clone the repository.
2. Ensure you have the required libraries installed: `pip install pandas numpy scikit-learn matplotlib seaborn`
3. Run the Python script or Jupyter/Colab Notebook. The script will automatically fetch the 10,000-record dataset from a public repository, train the model, and launch the interactive retention dashboard.
