# LITA-CAPSTONE-PROJECT 1

### Project Title: Sales Data
---

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools Used](#tools-used)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results](#results)
- [Recommendations](#recommendations)

### Project Overview 
---
This project aims to analyze the sales performance of a retail store. It aims to achieve this through the exploration of  sales data to uncover key insights such as top-selling products, regional performance, and monthly sales trends. 

### Data Sources
---
Excel file

### Tools Used
---
- Microsoft Excel
  1. For data cleaning
  2. For analysis
  3. For visualization
- Structured Query Language (SQL)
  1. For querying
  2. For analysis
- Microsoft Power BI
  1. For visualization
  2. For reports
- GitHub
  1. For portfolio building

### Data Cleaning and Preparation 
---
Data cleaning was performed at the initial phase of the analysis. It was carried out using the Microsoft Excel. The actions included;
 1. Data loading and inspection
 2. Removing duplicate data
 3. Formating and cleaning

![1730829942831831312448531670944](https://github.com/user-attachments/assets/e7b27e04-63f1-4a79-8104-af4a6cc1ca28)


### Exploratory Data Analysis 
---
To ensure a detailed analysis, the following questions were explored
 1. What is the total sales by product, region and month?
 2. What is the average sales by product?
 3. The top 3 selling product by total sales value

### Data Analysis 
---
The following SQL queries were performed on the data file.

```
SELECT 
    Product, 
    SUM(Quantity * UnitPrice) AS TotalSales 
FROM 
    SalesData 
GROUP BY 
    Product;
```

```
SELECT 
    Region, 
    COUNT(OrderID) AS SalesTransactions 
FROM 
    SalesData 
GROUP BY 
    Region;
```

```
SELECT 
    Product, 
    SUM(Quantity * UnitPrice) AS TotalSalesValue 
FROM 
    SalesData 
GROUP BY 
    Product 
ORDER BY 
    TotalSalesValue DESC 
LIMIT 1;
```

![17307906127052682545484678918572](https://github.com/user-attachments/assets/29334522-dae0-451a-b0e5-e0426fae4809)


### Results 
---
 - The result revealed that the month of February has the highest sales in across both years. 
 - The south had the highest revenue over the 2 years.
 - The top 3 selling products include; Shoes, shirts and hats.
 - A total of 6 different products were sold in the retail store
 - The total quantity of products sold was 38,681
 - The South region generated the highest percentage of revenue across the 2 years (44.2%)
   
![17307908222724532363609448051978](https://github.com/user-attachments/assets/e2e1b225-e94d-479f-af80-65d4a98e9741)



![17308275811685179146070337456874](https://github.com/user-attachments/assets/3094aadd-b664-4ce9-855d-25e4e1cd0e80)
