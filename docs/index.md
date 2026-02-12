---
title: Bank Customer Churn — Analytics, ML & Power BI
---

# Bank Customer Churn — Analytics, ML & Power BI

**Author:** Awais Pasha  
**Title:** Business Intelligence Analyst — Data Storytelling & ML  
**Repo:** ap-cloud-bit/bank-churn-analytics-powerbi

<p align="center">
  <img src="../images/banner.png" alt="Bank Customer Churn Analytics Banner" width="100%"s **10,000 bank customers** to understand and predict **customer churn** using **Python (Kaggle/Jupyter)** for data prep + modeling and **Power BI** for an executive‑ready interactive dashboard.

**Key questions:**
- Which attributes are more common among churners than non‑churners?
- Can churn be predicted using the variables in the data?
- What do overall demographics look like?
- Are there differences across **France**, **Spain**, and **Germany**?
- What **customer segments** exist?

---

## 🧭 Quick Navigation

- **GitHub Repo:** [Root README](../READMEs Summary:** [/docs/findings_summary.md- **Power BI Report (.pbix):** [/powerbi/Bank_Churn_Dashboardpbix
- **Exports used by PBIX:** [/powerbi/exports/](../powerbi/exportsotebooks/](../roject License:** /LICENSE

> Tip: If the PBIX link doesn’t download via page view, get it from the **Releases** page where it’s attached as a binary asset.

---

## 📊 Dashboard Pages (Power BI)

- **Overview:** KPIs, churn rate by geography, churn by age bucket  
- **Drivers:** Feature importance, churn by product behaviors, active member effect, balance‑to‑salary bands  
- **Geography Insights:** Churn (bars) + Avg Balance (line) by tenure buckets and country, plus a compact matrix  
- **Segments:** Cluster sizes, churn rate by segment, and a profile table (medians, %active, %card)  
- **Model Outputs:** Probability histogram, confusion matrix, and customer‑level predictions (actual vs predicted)

Screenshots (from `/images`):

| Overview | Drivers |
|---------|---------|
| !Overview | ![Drivers](../images/driversgments | Model Outputs |
|-----------|----------|---------------|
| ![Geography](../gments | ![Model Outputs](../images🧮 Modeling (Brief)

- **Data Prep:** cleaning, standardizing `Geography`, engineered `AgeBucket`, `TenureBucket`, `BalanceToSalary`  
- **Models:** Logistic Regression, Random Forest, Gradient Boosting  
- **Imbalance handling:** class weights; threshold tuning for **recall‑first** retention strategy  
