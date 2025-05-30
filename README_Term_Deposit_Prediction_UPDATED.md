# 📊 Term Deposit Subscription Prediction – Bank Marketing Dataset

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
- Confusion Matrix
- ROC Curve
- Classification report

## 📁 Files
- `Term_Deposit_Prediction_BankMarketing.ipynb` – Full Jupyter notebook with code and results
- `bank.csv` – Source dataset (not uploaded here for privacy)

## 🚀 How to Run
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```
Then open the notebook in Jupyter or Google Colab and run all cells.

## 📌 Insights & Conclusion

- The logistic regression model reached **71% accuracy** with **62% recall** for the minority class (subscribed customers), showing strong potential to capture real positives despite class imbalance.
- High recall is crucial in this marketing scenario, where reaching likely subscribers matters more than being perfectly precise.
- Features like **contact method**, **education**, and **loan/default history** are key drivers in predicting success.
- This model can help the bank **prioritize outreach**, **refine targeting**, and **increase campaign efficiency**.

## ✅ Next Steps
- Try additional models like XGBoost or SVM
- Add SHAP for explainable AI
- Deploy model via Streamlit
