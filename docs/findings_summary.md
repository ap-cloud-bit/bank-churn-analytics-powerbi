\# 📘 Findings Summary — Bank Customer Churn Project



This document summarizes the key analytical findings from the Bank Customer Churn project.  

It complements the Power BI dashboard and machine learning notebooks included in the repository.



---



\# ⭐ 1. Overview



The project analyzes \*\*10,000 bank customers\*\* from a European bank to identify drivers of churn, segment customers, and build predictive models.



Key questions:



\- Why are customers churning?

\- Which attributes are most important?

\- How does churn vary by geography and demographics?

\- Can we predict churn using machine learning?

\- What customer segments exist?



---



\# ⭐ 2. Overall Churn Metrics



\- \*\*Churn Rate:\*\* ~\*\*20.4%\*\*

\- Highest churn region: \*\*Germany (32.4%)\*\*

\- Lowest churn region: \*\*France (16.2%)\*\*



---



\# ⭐ 3. Key Churn Drivers (Feature Importance)



Top variables influencing churn:



1\. \*\*NumOfProducts\*\*  

2\. \*\*Age\*\*  

3\. \*\*IsActiveMember\*\*  

4\. \*\*Geography\_Germany\*\*  

5\. \*\*Balance\*\*  

6\. \*\*Balance-to-Salary Ratio\*\*



Most churners:



\- Use \*\*multiple products\*\*

\- Are \*\*older customers\*\*

\- Are \*\*inactive members\*\*

\- Have \*\*higher account balance\*\*

\- Are from \*\*Germany\*\*



---



\# ⭐ 4. Geography Insights



\- \*\*Germany\*\* has the highest churn (~32%).  

\- \*\*Spain\*\* and \*\*France\*\* are similar (~16–17%).  

\- Across all regions:

&nbsp; - Mid-to-late career customers (ages \*\*41–60\*\*) churn more.

&nbsp; - Customers with \*\*3–5 years\*\* of tenure also show elevated churn.



---



\# ⭐ 5. Customer Segments (K-Means)



Four meaningful segments identified:



| Segment | Description | Churn Rate |

|--------|-------------|------------|

| High Balance / Inactive | Older, high balance, inactive | \*\*32%\*\* |

| Low Balance / Multi‑Product | Younger, several products | \*\*19%\*\* |

| Middle-Age / Active | Active and engaged | \*\*13%\*\* |

| Young / High Products | Younger but multiple products | \*\*15%\*\* |



Segments reveal churn is \*\*behavioral\*\*, not just demographic.



---



\# ⭐ 6. Model Performance



Machine learning models evaluated using a \*\*recall-first strategy\*\* (business goal: catch all churners).



Model summary (from `model\_summary.csv`):



| Metric | Value |

|--------|--------|

| \*\*Accuracy\*\* | 0.65 |

| \*\*Precision\*\* | 0.65 |

| \*\*Recall\*\* | \*\*1.00\*\* |

| \*\*F1 Score\*\* | 0.78 |

| \*\*Best Threshold\*\* | 0.37 |



Interpretation:



\- \*\*Recall = 100%\*\* → we successfully catch all churners  

\- Precision moderate → some false positives expected  

\- Good for \*\*retention campaigns\*\* where missing a churner is costly



---



\# ⭐ 7. Power BI Dashboard Pages



1\. \*\*Overview:\*\* KPIs, churn by geography, churn by age  

2\. \*\*Drivers:\*\* Feature importance \& behavioral churn drivers  

3\. \*\*Geography Insights:\*\* Tenure vs churn vs balance  

4\. \*\*Segments:\*\* Size \& profile of customer clusters  

5\. \*\*Model Outputs:\*\* Predictions, histogram, confusion matrix  



---



\# ⭐ 8. Recommendations



\### For Retention:

\- Target \*\*High Balance / Inactive\*\* customers first  

\- Improve engagement among inactive members  

\- Conduct geographic investigation for \*\*Germany\*\*



\### For Product Strategy:

\- Revise cross-sell strategy for high-product customers  

\- Focus product personalization on ages \*\*41–60\*\*



\### For Marketing:

\- Proactive campaigns for customers with high \*\*balance-to-salary\*\* ratios  

\- Engagement nudges for customers with tenure \*\*3–5 years\*\*



---



\# END OF SUMMARY

