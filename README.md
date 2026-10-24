# Excel Sales Intelligence Dashboard

An interactive sales analysis dashboard built in Microsoft Excel using the UCI Online Retail dataset. This project explores revenue performance, monthly trends, country-level sales, and negative-quantity transactions to demonstrate practical Excel data analysis skills.

## Project Overview
The goal of this project is to transform raw retail transaction data into a structured sales dashboard that supports business performance analysis.
Using Microsoft Excel, I analyzed more than 500,000 transaction records and created KPI summaries, PivotTables, charts, and an interactive country slicer.

## Dataset
**Source:** [UCI Machine Learning Repository — Online Retail](https://archive.ics.uci.edu/dataset/352/online%2Bretail)

The dataset contains transactions from a UK-based online retailer between December 2010 and December 2011.
Key columns include:
- `InvoiceNo` — invoice identifier
- `StockCode` — product identifier
- `Description` — product description
- `Quantity` — quantity purchased or reversed
- `InvoiceDate` — transaction date and time
- `UnitPrice` — unit price in GBP
- `CustomerID` — customer identifier
- `Country` — customer country

## Tools and Skills

- **Microsoft Excel**
- Excel formulas: `SUM`, `SUMIF`, `COUNTIF`, `COUNTIFS`, `IF`, `UNIQUE`, `FILTER`, `INDEX`, and `MATCH`
- Excel Tables and structured references
- PivotTables and PivotCharts
- Interactive Slicers
- KPI dashboard design
- Data validation and exploratory analysis
- Business insight communication

## Key Dashboard Metrics

| Metric | Result |
|---|---:|
| Total Transaction Revenue | £9,747,747.93 |
| Unique Invoice Count | 25,900 |
| Highest-Revenue Country | United Kingdom |
| United Kingdom Revenue | £8,187,806.36 |
| Positive-Quantity Revenue | £10,644,560.42 |
| Negative-Quantity Revenue | -£896,812.49 |
| Negative-Quantity Rows | 10,624 |

*Results reflect the current workbook calculations and should be interpreted according to the metric definitions below.*

## Analysis and Key Findings

### 1. Country-Level Revenue
The United Kingdom generated the highest revenue in the country analysis, with approximately **£8.19 million**.
This indicates that the UK is the dominant market in the dataset. Further analysis could investigate revenue contribution by other countries and whether the business depends heavily on its largest market.

### 2. Monthly Revenue Trends
A monthly revenue line chart was created to examine changes in transaction revenue from December 2010 through December 2011.
The chart shows a rise toward November 2011 followed by a decline in December 2011. This pattern requires further investigation before attributing it to customer behavior, seasonality, or business performance.

### 3. Negative-Quantity Transactions
The analysis identified **10,624 rows with negative quantities**, representing **-£896,812.49** in revenue.
Negative quantities may reflect returns or transaction reversals. These records should be investigated before interpreting the total as net sales or accounting revenue.

### 4. Revenue Comparison
- Revenue from positive-quantity rows: **£10,644,560.42**
- Revenue from negative-quantity rows: **-£896,812.49**
- Total transaction revenue across all rows: **£9,747,747.93**

These values reconcile arithmetically. The negative-quantity revenue is approximately **8.43%** of positive-quantity revenue in absolute terms.

## Interactive Features
- Monthly revenue trend chart
- Top 10 countries by revenue
- Country slicer for filtering connected PivotTables and charts
- KPI summaries for overall sales performance

**Current limitation:** the country slicer does not yet update every KPI. Some KPI values remain based on the full dataset, so the dashboard should not be interpreted as having fully filter-responsive KPIs.

## Methodology
1. Loaded the full retail dataset into Excel.
2. Created a revenue calculation using `Quantity × UnitPrice`.
3. Summarized revenue by country with `SUMIF`.
4. Created PivotTables and PivotCharts for product and monthly analysis.
5. Built KPI summaries for transaction revenue, invoice count, customers, and country performance.
6. Investigated negative-quantity records and invoice identifiers beginning with `C`.
7. Created a dashboard with charts, KPI summaries, and an interactive country slicer.
