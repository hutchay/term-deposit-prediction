 📊 Term Deposit Subscription Prediction – Bank Marketing Dataset

This project uses classification models to predict whether a customer will subscribe to a term deposit based on a variety of demographic and campaign-related factors.

## 🧠 Objective
To build a predictive model using the Bank Marketing dataset (2015–2017) to support marketing decision-making.

## 🛠️ Tools Used
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

## 🔍 Key Techniques
- Exploratory Data Analysis (EDA)
- Feature engineering and scaling
- Handling class imbalance with `class_weight='balanced'`
- Logistic Regression model evaluation with classification report, confusion matrix, and ROC curve

## 📈 Performance Snapshot
- Accuracy: 71%
- Precision (Subscribed): 0.22
- Recall (Subscribed): 0.62
- ROC-AUC: _(you can calculate and insert this)_

## 📊 Visuals
- Subscription class distribution 

![image](https://github.com/user-attachments/assets/adc3b95b-4f6a-4f02-a5c3-6ee81b54657d)
 
- Confusion Matrix

  
![image](https://github.com/user-attachments/assets/d4c369d3-5bcd-4637-a8a8-dae2f24deadc)

- ROC Curve

  
![image](https://github.com/user-attachments/assets/b6675d7b-a073-4a88-9143-51dc7d116943)

- Classification report


  ![image](https://github.com/user-attachments/assets/ac4ab450-3306-4282-982e-c2404463c373)

## 📁 Files
- `Term_Deposit_Prediction_BankMarketing.ipynb` – Full Jupyter notebook with code and results
- `bank.csv` – Source dataset (not uploaded here for privacy)

## 🚀 How to Run
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```
Then open the notebook in Jupyter or Google Colab and run all cells.

### 🎯 Business Context
The goal was to predict whether a customer would subscribe to a term deposit offer, based on demographic and campaign-related features. The challenge: only a small percentage of customers said “yes” — making it a classic imbalanced classification problem.

### 📈 Model Findings
- The logistic regression model achieved an accuracy of 71%, but more importantly:
  - Precision (Subscribed): 22%
  - Recall (Subscribed): 62%
- This shows that:
  - While many predicted "yes" may be false positives, we are correctly identifying over 60% of customers who would actually subscribe.
  - This is useful in a marketing context, where recall is more important — better to reach out to most potential subscribers, even if some don’t convert.

### 🔍 Key Factors Driving Subscription
- Customers contacted via cellular were more likely to subscribe.
- Higher education levels and no history of default also contributed to higher subscription rates.
- Duration was excluded from the model to avoid data leakage, though it’s known to be highly predictive.

### ✅ What This Means
This model can help the bank:
- Prioritize leads for sales teams.
- Refine marketing efforts by targeting specific demographics.
- Reduce campaign costs by avoiding outreach to low-likelihood customers.

## 📌 Insights & Conclusion

- The logistic regression model reached **71% accuracy** with **62% recall** for the minority class (subscribed customers), showing strong potential to capture real positives despite class imbalance.
- High recall is crucial in this marketing scenario, where reaching likely subscribers matters more than being perfectly precise.
- Features like **contact method**, **education**, and **loan/default history** are key drivers in predicting success.
- This model can help the bank **prioritize outreach**, **refine targeting**, and **increase campaign efficiency**.
