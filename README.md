# FP&A Variance Tracker — Corporate Financial Dashboard

## Project Overview
End-to-end Financial Planning & Analysis (FP&A) project simulating
a corporate finance analyst's monthly reporting cycle. Built using
real-world Microsoft Financial Sample data across 5 business segments,
6 products, and 5 countries.

## Business Problem
Finance leadership needed visibility into which segments and products
were driving revenue variance, and a reliable rolling forecast model
to support strategic planning decisions.

## What I Built

### 1. Data Analysis & Cleaning (Python)
- Loaded and cleaned 700-row financial dataset
- Stripped column formatting issues
- Created new FP&A metrics: Profit Margin %, Discount Impact %, QoQ Growth

### 2. FP&A Variance Analysis
- Budget vs Actual analysis across all segments and products
- Revenue waterfall: Gross Sales → Discounts → COGS → Net Profit
- Discount impact analysis by band
- Identified key variance drivers per segment

### 3. Rolling Forecast Model
- Built Base Case and Conservative forecast scenarios
- Used weighted moving average (3-month window)
- Calculated MAPE forecast accuracy metric
- Visualized forecast range vs actuals

### 4. SQL Analysis Layer
- Created SQLite database from cleaned data
- Wrote 5 analytical SQL queries:
  - Profit by Segment and Country
  - Monthly Revenue Trend
  - Product Performance
  - Discount Band Analysis
  - Quarter-over-Quarter Growth
- Exported all results to Excel management report

### 5. Tableau Dashboard
- 5-page interactive dashboard
- KPI cards, trend charts, variance analysis
- Filters for Year and Segment

## Key Findings
- Government and Channel Partners drove highest profit margins
- High discount band reduced margins by X% vs No Discount band
- Base Case forecast achieved X% MAPE accuracy
- Q4 consistently outperformed other quarters by X%

## Tools Used
| Tool | Purpose |
|------|---------|
| Python (Pandas, NumPy) | Data cleaning and analysis |
| Matplotlib / Seaborn | Python visualizations |
| SQLite3 | SQL database and querying |
| Excel (openpyxl) | Management reports |
| Tableau | Interactive dashboard |
| Jupyter Notebook | Development environment |
| Git / GitHub | Version control |

## Files
- `notebooks/` — 5 Jupyter notebooks (exploration to SQL)
- `outputs/` — Charts, Excel reports, Tableau workbook
- `data/` — Cleaned CSV and SQLite database

## How to Run
1. Clone this repository
2. Install requirements: `pip install pandas numpy matplotlib seaborn openpyxl`
3. Open Jupyter Notebook and run notebooks in order 01 → 05
4. Open `outputs/FPA_Dashboard.twbx` in Tableau Desktop

## Dataset
Microsoft Financial Sample — publicly available Excel dataset
covering sales, profit, COGS, and discount data across
segments, products, and countries.
