# Credit Card Fraud Detection

## Project Overview
This project aims to detect fraudulent credit card transactions to protect customers from unauthorized charges. The dataset consists of transactions made by European cardholders in September 2013, featuring 284,807 transactions, of which 492 are fraudulent (0.172%). 

## Dataset Information
- **Source:** [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud)
- **Features:** 28 PCA-transformed numerical features (`V1` to `V28`), and two original features: 
  - `Time`: Seconds elapsed between each transaction and the first transaction.
  - `Amount`: Transaction amount.
- **Target Variable:** `Class` (0 = Not Fraud, 1 = Fraud).
- **Imbalance:** The dataset is highly imbalanced, with fraudulent transactions making up only 0.172% of the data.

## Libraries Used
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`

## Machine Learning Algorithms
- **Logistic Regression**

## Evaluation Metric
- Due to the class imbalance, model performance is measured using the Area Under the Precision-Recall Curve (AUPRC), which is more meaningful than traditional accuracy metrics.

## Results
- The models were trained and evaluated using the AUPRC metric, focusing on identifying fraudulent transactions accurately.

## Acknowledgments
- The dataset is provided by [Machine Learning Group - ULB](https://www.kaggle.com/mlg-ulb/creditcardfraud).
