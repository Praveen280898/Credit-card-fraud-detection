#  Credit Card Fraud Detection – Exploratory Data Analysis (EDA)

# Project Overview
This project explores **credit card transaction data** to uncover **patterns in fraudulent behavior** using Python-based data analysis and visualization.  
The goal is to understand how frauds differ from normal transactions across **time**, especially focusing on **hourly and daily variations**.


# Objectives
1. Perform **exploratory data analysis (EDA)** on the credit card dataset.  
2. Visualize and compare **normal vs fraudulent** transaction patterns.  
3. Identify **high-risk hours** when fraud is most frequent.  
4. Prepare the dataset for future **machine learning models** (optional next phase).  


# Tools and Libraries
- **Python**
- **Pandas**  data manipulation  
- **Matplotlib & Seaborn** data visualization  
- **NumPy** numerical computations  
- **Jupyter Notebook** for interactive analysis  


# Data Overview
- The dataset used is from **Kaggle: Credit Card Fraud Detection**.  
- It contains **284,807 transactions** with 31 columns.  
- `Class` variable:  
  - `0`  Normal transaction  
  - `1`  Fraudulent transaction  


# Data Processing Steps
1. **Loaded the dataset** into a pandas DataFrame.  
2. **Checked missing values**  none found, so no cleaning required.  
3. Created new time-based features:
   - `Hour`  extracted from the `Time` column  
   - `Day` derived to analyze transactions over multiple days  
   - `Hourofday`  used to plot 24-hour cycles across days  
4. Filtered data into:
   - **Normal transactions**
   - **Fraudulent transactions**


# Key Visualizations

# 1. Transactions (Normal vs Fraud)
A histogram comparing normal and fraudulent transactions per hour.

**Insight:**  
Normal transactions dominate heavily, making fraudulent activity almost invisible when plotted together.


# 2. Fraud Transactions by Hour (Two Days)
Visualized fraud counts for **Day 1** and **Day 2** separately over 24 hours.

**Insight:**  
Fraudulent transactions appear across all hours but show **distinct peaks during certain times**.  
This pattern suggests **repeated behavior** by fraudsters or system vulnerabilities during specific time windows.


# Key Insights
- The dataset is **highly imbalanced** (fraud = 0.17%).  
- Fraudulent transactions are not randomly distributed **hourly spikes** occur.  
- These findings can help:
  - **Banks** improve monitoring during high-risk hours.  
  - **Machine learning models** by providing engineered features (`Hour`, `Day`).


#  Future Scope
- Build a **classification model** (Logistic Regression, Random Forest, or XGBoost).  
- Implement **SMOTE or undersampling** to handle data imbalance.  
- Deploy a **real-time fraud detection dashboard** using Power BI or Streamlit.


# Author
**Praveen Kumar**  
 * Data Analyst | Business Strategy Enthusiast *  
PK3508687@gmail.com
