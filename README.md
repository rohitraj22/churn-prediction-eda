# Telco Customer Churn Analysis  

This project analyzes the **Telco Customer Churn dataset** to identify patterns, key factors, and customer behaviors that drive churn.  
The goal is to provide actionable insights for improving customer retention and reducing churn rates.  

---

## Project Overview  
- **Dataset Size:** 7,043 customers, 21 features  
- **Target Variable:** `Churn` (Yes/No)  
- **Objective:** Explore the dataset using **Exploratory Data Analysis (EDA)** and highlight factors most associated with churn.  

---

## Analysis Workflow  
1. **Data Loading & Cleaning**  
   - Converted `TotalCharges` to numeric.  
   - Verified no missing values.  

2. **Univariate Analysis**  
   - Distribution of gender, senior citizens, partners, contract types, and internet services.  

3. **Bivariate Analysis**  
   - Churn vs Senior Citizen, Contract Type, Internet Service, Payment Method.  

4. **Numerical Feature Analysis**  
   - Boxplots for `MonthlyCharges`, `Tenure`, and `TotalCharges` by churn status.  
   - Q-Q plot comparison for **Senior Citizens vs Non-Senior Citizens** (churned customers).  

5. **Correlation Analysis**  
   - Heatmap to examine relationships among `tenure`, `MonthlyCharges`, and `TotalCharges`.  

---

## Key Findings  

- **Churn Rate:** ~26.5% (1 in 4 customers leave).  
- **Demographics:** Senior citizens churn more often; customers without partners/dependents are more likely to leave.  
- **Contracts:** Month-to-month contracts have the highest churn; long-term contracts retain customers better.  
- **Services:** Fiber optic internet users churn more than DSL users.  
- **Billing:** Customers paying via **electronic check** churn the most; auto-pay methods reduce churn.  
- **Charges:**  
  - Churned customers have **higher monthly charges**.  
  - They also have **lower total charges**, as they churn earlier in their lifecycle.  
  - Q-Q plots reveal that churned **senior citizens face higher charges** than churned non-seniors.  
- **Correlations:**  
  - `Tenure` ↔ `TotalCharges` (0.83) → longer customers accumulate higher bills.  
  - `MonthlyCharges` ↔ `TotalCharges` (0.65).  

---

## Business Recommendations  
- Target **new customers with high monthly charges** for retention programs.  
- Provide **discounts or loyalty benefits** for senior citizens and high-charge customers.  
- Encourage **long-term contracts** instead of month-to-month plans.  
- Promote **auto-pay options** (bank transfer/credit card) to reduce churn from electronic check users.  
- Offer **value-added services** (tech support, device protection, online security) to increase stickiness.  

---

## Tech Stack  
- **Python** (pandas, numpy, matplotlib, seaborn)
- **Jupyter Notebook** for analysis
- **Visualization:** Countplots, Histograms, Boxplots, Heatmaps, Q-Q Plots
