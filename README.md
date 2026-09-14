# 📱 Mobile Sales Analytics Dashboard

An interactive Power BI dashboard analyzing ~3,800 mobile phone sales transactions (2021–2024) across five major brands and 19 Indian cities — tracking revenue, quantity, customer ratings, and payment trends with month-to-date and year-over-year comparisons.

## Overview

This project transforms raw retail transaction data into a set of interactive Power BI reports for tracking mobile phone sales performance. It covers three connected views — a main dashboard, an MTD (Month-to-Date) report, and a same-period-last-year comparison — all built on a single cleaned dataset and fully filterable by brand, mobile model, payment method, and time period.

## Dataset

`Mobile_Sales_Data.csv` contains 3,835 transaction records with the following fields:

| Field | Description |
|---|---|
| Transaction ID | Unique identifier for each sale |
| Day / Month / Year / Day Name | Date breakdown of the transaction |
| Brand | Apple, OnePlus, Samsung, Vivo, Xiaomi |
| Mobile Model | Specific phone model sold |
| Units Sold | Quantity per transaction |
| Price Per Unit | Sale price (₹) |
| Customer Name / Age | Buyer details |
| City | One of 19 Indian cities (Delhi, Mumbai, Bangalore, Chennai, Kolkata, Hyderabad, and more) |
| Payment Method | UPI, Credit Card, Debit Card, Cash |
| Customer Ratings | Rating given by the customer |

Data spans transactions from **2021 to 2024**.

## Dashboard Highlights

### 🏠 Main Dashboard
- **KPI cards**: Total Sales (₹769.2M), Total Quantity (19K units), Transactions (3.84K), Average Price (₹40.11K)
- **Total Sales by City** — geographic map view across India
- **Total Quantity by Month** — seasonal trend line
- **Customer Ratings by Rating Status** — Good / Average / Poor breakdown
- **Transactions by Payment Method** — UPI, Debit Card, Credit Card, and Cash split roughly evenly (~24–26% each)
- **Total Sales by Mobile Model** and **by Day Name**
- **Brand summary table** — sales, quantity, and transactions per brand (Apple, OnePlus, Samsung, Vivo, Xiaomi)

### 📅 MTD (Month-to-Date) Report
- Cumulative daily sales trend for a selected year/quarter/month
- KPI cards scoped to the selected period
- Drill-down by Year, Quarter, Month, and Day

### 📊 Same Period Last Year
- Year-over-year and quarter-over-quarter comparison charts
- Table comparing current period totals against the same period in the prior year
- Monthly and quarterly trend comparisons side by side

## Files in This Repository

| File | Description |
|---|---|
| `Mobile_Sales_Data.csv` | Raw/cleaned transaction dataset |
| `Mobile_Sales_Data_DashBoard.pbix` | Power BI source file with all report pages |
| `Mobile_Sales_Data_DashBoard.pdf` | Exported PDF snapshot of the dashboard |
| `Mobile_Sales_Report.docx` | Written summary report of findings |

## Tools & Technologies

- **Power BI Desktop** — data modeling, DAX measures, and visualization
- **CSV** — raw data source
- **DAX** — for KPIs, MTD calculations, and same-period-last-year comparisons

## How to Use

1. Clone or download this repository.
2. Open `Mobile_Sales_Data_DashBoard.pbix` in [Power BI Desktop](https://powerbi.microsoft.com/desktop/).
3. Use the slicers (Mobile Model, Payment Method, Brand, Year/Quarter/Month/Day) to filter the data.
4. Switch between the **Dashboard**, **MTD Report**, and **Same Period Last Year** pages using the in-report navigation buttons.

## Key Insights

- Apple leads in total sales (₹161.6M) narrowly ahead of Samsung and OnePlus, with Xiaomi at the lower end.
- Payment methods are fairly evenly distributed, with UPI slightly leading at ~26%.
- Customer satisfaction skews positive, with the majority of ratings falling in the "Good" category.
- Sales show mild seasonal fluctuation, peaking mid-year (July) and dipping in February.

## License

This project is intended for educational and portfolio purposes.
