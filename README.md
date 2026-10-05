# Online Retail Sales Dashboard (Tableau)

A Tableau dashboard that answers business questions from a CEO and a CMO using an online retail transaction dataset. Built as part of the Tata Data Visualisation Job Simulation on Forage.

## Business Problem
- **CEO:** How does revenue change month by month in 2011, and which international markets show the most demand for expansion?
- **CMO:** Which countries and customers generate the most revenue, so marketing can target them and keep them satisfied?

## Dataset
Online retail transactions from 1 Dec 2010 to 9 Dec 2011: 541,909 rows, 38 countries, 4,372 customers.
Columns: InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country.

## Data Cleaning
- Removed returns by keeping only Quantity of 1 or more.
- Removed invalid prices by keeping only Unit Price of 0 or more.
- 10,626 rows removed, leaving 531,283.
- Created a calculated field: `Revenue = Quantity * Unit Price`.
- Excluded blank CustomerIDs from the customer analysis.

## Dashboard Views
| Question | Audience | Visual |
|---|---|---|
| Revenue by month, 2011 | CEO | Line chart |
| Top 10 countries by revenue and quantity (excluding UK) | CMO | Bar chart |
| Top 10 customers by revenue | CMO | Sorted bar chart |
| Demand by country (excluding UK) | CEO | Bar chart showing all countries |

## Key Insights
- Revenue in 2011 was about 9.84M. Sales rose from September and peaked in November (about 1.51M), showing a strong seasonal pattern.
- The UK generates about 85% of total revenue, so the business depends heavily on one market.
- Outside the UK, the Netherlands (about 285K), EIRE (283K), Germany (229K), France (210K) and Australia (139K) lead in revenue.
- The top customers are 14646 (about 280K), 18102 (260K) and 17450 (195K).
- December 2011 looks low only because the data ends on 9 December.

## Files
- `dashboard.png`: dashboard screenshot
- `*.twbx`: Tableau workbook
- `Online_Retail.xlsx`: dataset (add source link)

## Live Dashboard
[View on Tableau Public](add-your-tableau-public-link-here)

## Author
**Shiva Kumar** | Aspiring Data Analyst
[LinkedIn](https://linkedin.com/in/shiva-kumar-270b20245) | [GitHub](https://github.com/shiva7065101749-spec) | [Tableau Public](https://public.tableau.com/app/profile/shiva.shiva4261)
