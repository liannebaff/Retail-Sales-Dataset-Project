# 🛍️ Retail Sales Dataset Project

### 📝 Project Summary
This repository contains an Excel-based analysis of a synthetic retail sales dataset. The project demonstrates core data analysis skills in Excel including data transformation, pivot analysis, and VLOOKUP. The aim of this project was to practice essential data analytics techniques and extract insights from the dataset.

Key skills demonstrated: `Data exploration` `Data transformation` `Pivot tables and charts (with slicers)` `VLOOKUP` `Conditional Formatting`

---
### 🗂️ Dataset Structure
Each row in the dataset represents a single transaction with the following fields:

| Column Name        | Description                                                                 |
|--------------------|-----------------------------------------------------------------------------|
| Transaction ID     | Unique identifier for each transaction                                      |
| Date               | Date of purchase (MM/DD/YYYY format)                                        |
| Customer ID        | Unique identifier for each customer                                         |
| Gender             | Gender of the customer (Male/Female)                                        |
| Age                | Age of the customer                                                         |
| Product Category   | Category of product purchased (Clothing, Beauty, Electronics)               |
| Quantity           | Number of units purchased                                                   |
| Price per Unit     | Price of a single unit                                                      |                                                        
| Day Name           | Shows the weekday name (Monday–Sunday) of the transaction.                  |
| Month Name         | Shows the shortened month name (e.g. Jan) of the transaction                |
| Month              | Shows numeric month (1–12) of the transaction.                              |
| Year               | Shows the year of the transaction.                                          |
| Day                | Shows the day of the month of the transaction.                              |
| Generation         | Shows the generation of customers (young adult, adult and senior) by age    |
| Total Sales        | Shows sale total per transaction (Quantity * Price per unit                 |
| Commission 2023    | Shows the commission per transaction in 2023                                |
| Commission 2024    | Shows the commission per transaction in 2024                                |

---
### 🛠️ Excel Skills Demonstrated
#### ☑️ Filtering & Sorting
- Sorted data by age, product category and customer demographics (age and gender).
- Applied filters to identify high-value transactions, view transactions from specific months and date ranges, and segment customers by product category and customer demographics (age and gender).

#### ☑️ Formulas and Functions
- Demonstrated use of Excel functions such as `SUM`, `SUMIF`, `SUMIFS` and `AVERAGE` within formulas to calculate totals and averages.
- Demonstrated use of Excel functions such as `TEXT`, `MONTH`, `YEAR`, `DAY`, `IFS`, 'CONCATENATE` and `VLOOKUP`.
- Demonstrated use of formulas with arithmetic operators (e.g. multiplication), using both relative and absolute cell references.

#### ☑️ Conditional Formatting
- Applied conditional formatting to highlight the highest and lowest total sales values to identify the highest- and lowest-performing product categories.
  
#### ☑️ Pivot Tables and Charts
- Built pivot tables to analyse sales by gender and product category and sales by generation and product category.
- Created charts (stacked column and clustered column charts) to visualise data.
- Added slicers to pivot tables to enable interactive filtering by gender, generation and product category.
---
## Process

I created additional fields using formulas and functions in Excel:  

| Column Name                    | Formula / Tool Used                                                               | Description                                                                 |
|--------------------------------|-----------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
| Day Name                       | `=TEXT(Date,"dddd")`                                                              | Shows the weekday name (Monday–Sunday) of the transaction.                  |
| Month Name                     | `=TEXT(Date,"mmm")`                                                               | Shows the shortened month name (e.g. Jan) of the transaction                |
| Month                          | `=MONTH(Date)`                                                                    | Shows numeric month (1–12) of the transaction.                              |
| Year                           | `=YEAR(Date)`                                                                     | Shows the year of the transaction.                                          |
| Day                            | `=DAY(Date)`                                                                      | Shows the day of the month of the transaction.                              |
| Generation                     | `=IFS()`                                                                          | Shows the generation of customers (young adult, adult and senior) by age    |
| Total Sales                    | Formulas with arithmetic operators (e.g.`=B1*A1`)                                 | Dynamic calculations based on row.                                          |
| Commission 2023                | Formulas with arithmetic operators and absolute cell references (e.g.`=$B$1*A1`)  | Shows the commission per transaction in 2023                                |
| Commission 2024                | As above.                                                                         | Shows the commission per transaction in 2024                                |

---
### 📁 Files in This Repository
- [retail_sales_dataset_analysis.xlsx](files/retail_sales_dataset_analysis.xlsx)
  <br> <br> **Worksheets**
  - <small><strong>Retail_Sales_Dataset:</strong> processed and analysed sales data.</small>
  - <small><strong>Sales by Gender and Product Category:</strong> pivot table and chart summarising sales</small>  
  - <small><strong>Sales by Generation and Product Category:</strong> pivot tables and charts summarising sales</small>  
  - <small><strong>Transactions Lookup:</strong> used transaction IDs to retrieve total sales and product categories via VLOOKUP</small>



