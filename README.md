# Fraud Detection Case Study

```
# Projects
1. Bank Transaction Dataset for Fraud Detection
2. Online Payments Fraud Detection Dataset
```
---

## 1. Bank Transaction Dataset for Fraud Detection
Following the same license as the author Dataset: https://www.kaggle.com/datasets/valakhorasani/bank-transaction-dataset-for-fraud-detection/data

```
# Folder sturcture to run the notebook locally
myproject/
├── .ipynb
└── dataset/
    └── bank_transactions_data_2.csv
```

**Contents:**
  - Data Analysis
  - The use of Data Mining Algorithms in Bank Transaction Fraud Detection
  - Finally, ideas of using Data Mining & Machine Learning Algorithms for future fraud prediction.

**Why Data Mining & Machine Learning?**
-    In this dataset, there are 2,000 transactions in 5 mins. So it is impossible for human to trace the transaction record one by one.

**Results:**
```
|  Clustering  | Potential Fraud Transaction |
|--------------|-----------------------------|
|  DBSCAN      | 0.68%                       |
|  OPTICS      | 0.48%                       |
```
<img width="567" height="457" alt="image" src="https://github.com/user-attachments/assets/12be6426-8d98-46e7-8d66-54128440741d" />

- DBSCAN: 0.68% of the transactions are classified as potential fraud transaction.

<img width="567" height="457" alt="image" src="https://github.com/user-attachments/assets/6edc4492-9acd-44c2-a21f-f19b0edc94ec" />

- OPTICS: 0.48% of the transactions are classified as potential fraud transaction.

**Suggestions of using Data Mining & Machine Learning Algorithms for fraud detection step by step:**
1.  The models find out "outliers" which are the potential fraud transactions in a short period of time.
2.  The staff investigate whether they are actually fraudulent transactions or not.
3.  Label the transaction as Normal / Fraud transaction after investigation.
4.  Use the labelled dataset to perform classification machine learning, for fraud detection of future transactions.

---

## 2. Online Payments Fraud Detection Dataset
Following the same license as the author Dataset: https://www.kaggle.com/datasets/rupakroy/online-payments-fraud-detection-dataset/data

```
# Folder sturcture to run the notebook locally
myproject/
├── .ipynb
└── dataset/
    └── PS_20174392719_1491204439457_log.csv
└── input/
    └── input.csv
```

**Contents:**
  - Data Analysis
  - Train and using Machine Learning model in Online Payment Transaction Fraud Detection
  - Finally, ideas of training the model with new data from time to time.

**Why Machine Learning model prediction?**
- The model could analyze the relationship of multiple columns of data for prediction, base on what it learned.

**Results:**
```
|  Classification Model | Recall Rate |
|-----------------------|-------------|
|  Random Forest        | 0.77        |
|  Logistic Regression  | 0.73        |
|  kNN                  | 0.65        |
|  SVM                  | 0.26        |
```
High Recall is Important: When the cost of false negatives is very high (fraud detection).

**Suggestions of using the model prediction step by step:**
1. Staff should investigate whether the model flagged transaction is actually a fraudulent transaction.
2. If YES, label the transaction as a fraud transaction (isFraud = 1). If NOT, label as 0.
3. Use those new labelled data as training data together with the original dataset.
4. Repeat the above process to update the model from time to time.

---
