# 📑 Technical Documentation  

## Project: E-Commerce Customer Analytics  
**Tools:** Python (Pandas, Scikit-learn, Matplotlib, Seaborn, Plotly), Jupyter  
**Deliverables:** RFM results, churn predictions, dashboards, technical pipeline  

---

### 1. Data Sources & Preparation  
- Dataset: Olist (Kaggle)  
- Files: orders, customers, items, payments, reviews, products, geolocation  
- Steps: missing values handled, dtype fixes, table merges, deduplication  

---

### 2. Descriptive Analytics  
- **RFM Segmentation:** quartile scoring → 9 groups (Champions, Loyal, At Risk, Lost, etc.)  
- **CLV:**  
  - Avg CLV ≈R$180 per customer  
  - VIPs >R$5K  
  - Total CLV ≈R$17–23M  

---

### 3. Diagnostic Analytics  
- Churn = inactivity >180 days  
- Cohort analysis: 99.7% drop-off within 3 months  
- Avg time between first & second purchase: 81 days  

---

### 4. Predictive Analytics  
- Model: Logistic Regression (70/30 split)  
- Features: Recency, Frequency, Monetary, days active, reviews, payments  
- Metrics: Accuracy 73.9%, F1 84.9%, ROC-AUC 0.64  
- Findings: 30,475 high-risk customers ≈R$5.7M CLV at risk  

---

### 5. Prescriptive Analytics  
- ROI-driven strategy: prioritize VIP & high-risk  
- Retention uplift: 20–40%  
- Protected revenue: ≈R$1.1–2.3M  

---

### 6. Deliverables  
- **Data:** RFM outputs, churn analysis, predictions, intervention list  
- **Visuals:** 10+ plots + executive dashboard  
- **Models:** Logistic Regression (pickle), scaler  
- **Docs:** Exec Summary, Technical Docs, README  

---

### 7. Limitations & Assumptions  
- Churn = 180+ days inactivity  
- Historical data only (2016–2018)  
- ROI depends on implementation quality  

---

### 8. Reproducibility  
- Code: Jupyter notebooks + scripts  
- Models & scalers saved  
- End-to-end preprocessing documented  
