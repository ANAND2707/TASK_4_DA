# 🚀 TASK-4-DA — Dashboard Design | Elevate Labs Internship

## 📌 Objective
Design an interactive dashboard using Power BI for business stakeholders to visualize and analyze key business metrics such as Sales, Profit, and Customer behavior.

---

## 🗂️ Files in this Repository

| File Name | Description |
|----------|-------------|
| `Sample - Superstore.csv` | Dataset used for building the dashboard. Contains order, customer, sales, and shipping information. |
| `task_4.pbix` | Power BI Dashboard file with visualizations and DAX measures. |

---

## 📊 Tools Used
- Power BI Desktop
- Excel (for minor data formatting)
- DAX (Data Analysis Expressions)

---

## 🧹 Data Cleaning Steps
- Converted date format from `mm/dd/yyyy` to `dd/mm/yyyy` using Power BI's Power Query editor with locale set to **English (United Kingdom)**.
- Verified and removed any null or duplicate `Order ID` entries.
- Renamed columns for readability where needed.

---

## 📈 Key Measures Created

| Measure Name | DAX Formula |
|--------------|-------------|
| **Total Sales** | `SUM([Sales])` |
| **Total Profit** | `SUM([Profit])` |
| **Average Order Value** | `DIVIDE(SUM([Sales]), DISTINCTCOUNT([Order ID]))` |
| **Average Quantity per Order** | `DIVIDE(SUM([Quantity]), DISTINCTCOUNT([Order ID]))` |
| **Unique Quantity Values** | `DISTINCTCOUNT([Quantity])` |
| **Unique Orders** | `DISTINCTCOUNT([Order ID])` |

---

## 📌 Dashboard Features
- **KPI Cards:** Total Sales, Total Profit, Average Order Value
- **Time-Series Line Charts:** Monthly trend of Sales and Profit
- **Slicers for Filtering:** Region, Segment, Category, and Date Range
- **Category Performance:** Visuals for Sales by Category and Sub-Category
- **Customer Segmentation:** Breakdown by Segment
- **Maps:** Sales distribution across US states

---
