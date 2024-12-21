# Lita Capstone Project Documentation

### Project Overview
---
This repository showcases my capstone project, which centers on Sales Performance Analysis for a retail store and Customer Segmentation for a subscription service. The project is divided into two primary sections, employing Excel, SQL, and Power BI for thorough data analysis and visualization.

### Project Status
---
- Project 1: Sales Performance Anaysis (Excel Completed)
- Project 2: Customer Segmentation (In Progress)
  
 ### Project 1: Sales Performance Analysis for a retail Store
 ---
  ### Current Implementation (Excel)

  ### Objective
  ---
  Analyze sales performance data to identify trend, patterns and key performance indicators for a retail store.

   ### Tools Used
   ---
   - Microsoft Excel: Used for data cleaning, preliminary analysis and basic visualizations.
  - SQL: To query, clean, and prepare data for analysis
  -  Power BI: For creating interactive dashboards and visualizations.

### Analysis Performed
---
- Pivot tables  to summarize total sales by product, region and month.
- Using Excel formulas to calculate average sales per product and total revenue by region.
- Generating additional insightful reports using charts.

### Key Insights from Excel Analysis
---
- Total Sales: Summarized Total revenue from sales transactions.
- Average Sales Per Product: Computed to understand product performance
- Regional Performance: Identified regions with the highest sales

  ### Data Visualization
 ---
 - Total Sales by Product, Region and Month.

![Screenshot 2024-11-05 152740 png pivot table](https://github.com/user-attachments/assets/887e9161-25e5-4020-9c77-464d693137c9)

- Average Sales Per Product and Total Revenue By Region

![Screenshot 2024-11-05 152928 png Average sales per product and Total revenue by region](https://github.com/user-attachments/assets/cda128aa-aade-497c-b3ee-88ba90a8bdb4)

- Additional insights represented by charts.

 ![Screenshot 2024-11-05 153057 png charts](https://github.com/user-attachments/assets/249af808-d5fa-44f6-93af-e7b993de5fdd)


### SQL Insights and Queries
---
This section continues the analysis from the Excel portion of the project by leveraging SQL to extract deeper insights from the data. The queries below address key business questions suchs as product performance, customer behaviour, and regional sales contribution.
Using SQL allows us to efficiently:
- Retrieve total sales per product category.
- Identify the top 5 customers by total purchase amount.
- Calculate total revenue,monthly sales trends, and more.
  
The queries and thier corresponding results are documented below.

 ## 1. Retrieve the Total Sales for Each Product Category
Query:

Select
Product,
SUM(CAST(Quantity AS INT) * CAST(UnitPrice AS DECIMAL(18,2))) AS TotalSales
FROM
[SalesDB].[dbo].[Lita Capstone project sales data]
GROUP BY
PRODUCT;

## Explanation: 
This query calculates the total sales for eaxh product category using rhe SUM function.The results help identify which product categories contribute the most revenue.
## Result:
The output provides a list of product categories with their respective total sales figures. The insights helps to identify top performing categories. Attached is the screenshot of the query result.

<img width="960" alt="Screenshot 2024-12-21 210935" src="https://github.com/user-attachments/assets/ccca7e74-6ba8-418f-9e2e-d406709d5da5" />

## 2.Find the Number of Sales Transaction in Each Region
Query:
SELECT
Region,
COUNT(OrderID) AS NUMBEROFSALESTRANSACTION
FROM [SalesDB].[dbo].[Lita Capstone project sales data]
GROUP BY Region;

## Explanation:
This query counts the number of transactions for each region. it provides insights into the volume of sales activity across ifferent locations.
## Result:
A table showing the total number of transactions for each region, highlighting the most active regions in term of sales. Attached is the scrrenshot of the query result.

<img width="960" alt="image" src="https://github.com/user-attachments/assets/e1e4f745-80e9-42a2-854c-1c69e9473022" />





### Upcoming Implementation
---
- Power Bi Dashboard (In Progress)

### Project 2: Customer Segmentation for a Subscription Service
  ---
  ### Objectives
  ---
 - Segment Customers: Group customer based on demographics, behaviors,and subscription types
- Analyze Subscription Trends: Track the popularity of different subscription types.
- Understand Retention: Identify patterns in customer cancellations and renewals.
- Develop a Power BI Dashboard: Present findings visually for easy exploration and decision making.

 ### Planned Implementation
  ---
 - Customer behavior analysis using Excel
- Database queries and analysis using SQL
- Interactive dashboards using Power BI

 ### Tools Used
  ---
 - Microsoft Excel (In Progress)
- SQL (In Progress)
- Power BI ( In Progress)




  


