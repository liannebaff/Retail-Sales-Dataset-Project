# 🛍️ Retail Sales Dataset Project

### 📝 Project Summary
This repository contains an Excel-based analysis of a synthetic retail sales dataset. The project demonstrates core data analysis skills in Excel, including data transformation, pivot charts/graphs and VLOOKUP. The aim of this project was to practice essential data analytics techniques and extract insights from the dataset.

### 🎯 Key skills demonstrated:
`Data exploration` `Data transformation` `Pivot tables and charts (with slicers)` `VLOOKUP` `Conditional Formatting`

### 🗂️ Dataset Overview
The dataset contains synthetic sales transactions for a retail store, including **customer details** (ID, age, gender, generation), **transaction details** (date, product category, price) and **calculated fields** such as total sales and transaction commission.



---
### 🛠️ Excel Skills Demonstrated
#### ☑️ Filtering & Sorting
- Sorted data by product category and customer demographics (age and gender).
- Applied filters to identify high-value transactions, view transactions over specific date ranges and group customers by product category and customer demographics.

#### ☑️ Formulas and Functions
- Demonstrated use of Excel functions such as `SUM` `SUMIF` `SUMIFS` `AVERAGE` within formulas to calculate totals and averages.
- Demonstrated use of Excel functions such as `TEXT` `MONTH` `YEAR` `DAY` `IFS` `CONCATENATE` `VLOOKUP`.
- Demonstrated use of formulas with arithmetic operators (e.g. multiplication), using both relative and absolute cell references.

#### ☑️ Conditional Formatting
- Applied conditional formatting to highlight the highest and lowest total sales values to identify the highest- and lowest-performing product categories.
  
#### ☑️ Pivot Tables and Charts
- Built pivot tables to analyse sales by gender and product category and sales by generation and product category.
- Created charts (stacked column and clustered column charts) to visualise data.
- Added slicers to pivot tables to enable interactive filtering by gender, generation and product category.
---
### 🧩Process
 The goal of this project was to explore and visualise the data in order to uncover patterns in customer behaviour, highlight interesting trends and create a clear picture of how different customers purchase across product categories. Here's how I worked through the Excel project, step by step.

 #### ⤵️ Data Loading
 - Imported the dataset into Excel.
 - Checked that dates, numbers and text were in the correct format.
 - Made sure key fields such as Product Category, Quantity, Price per unit, Age  and Gender had no missing values.

<img width="1068" height="288" alt="image" src="https://github.com/user-attachments/assets/c8446c66-e50e-47fc-be0b-7879454f791c" />

#### ➕ Creating Extra Fields
- The original dataset included the following fields: Transaction ID, Date, Customer ID, Age, Product Category, Quantity and Price per Unit.   
- In order to make it easier to spot patterns by day, month and generation, I created new calculated fields using formulas and functions in Excel.
- Calculated fields were created to assess the commission amounts and  total of each sale transaction.

| Column Name                    | Formulas / Functions Used                            | Description                                                       |
|--------------------------------|------------------------------------------------------|-------------------------------------------------------------------|
| Day Name                       | `TEXT`                                               | Weekday name (e.g. Monday) of the transaction                     |
| Month Name                     | `TEXT`                                               | Month name (e.g. Jan) of the transaction                          |
| Month                          | `MONTH`                                              | Numeric month (1–12) of the transaction                           |
| Year                           | `YEAR`                                               | Year of the transaction                                           |
| Day                            | `DAY`                                                | Day of the month of the transaction                               |
| Generation                     | `IFS`                                                | Generation of customers (young adult, adult and senior) by age    |
| Sale Total                     | Formulas with arithmetic operators                   | Sale total per transaction                                        |
| Commission 2023                | Formulas with absolute cell references               | Shows the commission per transaction in 2023                      |
| Commission 2024                | As above.                                            | Shows the commission per transaction in 2024                      |

- **Examples of formulas used:**  
`=TEXT(E2,"DDDD")` `=MONTH(E2)` `=YEAR(E2)` `=DAY(E2)` `=IFS(K2>50, "Senior", K2>=30, "Adult", K2<30, "Young Adult")` `=M2*N2` `=O2*$S$3`   
  
#### 🔍 Exploring and Summarising the Dataset

- Used conditional formatting to highlight the products with the highest and lowest overall sales (sum of all sale totals).
  
<img width="617" height="137" alt="image" src="https://github.com/user-attachments/assets/8bbffddc-2dbb-44a5-b84f-f7721b2296a8" />

- Explored the dataset by sorting and filtering by variables such as age, gender, product category and date.
  
<img width="1048" height="266" alt="image" src="https://github.com/user-attachments/assets/522b881f-f561-4bfc-9c49-7ba0359e02d8" />

- Calculated the total and average commission across 2023 and 2024 using `SUMIF` and `SUMIFS`.
- Used `CONCATENATE` to combine the total sales and product category into a single descriptive cell.
- **Examples of Formulas used:**  
`=SUMIF(L:L,R11,O:O)` `=SUMIFS(M:M,I:I,$T$10,L:L,R11)`




#### 🔭 `VLOOKUP` 
Used `VLOOKUP` to pull total sales and product category using the transaction ID.    
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; e.g. &nbsp; `=VLOOKUP(A2,retail_sales_dataset!A1:Q1001,COLUMN(retail_sales_dataset!O:O),FALSE)`

  
 <img width="1097" height="328" alt="image" src="https://github.com/user-attachments/assets/2d8b9728-2ddb-4979-bd6a-a82b18825837" />


#### 🔀 Pivot Tables
Built pivot tables for easy grouping, comparison and analysis of the dataset and added slicers for interactive filtering.
  
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; **a) Sales by Gender & Product Category** | **Rows =** Product Category, **Columns =** Gender and **Values =** sum of Sale Total <br> <br>
      <img width="380" height="130" alt="image" src="https://github.com/user-attachments/assets/ef5b6977-d126-452e-9647-c6d286e83182" />

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;**b) Sales by Generation & Product Category** | **Rows =** Generation, **Columns =** Product Category and **Values =** sum of Sale Total <br> <br>
      <img width="617" height="457" alt="image" src="https://github.com/user-attachments/assets/23dd53ff-9a2f-45dc-b7b0-a4512b1e2816" />


#### 📊 Pivot Charts
- Created pivot charts to visualise insights clearly.
  - Clustered column chart comparing product category sales across gender.
  - Stacked column chart illustrating sales distribution by category and generation.

<div style="display: flex; justify-content: center; gap: 20px;">
  <img src="https://github.com/user-attachments/assets/58589a08-38f5-425f-a70a-b21b2119f669" width="503.5" alt="Image 1"/>
  <img src="https://github.com/user-attachments/assets/143dd869-2138-472b-9640-84c2024261ef" width="503.5" alt="Image 2"/>
</div>

---
### 🪞Reflection

During the analysis, I explored customer behaviour, sales trends and product category performance.    
**Key findings include:**
- Adults make up the largest proportion of the overall sales across all product categories.
- The highest performing product category is electronics, whereas the lowest performing is beauty.
- Female customers bought more clothing items, whereas male customers bought more electronics than other product categories.
- Adult customers spent the most on beauty items, senior customers spent the most on electronics, and young adult customers spent the most on clothing.

---
### 📁 Files in This Repository
- **[Retail_Sales_Dataset_Analysis.xlsx](files/retail_sales_dataset_analysis.xlsx)**
&nbsp;  
  **Worksheets:**
  - <small><strong>Retail_Sales_Dataset:</strong> processed and analysed sales data.</small>
  - <small><strong>Sales by Gender and Product Category:</strong> pivot table and chart summarising sales</small>  
  - <small><strong>Sales by Generation and Product Category:</strong> pivot tables and charts summarising sales</small>  
  - <small><strong>Transaction Lookup Tool:</strong> used transaction IDs to retrieve total sales and product categories via VLOOKUP</small>

### 📋 Dataset Structure

| Column Name        | Description                                                                 |
|--------------------|-----------------------------------------------------------------------------|
| Transaction ID     | Unique identifier for each transaction                                      |
| Date               | Date of purchase (MM/DD/YYYY format)                                        |
| Customer ID        | Unique identifier for each customer                                         |
| Gender             | Gender of the customer (male/female)                                        |
| Age                | Age of the customer                                                         |
| Product Category   | Category of product purchased (clothing, beauty, electronics)               |
| Quantity           | Number of units purchased                                                   |
| Price per Unit     | Price of a single unit                                                      |                                                        
| Day Name           | Shows the weekday name (Monday–Sunday) of the transaction                   |
| Month Name         | Shows the shortened month name (e.g. Jan) of the transaction                |
| Month              | Shows numeric month (1–12) of the transaction                               |
| Year               | Shows the year of the transaction                                           |
| Day                | Shows the day of the month of the transaction                               |
| Generation         | Shows the generation of customers (young adult, adult and senior) by age    |
| Sale Total         | Shows sale total per transaction (quantity x price per unit)                |
| Commission 2023    | Shows the commission per transaction in 2023                                |
| Commission 2024    | Shows the commission per transaction in 2024                                |

