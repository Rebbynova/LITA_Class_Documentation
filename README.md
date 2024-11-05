# Project Title: Sales Performance Analysis for a Retail Store

## Table of Contents
1. [Project Overview](#project-overview)
2. [Tools Used](#tools-used)
3. [Data Sources](#data-sources)
4. [Data Preparation in Excel](#data-preparation-in-excel)
5. [Data Exploration](#data-exploration)
6. [Excel Pivot Tables and Charts](#excel-pivot-tables-and-charts)
7. [SQL Queries and Analysis](#sql-queries-and-analysis)
8. [Power BI Visualization](#power-bi-visualization)
9. [Conclusion](#conclusion)
   
## Project Overview
This project aims to analyze and extract insight from the sales performance of a retail store. This project utilizes Microsoft excel for data cleaning and SQL for data querying and analysis, the goal is to identify trends and important metrics in the sales data and also produce an interactive Power BI dashboard.
## Tools Used
- **Excel**: For data cleaning and preliminary analysis.
- **SQL**: For querying the dataset and generating insights.
- **Power BI**: For visualization.
## Data Sources

  The dataset was provided by my instructor for a project focused on sales performance analysis for a retail store. It includes information on product, quantity, unit price, and sales.
## Data Preparation in Excel
- Data cleaning involved removing duplicates, handling missing values, and standardizing the format of the dataset.
- **Example**:
   - **Before Cleaning**: 
  2. ![image](https://github.com/user-attachments/assets/16c177b8-9a3c-458e-9eeb-013be9b2d21c)
   ![image](https://github.com/user-attachments/assets/b49ef052-ea22-4160-ae68-fe4b3bec3c99)

   - **After Cleaning**:![image](https://github.com/user-attachments/assets/a27bce2f-9a5f-468d-9293-f4c96628e57c)![image](https://github.com/user-attachments/assets/ff3faf42-2b2c-4b7f-85bf-c448207c4bdf)
## Data Exploration
The data exploration phase provided initial insights into the dataset, highlighting:
1. Most Popular Subscription Type by Number of Customers
2. Customers Who Canceled Their Subscription Within 6 Months
3. Average Subscription Duration for All Customers
4. Customers with Subscriptions Longer Than 12 Months
5. Total Revenue by Subscription Type
6. Top 3 Regions by Subscription Cancellations
7. Total Number of Active and Canceled Subscriptions

## Excel Pivot Tables and Charts

### 1. Total Sales by Product
![image](https://github.com/user-attachments/assets/755e24e0-98ed-480c-8cfb-718b3d367295)

This pivot table summarizes total sales by product, providing a clear view of revenue contributions from each item. It allows for quick comparisons and highlights which products are driving sales.
![image](https://github.com/user-attachments/assets/641c0d10-d544-403a-8eb3-3d7daa0b2d77)

Accompanying the pivot table, this pivot chart visually represents total sales by product. It offers a graphical perspective on the data, making it easier to identify trends and key performers at a glance.
### 2. Total Sales by Region
![image](https://github.com/user-attachments/assets/26fd65ff-fc35-4126-ae20-b9dfb8df9fbe)

This pivot table summarizes total sales by region, providing an overview of revenue contributions from different geographical areas. It enables quick comparisons and insights into regional performance
![image](https://github.com/user-attachments/assets/c6dfbbbd-695f-41c7-8628-1242a0e459d3)

Accompanying the pivot table, this pivot chart visually represents total sales by region. It helps to illustrate the distribution of sales across different areas, making it easier to identify regions that are performing well or need improvement.
### 3. Total Sales by Month
![image](https://github.com/user-attachments/assets/38382490-7d30-4762-b5fb-ae95aba4bd53)

This pivot table summarizes total sales by month, providing insights into sales trends over time. It allows for easy identification of seasonal patterns and monthly performance variations.
![image](https://github.com/user-attachments/assets/99914e15-9e9c-41ec-a0bd-04e0dcc1ecba)

Accompanying the pivot table, this pivot chart visually represents total sales by month. It highlights sales trends and fluctuations throughout the year, making it easier to observe patterns and identify peak sales periods.
## SQL Queries and Analysis
This phase involved executing SQL queries to extract critical insights, such as top-selling products and total revenue per product.
### Query 1: Total Sales Product
```sql
SELECT Product, SUM(Sales) AS TotalSales
FROM Salesdata
GROUP BY Product;
```

- **Purpose**: This query retrieves the total sales generated by each product,providing insight into the store's top-selling items.
### Query 2: Highest Selling Product
```sql
SELECT
     product,
     SUM(revenue) as totalsales
FROM
     csvcapstoneproject
group BY
     product
order BY
     totalsales DESC
limit 1
```
- **Purpose**: This query identifies the product with the highest sales,providing insight into the store’s best-performing item.
### Query 3: Total Revenue per Product
```sql
select 
    product,
    SUM(revenue) as totalrevenue
FROM
    csvcapstoneproject
group BY
    product
```
- **Purpose**: This query calculates the total revenue generated by each product helping to identify top-performing items in the store.

## Power BI Visualization
![image](https://github.com/user-attachments/assets/08f99fe1-50a0-4806-ad92-e8050f043492)

### Description:
This dashboard provides a comprehensive view of a retail store’s sales performance, with key metrics and visualizations to highlight important insights.

- Cards (Total Sales Revenue, Average Order Value, Total Number of Transactions): These cards offer quick insights into the store’s overall sales performance by showing total revenue, average order value, and the total number of transactions, enabling a fast assessment of key metrics.
- Product Category Chart (Bar Chart): This bar chart breaks down sales by product category, allowing viewers to see which products contribute the most to revenue. This insight helps in identifying top-performing categories for better inventory and marketing decisions.
- Regional Sales (Bar Chart): Displays revenue distribution across different regions, helping to identify areas with strong or weak sales performance. This regional breakdown can guide targeted sales strategies for each location.
- Product Quantity (Pie Chart): Shows the quantity of products sold by category, illustrating the volume of each product type sold relative to others. This is useful for understanding customer demand across various products.

## Conclusion
This project showcases my journey in analyzing sales data to derive actionable insights that can drive business decisions. Through the application of various analytical tools, including Excel for data cleaning,pivot tables and charts,and SQL for data querying as well as Power BI for visualizations, I have demonstrated my ability to interpret complex data sets and present findings in a clear, and impactful manner.

**Key Takeaways** 
- Comprehensive Sales Overview: An aggregation of total sales, average sales values, and transaction counts that provides a snapshot of overall business performance.
- Identification of Top-Performing Products: Insight into which products contribute most significantly to revenue, allowing for informed inventory and marketing strategies.
- Regional Performance Analysis: A breakdown of sales by region, identifying high-performing areas and opportunities for growth.

This project not only reflects my technical skills in data analysis and visualization but also my commitment to leveraging data to support strategic business initiatives. I look forward to applying these skills in future projects and contributing to data-driven decision-making processes.




