
# 📑 Technical Documentation  

## Project: E-Commerce Customer Analytics  
**Language & Tools:** Python (Pandas, Scikit-learn, Matplotlib, Seaborn), Jupyter Notebooks  
**Deliverables:** RFM results, churn predictions, executive dashboard, technical pipeline  

---

### 1. Data Sources & Preparation  
- Dataset: Olist Brazilian E-Commerce Public Dataset (Kaggle)  
- Files: orders, customers, order_items, payments, reviews, products, geolocation  
- Data Cleaning Steps:  
  - Missing value treatment  
  - Data type conversions (dates, floats, categories)  
  - Merge across multiple tables (customer → order → item → payment → review)  
  - Deduplication & quality checks  

---

### 2. Descriptive Analytics  
**RFM Segmentation:**  
- Recency: Days since last purchase  
- Frequency: Number of purchases per customer  
- Monetary: Total spend  
- Scoring: Quartile-based (1–4) → Segmentation into 9 groups (Champions, Loyal, At Risk, Lost, etc.)  

**Customer Lifetime Value (CLV):**  
- CLV = (Average Order Value × Purchase Frequency × Gross Margin × Time Horizon)  

---

### 3. Diagnostic Analytics  
- **Churn Analysis:** Defined churned customers as those inactive for 6+ months  
- **Cohort Analysis:** Built monthly cohorts by acquisition month, tracked retention over time  
- **Repeat Purchase Analysis:** Time between first and second purchase (avg 81 days)  

---

### 4. Predictive Analytics  
**Modeling Objective:** Predict churn risk for active customers  

- Features engineered: Recency, Frequency, Monetary, days since first purchase, review scores, payment types  
- Model: Logistic Regression (baseline for interpretability)  
- Training/Test Split: 70/30  
- Performance Metrics:  
  - Accuracy: 73.85%  
  - ROC-AUC: 0.64  
  - Precision-Recall tradeoffs evaluated  
- Outputs: churn_predictions_improved.csv, logistic_regression_model.pkl  

---

### 5. Prescriptive Analytics  
**Action Plan Development:**  
- Segment-level strategy mapping (Champions vs At Risk vs Lost)  
- ROI-based prioritization → high-value at-risk customers first  
- Projected retention uplift: 20–40%  
- Dashboard: Executive view summarizing segments, risks, and financial impact  

---

### 6. Deliverables  
- **Data Files:** RFM results, churn analysis, predictions, intervention list  
- **Visuals:** 10+ analytical plots, executive dashboard screenshot  
- **Models:** Logistic regression pickle file, feature scaler  
- **Documentation:** Executive Summary (business), Technical Documentation (methodology), README (portfolio)  

---

### 7. Limitations & Assumptions  
- Assumes churn defined as **180 days of inactivity**  
- Predictive model trained only on historical data (2016–2018)  
- ROI estimates depend on implementation effectiveness  

---

### 8. Reproducibility  
- Full code available in repository (Jupyter notebooks + .py scripts)  
- Data preprocessing and modeling steps documented end-to-end  
- Models & scalers saved for production use  

---

✅ **This documentation ensures technical transparency and reproducibility, while the Executive Summary communicates business value to stakeholders.**  
