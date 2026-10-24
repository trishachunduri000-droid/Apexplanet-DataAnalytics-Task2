# ApexPlanet Task 2 — EDA & Business Intelligence

## Files
- `EDA_Report.pdf`: summary, key findings, recommendations and charts.
- `task2_eda.py`: reusable Python EDA script.
- `task2_queries.sql`: seven SQL business queries.
- `task2_dashboard_mockup.xlsx`: KPI dashboard workbook and query result sheets.
- `sales_data.sqlite`: SQLite database with table `sales_data`.
- PNG files: charts used in the report.

## Dataset summary
- Rows: 1000
- Columns: 19
- Total sales: ₹139,399,439.65 (confirm source currency)
- Orders (`Order_ID`): 1000
- Unique customers: 947
- Total quantity sold: 5435
- Missing cells: 0
- Exact duplicate rows: 0
- IQR outlier flags: 19

## How to run
1. Install dependencies: `pip install pandas matplotlib seaborn`
2. Place the cleaned CSV beside `task2_eda.py`.
3. Run: `python task2_eda.py`
4. Open `task2_dashboard_mockup.xlsx` to review KPIs, summaries and SQL outputs.

## Notes
- SQL queries use SQLite-compatible syntax. The monthly query groups by both year and month.
- The dataset includes both `Order_ID` and `Original_Order_ID`; use `Order_ID` for unique order counts.
- Outlier flags should be investigated, not automatically deleted.
- Confirm the actual currency and business meaning of `Total_Sales` before publishing results.
