# Fraud Detection Case Study

## 1. Bank Transaction Dataset for Fraud Detection
Following the same license as the author Dataset: https://www.kaggle.com/datasets/valakhorasani/bank-transaction-dataset-for-fraud-detection/data

```
# Folder sturcture to run the notebook locally
myproject/
├── .ipynb
└── dataset/
    └── bank_transactions_data_2.csv
```

Contents:
  - Data Analysis
  - The use of Data Mining Algorithms in Bank Transaction Fraud Detection
  - Finally, ideas of using Data Mining & Machine Learning Algorithms for future fraud prediction.

Why Data Mining & Machine Learning?
-    In this dataset, there are 2,000 transactions in 5 mins. So it is impossible for human to trace the transaction record one by one.

Results:
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

Suggestions of using Data Mining & Machine Learning Algorithms for fraud detection step by step:
1.  The models find out "outliers" which are the potential fraud transactions in a short period of time.
2.  The staff investigate whether they are actually fraudulent transactions or not.
3.  Label the transaction as Normal / Fraud transaction after investigation.
4.  Use the labelled dataset to perform classification machine learning, for fraud detection of future transactions.
