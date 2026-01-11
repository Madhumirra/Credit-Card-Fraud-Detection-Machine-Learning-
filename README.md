# credit-card-fraud-XGBoost

Credit Card Fraud Detection using XGBoost with robust evaluation on highly imbalanced transaction data.

# 💳 Credit Card Fraud Detection using Machine Learning

## 🔎 Project Overview
This project demonstrates **Credit Card Fraud Detection** using **XGBoost**, a powerful machine learning algorithm for structured data.  
The objective is to accurately identify fraudulent transactions while handling severe class imbalance and evaluating real-world business impact.

The project focuses on:
- Building a reliable fraud detection model
- Using appropriate evaluation metrics for imbalanced data
- Measuring business cost instead of relying only on accuracy

---

## 📂 Repository Structure
- `creditcard_fraud.ipynb` → Main notebook (data preprocessing, model training, evaluation)
- `requirements.txt` → Required dependencies
- `.gitignore` → Ignore datasets, cache, junk files
- `data/creditcard_demo_sample.csv` → Small demo file with legit + fraud rows
- `outputs/` → ROC and PR curve outputs

---

## 📊 Results
The model was evaluated using metrics suitable for imbalanced fraud data:

- **ROC-AUC**: ~0.99  
  - Indicates excellent separation between fraud and non-fraud transactions

- **PR-AUC**: ~0.92  
  - Reflects strong fraud detection performance when fraud cases are rare

- **F1-score**:  
  - Balanced precision and recall (calculated in notebook)

### 💼 Business KPI Evaluation
To reflect real-world impact, business costs were assigned:
- **False Negative (missed fraud)** cost = ₹10,000  
- **False Positive (false alarm)** cost = ₹500  

Using these values, the estimated business loss on the test dataset was calculated to assess practical usefulness of the model.

---

## ⚙️ Installation
Clone the repository and install dependencies:

```bash
git clone https://github.com/<your-username>/credit-card-fraud-XGBoost.git
cd credit-card-fraud-XGBoost
pip install -r requirements.txt
