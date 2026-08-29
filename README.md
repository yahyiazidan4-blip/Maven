# 🥦 Maven Market — Sales Performance Dashboard (Power BI)

A single-page interactive **Power BI** dashboard analyzing sales, profit, returns, and store distribution for the Maven Market grocery chain dataset (1997–1998), with DAX measures, target/goal tracking, and cross-filtering slicers.

---

## 🗂️ Data Model (Star Schema)

Built on a proper Power BI data model with a dedicated measures table:

**Fact tables**
- `Transactions`
- `Returns_1997-1998`

**Dimension tables**
- `Calendar`
- `Products`
- `Customers`
- `Stores`
- `Regions`

**`measure`** — a dedicated (disconnected) table used to organize all DAX measures separately from the data tables, following Power BI modeling best practice.

---

## 📊 Dashboard Visuals

- **KPI cards** (with trend line & goal tracking): Current Month Order (Total Sales), Current Month Profit, Current Month Return
- **Matrix / pivot table**: Total Transactions, Total Profit, Profit Margin, and Return Rate broken down by `product_brand`
- **Line chart**: Weekly Revenue over time, with a trend line
- **Gauge chart**: Revenue vs. Target Revenue
- **Treemap**: Store distribution by order, grouped by `store_country`
- **Filled map**: Total Transactions by store country
- **Slicers**: Date range (with a timeline slider) and Store Country

---

## 🧮 DAX Measures Used

Measures defined in the dedicated `measure` table, including:

- `Total Sales`
- `Total Profit`
- `Profit Margin`
- `Return Rate`
- `Total Return`
- `Total Transactions`
- `Revenue`
- `target revenue`
- `last month return`
- `last month transaction`
- `Last Month Profit`

These power the KPI cards' goal comparisons (e.g., "+5.69%" vs. last month) and the gauge chart's actual-vs-target visual.

---

## 🧰 Tools & Techniques Used

- **Power BI Desktop** (.pbix)
- **Data Modeling** — star schema with fact/dimension tables and relationships
- **DAX** — measures for sales, profit, returns, and month-over-month/target comparisons
- **Interactive slicers** — date range and store country, filtering all visuals on the page
- **KPI visuals** with trend lines and goal indicators
- **Filled map** and **treemap** for geographic/categorical distribution

---

## 🖼️ Dashboard Screenshot

> Add a dashboard screenshot here after uploading it to the repo, e.g.:
> ```markdown
> ![Maven Market Dashboard](./screenshots/dashboard.png)
> ```

---

## 🎓 About the Project

This project was built as part of hands-on training in the **Digital Pioneers Initiative (Digilians)** program, applying Power BI data modeling, DAX, and dashboard design skills on the Maven Market dataset.

---

## 👤 Author

**Yahyia**
