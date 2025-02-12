# Credit Card Fraud Detection 🚀

## 📌 Project Overview
This project aims to detect fraudulent credit card transactions using **machine learning techniques**.  
The dataset is highly imbalanced, so **SMOTE** was applied to balance the classes.  
A **Random Forest classifier** was used and fine-tuned to improve recall while preventing overfitting.  

## 📊 Dataset Information
- **Dataset:** [Credit Card Fraud Detection Dataset (Kaggle)](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)  
- **Features:** 30 PCA-transformed variables + `Time`, `Amount`  
- **Target Variable:** `Class` (0 = Non-Fraud, 1 = Fraud)  
- **Class Imbalance:** Fraud cases are **only 0.17%** of the dataset.

## ⚙️ Steps in the Project
1. **Exploratory Data Analysis (EDA)**  
   - Visualized fraud vs. non-fraud transactions  
   - Checked feature distributions and class imbalance  

2. **Data Preprocessing**  
   - Scaled `Amount` and `Time` features  
   - Applied **SMOTE** to balance fraud cases  

3. **Model Training & Tuning**  
   - Trained a **Random Forest model**  
   - Tuned hyperparameters to optimize recall  
   - Evaluated using precision, recall, and F1-score  

4. **Feature Importance Analysis**  
   - Identified the most important fraud detection features  

## 🏆 Results
- **Final Model:** Random Forest (Tuned)  
- **Recall (Fraud Cases):** Improved from **0.80 → 0.82**  
- **Precision:** 0.82 (balanced with recall)  
- **Feature Importance:** `V10`, `V12`, `V14`, `V17` were the most significant  

## 🛠️ Installation & Usage
### 1️⃣ Clone the Repository
```bash
git clone https://github.com/ashkan3171/credit-card-fraud-detection.git
cd credit-card-fraud-detection
