# 🧾 Vendor Performance Analysis  
**SQL | Python | Power BI**  
A complete data analytics pipeline to evaluate and optimize vendor performance in the retail/wholesale sector.

---

## 🚀 Overview
This project analyzes vendor contribution across sales, profitability, inventory, and operations. From ETL to reporting, we identify underperformers, optimize procurement, and provide actionable insights to stakeholders.

> **Goal:** Improve profit, reduce unsold inventory, and enhance vendor relationships using data-driven strategies.

---

## 📌 Business Questions
- Who are the top vs. underperforming vendors?
- Are purchases converting effectively into sales?
- Do high-margin vendors underperform in volume?
- Which vendors hold excessive unsold stock?
- Does bulk buying reduce unit cost?

---

## 🛠️ Tools & Tech
- **MS SQL Server:** Central data warehouse  
- **Python:** ETL, data wrangling (Pandas, NumPy, SQLAlchemy)  
- **SQL:** Data joining, transformation, aggregation  
- **Power BI:** Dashboards, KPI visualization  
- **Jupyter Notebooks:** EDA & visualization  
- **GitHub:** Version control & reproducibility  

---
```plaintext
## 📁 Project Structure
│
├── Data/                              # Raw CSV files
├── logs/                              # ETL logs 
├── data_ingestion.py                  # Python ETL script
├── get_vendors_summary.py             # Feature aggregation script
├── Exploratory Data Analysis.ipynb    # Python EDA notebook (All company's raw csv data files)
├── Vendor Performance Analysis.ipynb  # Additional analysis (EDA, cleaning, feature engineering, reaearch questions & insights from vendors_final_summary)
├── Visualizing Insights.pbix          # Power BI dashboard file
└── README.md                          # Project overview and documentation (you're here!)
```

---

## 🔄 Workflow Summary
1. **Define KPIs** → Vendor performance metrics aligned to retail goals  
2. **ETL Pipeline** → CSV to MySQL via Python scripts (`ingestion_db.py`)  
3. **Logging** → Separate logs for ingestion, transformation & debugging  
4. **Cleaning & EDA** → Python + SQL for nulls, duplicates, formatting  
5. **Feature Engineering** → Profit margin, stock turnover, purchase-to-sale ratio  
6. **Aggregation** → Vendor summary table stored in DB for automation  
7. **Deep Analysis** → Python (Seaborn, Matplotlib) on final summary  
8. **Dashboarding** → Power BI connected to MySQL (auto-refresh enabled)  
9. **Reporting** → PDF with insights, strategy & recommendations  

---

## 📊 Key Insights
- 🔴 **High Margin, Low Sales:** Low performers show 41.53% avg margin vs. top vendors’ 31.17%  
- 📦 **Unsold Stock:** $2.69M in idle inventory → urgent clearance or strategy shift  
- 📉 **Over-Reliance:** Top 10 vendors = 65% of purchases → major risk  
- 💸 **Bulk Buying Advantage:** Up to 72% unit cost reduction  
- 📈 **Turnover ≠ Profit:** Weak correlation (-0.04) between stock turnover and gross profit

---

## 🧪 Hypothesis Test
**Q:** Is there a significant difference in profit margin between top and low-performing vendors?  
**Result:** ✅ *Yes* — we reject the null hypothesis. Profitability varies meaningfully.

---

## ✅ Recommendations
- 🏷️ Reprice high-margin, low-volume products to increase sales  
- 📦 Diversify vendors to reduce dependency risks  
- 📉 Optimize slow movers — clearance sales, reorder limits  
- 📊 Encourage bulk purchases with discount incentives  
- 📣 Improve marketing for poor-performing vendors  
- 🔄 Automate dashboard refresh for real-time insights  

---

> **Outcome:** Strategic improvements in profit, inventory turnover, and vendor efficiency through end-to-end analytics.

