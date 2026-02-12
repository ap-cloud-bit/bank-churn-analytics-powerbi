images/banner_1600x800.png
</p>

<div align="center">

![Status
![Python](https://img.shields.io/badge/Python-3.10+-blue?it](httpsize

</div>

---

# 📊 Bank Customer Churn — Analytics, ML & Power BI

End‑to‑end churn analysis for a European bank (10,000 customers).  
Built using **Python** (EDA, ML pipeline, segmentation) and **Power BI** (5‑page dashboard).

---

## 🔍 Highlights

- **Overall churn ≈ 20%; Germany shows the highest (~32%)**
- Key drivers: **NumOfProducts, Age, IsActiveMember, Germany, Balance**
- **K‑Means segmentation** identified high‑balance inactive cluster (highest churn)
- ML model optimized for **recall‑first** retention strategy

📄 **Findings summary:**  
➡️ [`docs/findings_summary.md`](docs*PDF Brief:** Included in Releases

---

## 🧭 Quick Navigation

- 📘 Findings → [`cs/findings_summary.md`  
- 📓 Notebooks → [`/notebooks`  
- 📊 Power BI →/powerbi/Bank_Churn_Project.pbix`  
- 📁 PBIX Data Sources → [`/powerbi/exports`  
- ⚖ License → [`LICENSE`

---

## 📊 Dashboard Pages (Screenshots)

### Overview vs Drivers
| Overview | Drivers |
|---------|---------|
| images/overview.png | images/drivers.png |

### Geography vs Segments vs Model Outputs
| Geography | Segments | Model Outputs |
|-----------|----------|---------------|
| <img src="images/geography.png" width="png | images/model_outputs.png |

---

## 🧮 Modeling Details

### **Feature Engineering**
- Created: `AgeBucket`, `TenureBucket`, `BalanceToSalary`
- Standardized: `Geography`
- Outlier clipping for stability

### **Models Used**
- Logistic Regression  
- Random Forest  
- Gradient Boosting  

Class imbalance handled via *class_weight="balanced"*.

### **Performance (see `model_summary.csv`)**
- Accuracy: **0.65**
- Precision: **0.65**
- Recall: **1.00**
- F1: **0.78**

### **Segmentation**
- K‑Means (4 clusters)
- Behavioral + demographic grouping

---

## 🚀 Reproduce Locally

```bash
git clone https://github.com/ap-cloud-bit/bank-churn-analytics-powerbi.git
cd bank-churn-analytics-powerbi
pip install -r requirements.txt
