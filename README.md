# 📊 Data Intelligence Dashboard

**Data Analysis using Microsoft Excel** — *Data • Insights • Growth*

An end-to-end Excel project that turns 250 raw customer transactions into an interactive dashboard, customer segmentation, what-if scenarios, a regression model, and an auto-updating written report.

| | |
|---|---|
| **Submitted by** | Thakkar Disha |
| **GR ID** | 12782 |
| **Tool** | Microsoft Excel (Excel 365 recommended) |
| **File** | `Finnal_project.xlsx` |

---

## 📌 Project Overview

The workbook analyses one year of sales (**11 Apr 2024 – 11 Apr 2025**) to answer questions such as:

- Who are our most valuable customers?
- Which products and regions drive the most revenue?
- How is revenue trending month to month?
- How does order quantity relate to order value?
- What happens to revenue under best, base and worst-case assumptions?

Every analysis sheet is formula-driven and reads from the `Raw Data` sheet, so results update automatically when the data changes.

---

## 📁 Workbook Structure

| # | Sheet | Description |
|---|-------|-------------|
| 1 | **Cover** | Project title and author details |
| 2 | **Contents** | Clickable index of all sheets |
| 3 | **Dashboard** | KPI cards and 4 charts with key insights |
| 4 | **Guide** | How-to steps for pivot tables, slicers, ToolPak, Goal Seek and more |
| 5 | **Raw Data** | 250 transactions plus helper columns (`DATEDIF`, `EOMONTH`, filter helper) |
| 6 | **Analysis** | Date functions, customer group-by, high-value customers, products, regions, monthly trend |
| 7 | **Filter** | Region dropdown that returns all matching transactions |
| 8 | **What-If** | Scenario table (Best / Base / Worst) and Goal Seek |
| 9 | **Regression** | Linear regression of Quantity vs Total Amount |
| 10 | **Visualizations** | Bar, line, pie, top-customers bar, scatter with trendline |
| 11 | **Final Report** | Auto-updating insights and storytelling |

---

## 🗂️ Dataset

`Raw Data` contains **250 transactions** across **50 customers** with these columns:

`Transaction_ID` · `Date` · `Customer_ID` · `Customer_Name` · `Product_ID` · `Product_Name` · `Category` · `Quantity` · `Unit_Price` · `Payment_Method` · `Region` · `Customer_Segment` · `Customer_Since` · `Total_Amount`

Helper columns (formulas): `Days Ago (DATEDIF)`, `Month End (EOMONTH)`, `Filter Helper`.

---

## 🧮 Excel Features Demonstrated

- **Date & time functions:** `TODAY`, `NOW`, `DATEDIF`, `EOMONTH`, `EDATE`
- **Group-by aggregation:** `SUMIFS`, `COUNTIFS`
- **Text functions:** `LEFT`, `MID`, `FIND`, `UPPER`, `TEXT` (customer abbreviations)
- **List comparison:** `MATCH` (VIP list check)
- **Filtering:** `FILTER` (Excel 365) plus a version compatible with all Excel versions
- **Conditional formatting:** icon-set arrows, data bars, KPI colour rules
- **Pivot tables, PivotCharts, Slicers and Timeline** (steps in the `Guide` sheet)
- **What-If Analysis:** Scenario Manager and Goal Seek
- **Statistics:** `SLOPE`, `INTERCEPT`, `RSQ`, plus the Analysis ToolPak regression
- **Timestamp trick:** `NOW()` with iterative calculation to freeze a time value

---

## 🔑 Key Findings

| Metric | Result |
|--------|--------|
| Total revenue | **$229,192** |
| Total orders | **250** |
| Average order value | **$916.77** |
| Active customers | **50** |
| Top customer | Mark Carter (12 orders, $15,660) |
| Top product by revenue | Laptop (~29% of revenue) |
| Most frequently purchased product | Bookshelf |
| Best region | East ($59,288, ~26% share) |
| Weakest region revenue | $36,399 |
| High-value customers | 13 of 50 (revenue ≥ $6,305) driving ~49% of revenue |
| Last full month (Mar-25) | $19,899, up 23.8% vs prior month |

### Regression (Quantity → Total Amount)

- Slope: ≈ **$354** extra revenue per additional unit
- R² = **0.21**, correlation r = **0.46** (positive but moderate relationship)

### What-If Scenarios

| Scenario | Price | Volume | Discount | Revenue |
|----------|------:|-------:|---------:|--------:|
| Best case | +10% | +8% | 1% | $269,558 |
| Base case | +5% | +2% | 3% | $238,101 |
| Worst case | −2% | −5% | 6% | $200,575 |

Reaching a **+10% revenue** target ($252,112) requires roughly an **11.2% price increase**, all else equal.

---

## 💡 Recommendations

1. Focus retention efforts on **High-Value customers**.
2. Keep **best-selling products** well stocked.
3. Run campaigns in the **weakest regions and months** flagged red on the Analysis sheet.

---

## 🚀 How to Use

1. Download or clone this repository.
2. Open `Finnal_project.xlsx` in Microsoft Excel (Excel 365 recommended for `FILTER`).
3. Start at the **Contents** sheet and click any sheet name to navigate.
4. **Colour code:** blue text on yellow fill = editable inputs; black = formulas.
5. Change the region on the **Filter** sheet or the assumptions on the **What-If** sheet and watch everything update.

> **Note:** For the timestamp trick, enable *File → Options → Formulas → Enable iterative calculation*. For the regression tool, enable the *Analysis ToolPak* add-in.

---

## 📂 Repository Structure

```
.
├── Finnal_project.xlsx   # Main Excel workbook
└── README.md             # Project documentation
```

---

## 👩‍💻 Author

**Thakkar Disha** — GR ID: 12782

*Analyze • Create • Achieve*
