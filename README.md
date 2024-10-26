# Project Title: Sales Performance Analysis for a Retail Store
## Project Overwiew
This project aims to analyze and extract insight from the sales performance of a retail store. This project utilizes Microsoft excel for data cleaning and SQL for data querying and analysis, the goal is to identify trends and important metrics in the sales data and also produce an interactive Power Bi dashboard.
## Tools Used
- **Excel**: For data cleaning and preliminary analysis.
- **SQL**: For quering the dataset and generating insights.
- **Power BI**: For visualization.
## Data Sources
  The dataset was provided by my instructor for a project focused on sales performance analysis for a retail store. It includes information on product, quantity, uunit price, and sales.
## Data Preparation in Excel
- Data cleaning involved removing duplicates,handling missing values, and standardizing the format of the dataset.
- **Example**:
   - **Before Cleaning**:![WhatsApp Image 2024-10-26 at 17 56 20](https://github.com/user-attachments/assets/2bdfaf4e-1566-4861-aacb-f4903dd33094) ![WhatsApp Image 2024-10-26 at 17 56 21](https://github.com/user-attachments/assets/47310da2-c10e-46b7-b029-102953d8c0b0)
   - **After Cleaning**:![WhatsApp Image 2024-10-26 at 17 56 14 (1)](https://github.com/user-attachments/assets/07e17834-6955-481d-988a-c02e54bebd5d)![WhatsApp Image 2024-10-26 at 17 56 15 (1)](https://github.com/user-attachments/assets/b7318a18-7a45-47de-8e1b-76aa5bc530ad)
## Data Exploration
The data exploration phase provided intial insights into the dataset,highlighting:
1. Most Popular Subscription Type by Number of Customers
2. Customers Who Canceled Their Subscription Within 6 Months
3. Average Subscription Duration for All Customers
4. Customers with Subscriptions Longer Than 12 Months
5. Total Revenue by Subscription Type
6. Top 3 Regions by Subscription Cancellations
7. Total Number of Active and Canceled Subscriptions
## SQL Queries and Analysis
This phase involved executing SQL queries to extract critical insights, such as top-selling products and total revenue per product.
### Query 1: Total Sales Product
```sql
SELECT Product, SUM(Sales) AS TotalSales
FROM Salesdata
GROUP BY Product;
```

- **Purpose**: This query retrieves the total sales generated by each product,providing insight into the store's top-selling items.
