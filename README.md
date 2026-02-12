<p align="center">
  images/banner_1600x800.png
</p>

<div align="center">

!Status
!Python
![Power BI](https://img.shields.io/badge/PowerBI-Dashboard-F2C811?ields--

# 📊 Bank Customer Churn — Analytics, ML & Power BI

End‑to‑end churn analysis for a European bank (10,000 customers).  
Built with **Python** for data preparation, EDA, ML modeling & segmentation, and **Power BI** for a production‑ready dashboard.

---

## 🔎 Highlights

- **Overall churn ≈ 20%**; **Germany** has the highest rate (~32%).
- Key drivers: **NumOfProducts**, **Age**, **IsActiveMember**, **Geography (Germany)**, **Balance**.
- **K‑Means segmentation** discovered a high‑balance, inactive cluster with the highest churn.
- ML model tuned for **recall-first** to ensure capturing all churners.
- Full pipeline from **EDA → Feature Engineering → Modeling → Segmentation → Dashboarding**.

> Full findings:  
> 📄 [`docsfindings_summary.md`  
> 📘 PDF brief available in Releases

---

## 🧭 Quick Navigation

- 📘 Findings: `docs/findings_summary.md`  
- 📓 Notebooks: [`/notebooks`](not� PBIX File: [`/powerbi/Bank_Churn_Dashboard.pbix`](powerbi/Bank_Churn_Dashboard.pb`/powerbi/exports`  
- ⚖️ License: `LICENSE`

---

## 📊 Power BI Dashboard (Screenshots)

### **Overview vs Drivers**

| Overview | Drivers |
|---------|---------|
| <img src="rview.png | images/drivers.png |

### **Geography vs Segments vs Model Outputs**

| Geography | Segments | Model Outputs |
|-----------|----------|---------------|
| images/geography.png | <img srcegments.png | images/model_outputs.png |

---

## 🧮 Modeling Details

### **Feature Engineering**
- Created `AgeBucket`, `TenureBucket`, `BalanceToSalary`
- Standardized `Geography`
- Outlier handling & clipping on selected numeric fields

### **Machine Learning Models**
- Logistic Regression  
- Random Forest  
- Gradient Boosting  

Class imbalance handled via `class_weight="balanced"`.

### **Model Metrics** (See `model_summary.csv`)
- **Accuracy:** 0.65  
- **Precision:** 0.65  
- **Recall:** **1.00**  
- **F1:** 0.78  
- Business strategy: *Recall-first* (don’t miss churners)

### **Segmentation**
- K‑Means (4 clusters)
- Behavioral + demographic segmentation
- Exported to Power BI for profiling

---

## 🚀 Reproduce Locally

```bash
git clone https://github.com/ap-cloud-bit/bank-churn-analytics-powerbi.git
cd bank-churn-analytics-powerbi
pip install -r requirements.txt
