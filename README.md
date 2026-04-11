# 📊 Customer Churn Prediction – Interconnect Telecom

## 🧠 Business Problem

Interconnect, a telecommunications company, aims to reduce customer churn by identifying users who are likely to cancel their services. Early detection allows the company to implement proactive retention strategies such as targeted promotions and personalized plans.

---

## 🎯 Objective

Develop a machine learning model capable of predicting customer churn using customer demographics, service usage, and contract information.

---

## 📂 Dataset

The dataset consists of multiple sources containing customer-related information:

* **contract.csv** — contract details (billing, tenure, contract type)
* **personal.csv** — demographic data
* **internet.csv** — internet services and features
* **phone.csv** — phone service details

Each dataset is linked through a unique `customerID`.

---

## ⚙️ Project Workflow

1. **Data Cleaning**

   * Handling missing values
   * Data type corrections
   * Feature consistency across datasets

2. **Exploratory Data Analysis (EDA)**

   * Distribution of customer features
   * Churn patterns across services and contract types
   * Identification of key drivers of churn

3. **Feature Engineering**

   * Encoding categorical variables
   * Creation of meaningful features (e.g., tenure groups)
   * Data normalization (if applicable)

4. **Model Development**

   * Logistic Regression
   * Random Forest
   * Gradient Boosting
   * LightGBM

5. **Model Evaluation**

   * ROC-AUC (primary metric)
   * Accuracy (secondary metric)
   * Cross-validation

---

## 🤖 Model Selection

The **LightGBM model** was selected as the final model due to its superior performance in predicting customer churn compared to other algorithms.

---

## 📈 Results

* **ROC-AUC:** ~0.93
* **Accuracy:** ~0.85

The model demonstrates strong predictive capability and generalization performance.

---

## 🔍 Key Insights

* Customers with **month-to-month contracts** show significantly higher churn rates.
* Lack of **technical support and online security services** is associated with increased churn.
* Customers with **short tenure** are more likely to leave.

---

## 💡 Business Impact

This model enables Interconnect to:

* Identify high-risk customers before they churn
* Apply targeted retention strategies
* Improve customer lifetime value (CLV)
* Optimize marketing resource allocation

---

## 🔧 Real-World Applications

This type of predictive model can be applied in:

* Telecommunications (customer retention)
* Automotive (predictive maintenance & customer behavior)
* Subscription-based services (SaaS, streaming platforms)

---

## 📁 Repository Structure

```
customer-churn-prediction-ds/
│
├── data/
│   ├── contract/
│   ├── internet/
│   ├── personal/
│   ├── phone/
│
├── notebooks/
│   └── churn_analysis.ipynb
│
├── README.md
├── requirements.txt
```

---

## 🚀 How to Run

```bash
git clone https://github.com/your-username/customer-churn-project.git
cd customer-churn-project
pip install -r requirements.txt
jupyter notebook
```

---

## 🧾 Requirements

* Python 3.9+
* pandas
* numpy
* scikit-learn
* lightgbm
* matplotlib / seaborn

---

## 📌 Conclusion

This project demonstrates how machine learning can be leveraged to solve real-world business problems by predicting customer behavior and enabling data-driven decision-making.

---
