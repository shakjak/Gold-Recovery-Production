#  Gold Recovery Prediction — Zyfra Project

##  Overview
This project develops a **machine learning prototype for Zyfra**, a company that builds efficiency solutions for heavy industry.  
The goal is to **predict the amount of gold recovered from gold ore** during extraction and purification, enabling Zyfra to **optimize production**.

---

##  Dataset
The dataset includes information on:
- **Ore parameters** during extraction and purification stages  
- **Concentrations** of gold, silver, and other elements at various process points  
- **Process flow data** and **recovery efficiency**

The data is split into:
- `train.csv` — training data  
- `test.csv` — testing data  
- `full.csv` — reference dataset with complete parameters  

---

##  Approach

1. **Data Preparation**  
   - Loaded and merged datasets.  
   - Verified feature consistency across train/test sets.  
   - Handled missing values and outliers.  

2. **Exploratory Data Analysis (EDA)**  
   - Examined key features affecting gold recovery rates.  
   - Visualized metal concentrations across process stages.  
   - Analyzed correlations and recovery efficiency trends.  

3. **Feature Engineering**  
   - Created new process-based and ratio-based features.  
   - Removed redundant or low-impact variables.  

4. **Model Development**  
   - Trained multiple regression models (Linear Regression, RandomForest, XGBoost).  
   - Tuned hyperparameters using cross-validation.  
   - Evaluated performance with **SMAPE** (Symmetric Mean Absolute Percentage Error).

---

##  Results
- **Best Model:** RandomForestRegressor  
- **Evaluation Metric (SMAPE):** Achieved strong predictive performance (low error).  
- **Outcome:** The model effectively predicts gold recovery rate and identifies process conditions linked to inefficiency.

---

## 🧰 Tools & Libraries
Python • Pandas • NumPy • PlotyExpress • Scikit-learn  

---

## 💡 Key Insights
- The **rougher and final concentrate stages** are critical for predicting overall recovery.  
- **Gold concentration ratios** between feed, rougher, and final stages are strong predictive features.  
- Proper **feature scaling and data consistency checks** significantly improved model stability.

---
