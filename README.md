# 🛡️ Fraud Detection in Financial Transactions

This project aims to build a machine learning model to detect fraudulent financial transactions. The dataset simulates real-world financial activity over a period of 30 days and includes over 6 million transaction records.

---

## 📌 Project Objective

- Predict whether a transaction is fraudulent (`isFraud = 1`) or not (`isFraud = 0`)
- Identify key features that influence fraudulent behavior
- Support financial institutions in reducing fraud risk through proactive detection

---

## ⚙️ Tech Stack

- **Language**: Python
- **Libraries**: Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn
- **Notebook**: Jupyter Notebook

---

## 📊 Key Steps

1. **Data Cleaning**
   - Checked and handled missing values and duplicates
   - Dropped irrelevant columns like customer names

2. **Feature Engineering**
   - Converted `type` column using one-hot encoding
   - Analyzed correlations to handle multicollinearity

3. **Model Building**
   - Used Random Forest Classifier for classification
   - Split data into training and test sets (80/20)
   - Trained the model and evaluated using:
     - Confusion Matrix
     - Classification Report
     - ROC AUC Score

4. **Prediction Output**
   - Generated human-readable fraud labels: “Fraud” or “Not Fraud”
   - Displayed results with actual vs predicted labels

5. **Feature Importance**
   - Visualized the top contributing features to fraud detection

---

## 📈 Sample Output

| Actual | Predicted | Fraud_Detected |
|--------|-----------|----------------|
| 0      | 0         | Not Fraud      |
| 1      | 1         | Fraud          |
| 0      | 0         | Not Fraud      |

---

## 🔍 Key Insights

- Fraudulent transactions often have:
  - High transaction amounts
  - Zero or low initial and final balances
  - `TRANSFER` or `CASH_OUT` transaction types
- Feature importance revealed that `amount`, `oldbalanceOrg`, and transaction type were key predictors

---

## 📁 Repository Contents

- `FraudDetection.ipynb` – Main Jupyter Notebook with full project
- `Fraud.csv` – Input dataset (optional, based on privacy/sharing)
- `README.md` – Project overview and documentation

---

## ✅ Conclusion

This project successfully demonstrates how machine learning can be used to identify potentially fraudulent transactions in financial systems. The trained model and insights can be used to build automated fraud detection systems in real-time.

---
 
