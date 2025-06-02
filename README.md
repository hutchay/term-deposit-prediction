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
- Decision Tree model evaluation with classification report and confusion matrix
- Random Forest model evaluation with classification report and confusion matrix

## 📊 Visuals
- Subscription class distribution 

![image](https://github.com/user-attachments/assets/adc3b95b-4f6a-4f02-a5c3-6ee81b54657d)
 
- Confusion Matrix

Logistic Regression  
![image](https://github.com/user-attachments/assets/87d9b121-0116-4132-8e8a-69a4972d9cf5)


- Decision Tree

  
![image](https://github.com/user-attachments/assets/655caf7e-bdca-4ab7-9624-9e50158ee382)


- Random Forest

  ![image](https://github.com/user-attachments/assets/80be9641-7e18-4bd2-9721-60733024a336)


## 📈 Performance Snapshot - Classification report


  ![image](https://github.com/user-attachments/assets/c973ca00-d13d-4ca3-9837-dfe32fa10379)


## 📁 Files
- `Term_Deposit_Prediction_BankMarketing.ipynb` – Full Jupyter notebook with code and results
- `bank.csv` – Source dataset (not uploaded here for privacy)

## 🚀 How to Run
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```
Then open the notebook in Jupyter or Google Colab and run all cells.

## 🧠 Interpretation of Results

### 🎯 Business Context
The goal was to predict whether a customer would subscribe to a term deposit offer, based on demographic and campaign-related features. The challenge: only a small percentage of customers said “yes” — making it a classic imbalanced classification problem.

### 📈 Model Findings
- Logistic Regression achieved a recall of 62%, meaning it successfully identified over half of actual subscribers — crucial for marketing outreach.

- Decision Tree performed well in terms of accuracy but had lower recall, limiting its usefulness for identifying "yes" customers.

- Random Forest had the highest precision and accuracy but the lowest recall (11%), meaning it missed most of the actual subscribers — not ideal for this use case.

### 🔍 Key Factors Driving Subscription
- Customers contacted via cellular were more likely to subscribe.
- Higher education levels and no history of default also contributed to higher subscription rates.
- Duration was excluded from the model to avoid data leakage, though it’s known to be highly predictive.

### ✅ What This Means
- Logistic Regression or a hybrid ensemble can be used if recall (reaching likely subscribers) is the priority.

- This model can help the bank:
  - Prioritize leads for sales teams.
  - Refine marketing efforts by targeting specific demographics.
  - Reduce campaign costs by avoiding outreach to low-likelihood customers.

## 📌 Insights & Conclusion

- The project demonstrates how different models can trade off recall vs. precision — an important business decision point.
- Logistic Regression, though simpler, offered the best recall-to-precision tradeoff, making it more effective in this marketing scenario.
- Strategic features like contact method, education, and loan history were the strongest predictors of term deposit subscription.
- Features like **contact method**, **education**, and **loan/default history** are key drivers in predicting success.
- This model can help the bank **prioritize outreach**, **refine targeting**, and **increase campaign efficiency**.
