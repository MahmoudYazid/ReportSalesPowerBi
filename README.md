# ReportSalesPowerBi
# Retail Sales Dashboard — Power BI Report

A multi-page Power BI report (`report1.pbix`) built on a single transactional dataset, giving an overview of sales activity by **country**, **customer**, **item**, and **time**.

## 📊 Data Source

| | |
|---|---|
| Table | `Assignment-1_Data 2` |
| Columns | `BillNo`, `Itemname`, `Quantity`, `Date`, `Country`, `CustomerID` |
| Custom measure | `Measure` (used to drive the trend/line charts) |

The column names (`BillNo`, `Itemname`, `CustomerID`, `Country`, `Quantity`, `Date`) match the classic **online retail transactions** dataset structure — one row per line item on a customer's bill/invoice.

## 📄 Report Pages (10)

The report contains 10 pages mixing KPI cards, slicers, and charts:

| Page | Content |
|---|---|
| Page 1 | Clustered column chart — Total `BillNo` by `Country` |
| Page 2 | Bar chart — Total `Quantity` by `Itemname`, with `Date` & `Country` slicers |
| Page 3 | KPI card — Total `BillNo`, with `Country` & `Itemname` slicers |
| Page 4 | KPI overview cards — Total `BillNo`, distinct `CustomerID` count, `Country`, `Itemname` |
| Page 5 | Clustered column chart — Distinct `CustomerID` count by `Country` |
| Page 6 | KPI card — `Measure`, with `CustomerID` slicer |
| Page 7 | KPI cards — `Itemname`, distinct `CustomerID` count, Total `BillNo`, with `Country` slicer |
| Page 8 | Line chart — `Measure` trend over `Date` (Year/Quarter/Month/Day), with `Itemname` slicer |
| Page 9 | Line chart — Total `BillNo` trend over `Date`, with `CustomerID` slicer |
| Page 10 | Line chart — `Measure` trend over `Date`, with `Country` slicer *(default landing page)* |

> Pages are currently labeled generically ("Page 1"–"Page 10"); consider renaming them to reflect their content (e.g. "Overview", "Sales by Country", "Top Items", "Trend").

## 🛠️ Built With

- **Power BI Desktop** — PBIR (enhanced report format), schema `3.3.0`
- **Theme:** default Fluent2 theme, generated via Power BI's *Quick Create* feature

## ▶️ Opening the Report

1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (a recent version, since this file uses the newer PBIR project format).
2. Open `report1.pbix` directly.
3. Use the slicers (Country, Item, Customer, Date) on each page to filter the visuals.

## 📌 Possible Next Steps

- Rename the generic `Measure` to something descriptive (e.g. `Total Sales`).
- Add page titles/descriptions for navigation.
- Add a proper "Summary"/landing page combining the key KPIs from Page 4.
