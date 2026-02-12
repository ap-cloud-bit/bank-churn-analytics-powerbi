[Banner]
<p align="center">
  images/banner_1600x800.png
</p>

<div align="center">

![Status](https://Power BI](https://imgtps://img.shhttps://img.shields.io/github/forks/ap-cloud-bit

---

## 🔎 Highlights

- **Overall churn ≈ 20%**; **Germany** has the highest rate (~32%).  
- Key drivers: **NumOfProducts, Age, IsActiveMember, Geography (Germany), Balance**.  
- **K‑Means** segmentation: high‑balance inactive cohort shows the highest churn.  
- Model tuned for **recall‑first** retention scenario (see `model_summary.csv`).

> See **docs/findings_summary.md** for the brief narrative and **project_brief_fixed.pdf** in Releases.

---

## 🧭 Quick Navigation

- **Findings summary:** [`docs/findingssummary.md`  
- **Notebooks:** [`/notebooks` 
- **Power BI (.pbix):** [`/powerbi/Bank_Churn_Dashboard.pbix`](powerbi/Bank_Churn_Dashboard.pbixxports used by PBIX:** [`powerbi/exports`  
- **Project license:** `LICENSE`

---

## 📊 Dashboard Pages (Power BI)

- **Overview:** KPIs + churn by geography, age.  
- **Drivers:** Feature importance, products, activity, balance‑to‑salary bands.  
- **Geography Insights:** Churn vs Tenure by country; compact KPI matrix.  
- **Segments:** Cluster sizes + profile table (medians, %active, %card).  
- **Model Outputs:** Churn probability histogram, confusion matrix, customer‑level predictions.

Screenshots:

| Overview | Drivers |
|---------|---------|
| images/overview.png | <img src="images/drivers.png" width="420ents | Model Outputs |
|-----------|----------|---------------|
| images/geography.png | <img src="images/segments.png"="imagesputs.png |

---

## 🧮 Modeling

- **Prep/Features:** standardize `Geography`; derive `AgeBucket`, `TenureBucket`, `BalanceToSalary`.  
- **Models:** Logistic Regression, Random Forest, Gradient Boosting; class‑weighting; threshold tuning for **recall**.  
- **Explainability:** permutation + tree importances → exported to `feature_importance.csv`.  
- **Segmentation:** K‑Means (K=4) on standardized behavior/demographics.

---

## 🚀 Reproduce Locally

```bash
git clone https://github.com/ap-cloud-bit/bank-churn-analytics-powerbi.git
cd bank-churn-analytics-powerbi
pip install -r requirements.txt
