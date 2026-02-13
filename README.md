```markdown
<p align="center">
  images/banner_1600x800.png
</p>

<div align="center">

!Status
!Python
!Power BI
!Machine Learning
!License
!Last Commit
!Repo Size

</div>

---

# 📊 Bank Customer Churn — Analytics, ML & Power BI

End‑to‑end churn analysis for a European bank (10,000 customers).  
Built using **Python** (EDA, ML pipeline, segmentation) and **Power BI** (5‑page dashboard).

---

## 🔍 Highlights

- **Overall churn ≈ 20%; Germany shows the highest (~32%)**  
- Key drivers: **NumOfProducts, Age, IsActiveMember, Geography (Germany), Balance**  
- **K‑Means segmentation** identified high‑balance inactive cluster (highest churn)  
- Model optimized for **recall‑first retention** (don’t miss churners)

📄 Findings summary → `docs/findings_summary.md`  
📘 PDF Brief → Available in Releases

---

## 🧭 Quick Navigation

- Findings → `docs/findings_summary.md`  
- Notebooks → `/notebooks`  
- Power BI Dashboard → `/powerbi/Bank_Churn_Project.pbix`  
- PBIX Data Sources → `/powerbi/exports`  
- License → `LICENSE`

---

## 📸 Dashboard Pages (Screenshots)

### Overview vs Drivers
| Overview | Drivers |
|---------|---------|
| images/overview.png | images/drivers.png |

### Geography vs Segments vs Model Outputs
| Geography | Segments | Model Outputs |
|-----------|----------|---------------|
| images/geography.png | images/segments.png | images/model_outputs.png |

---

## 🧮 Modeling Details

### Feature Engineering
- Created `AgeBucket`, `TenureBucket`, `BalanceToSalary`
- Standardized `Geography`
- Outlier clipping

### ML Models
- Logistic Regression  
- Random Forest  
- Gradient Boosting  

Imbalance handled via `class_weight="balanced"`.

### Performance (see `model_summary.csv`)
- Accuracy: **0.65**  
- Precision: **0.65**  
- Recall: **1.00**  
- F1 Score: **0.78**

### Segmentation
- K‑Means (4 clusters)
- Behavioral + demographic grouping
- Exported to Power BI

---

## 🚀 Reproduce Locally

```bash
git clone https://github.com/ap-cloud-bit/bank-churn-analytics-powerbi.git
cd bank-churn-analytics-powerbi
pip install -r requirements.txt
