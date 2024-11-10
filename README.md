# Retail Store Sales Performance Analysis
[Introduction](#introduction)

[Data Overview](#data-overview)

[Data cleaning with excel](#data-cleaning-with-excel)

[Data Transformation](#data-transformation)

[Basic statistics about the dataset](#basic-statistics-about-the-dataset)

[Power BI Visualization](#power-bi-visualization)

[INSIGHTS](insights)

[SQL](sql)


### Introduction
#### This project presents the results of analyzing the sales performance of a retail store. Uncovering insights that can help with the growth of the organization and also addressing the less productive areas of the business.

Key insights addressed;

- Highest selling product to identify product with less sales and the one topping the list.

- The total sales of each region and identifying the region with less sales.
- The quantity of each products sale.
- The total revenue earned in each month, year and quarter.
- The analysis includes deriving various objectives to understand the underlying issues and to propose actionable recommendations.

  ---
### Data Overview
- Data Source:The primary source of data used here is Lita Capstone Datasets which was provided by the Incubator Hub, an organization that supplies educational datasets for learning and training purposes. The data was provided in an excel format, making it easy to analyze on the Excel Spreadsheets.
- Tools: Microsft Excel [Download Here](https//:www.microsoft.com).
- Sql
- Power Bi
  

     ----
  ### Data Cleaning with Excel:
1. Removed duplicate values,checked spelling errors, blank cells: About 40,099 duplicated values were removed and this includes blank spaces, duplicated figures.
![duplicate value Screenshot 2024-11-04 131317](https://github.com/user-attachments/assets/23a094d3-2b27-4f58-9066-c4d9d66b7948)


3. Formatting: Introduced calculated revenue column to show the revenue acquired by each cell by their quantity and unit price,E.g =Quantity(cell)*Unit price(cell).Using my cursor to autofill by clicking and holding the fill handle by double clicking on the plus sign beside my cell.

  ![revenue calculation](https://github.com/user-attachments/assets/3fb9e5fd-11bc-4d1e-9e33-d408ecb65fbb)

2a.  Calcualated the average sales of each product by using formula 
=AVERAGEIF(C2:C9922,"SHIRT",H2:H9922)
In this formula, "Shirt" was replaced with other products like Gloves, Hat, Socks, Shoes and Jacket to get the average sales of each product.

![Screenshot 2024-11-05 114431 pngAVERAGE](https://github.com/user-attachments/assets/711a41b7-8869-48c8-98f6-2753a09a7ef7)

### Data Transformation:
1.  Ensured all data fields were assigned the correct data types, with numerical fields formatted by removing the decimal point, 
   differentiating figures by comma(,) where appropriate, and rounding up figures by custom.
 
2.  Sorting: Sorted the dataset by the largest to smallest to show the top selling product and highest sales.

3. Inserted Pivot Table to create dashboard:
  Pivot Table Summarization Includes
 

  i. Total Sales by revenue: This report provides a summary of total sales generated. It summarizes the total generated from the retail store all year roun.

 ii. Total Sales by Month: This report provides a summary of total sales by month. This show the different sales made in each months, it showcase the trends of sales in months, which will enable track performance, make data driven decisions, optimize operation and enhances customer experience,it also helps to know sales channel, employee productivity, cash flow,by leveraging on the monthly reports it helps the retail store to make profound decisons,drive growth and stay competitive.

 iii. Total Sales by Region: This report summarizes total sales across different regions. This helps in identifying high-performing region, detect under performing regions, to make expansion or contraction decisions.

 iv Total Sales by Product: This provides a summary of total sales each product generated. It helps identify high selling products,product with less sales, to know product discontinuation or replacement, to also recognize products that needs more visibilty or publicity, this also enables the retail store identifies the most preffered customer product demand in order to improve or maintain such product and get feedbacks to improve on other products underperforming.

 v. Average Sales Report: This report presents the average sales of each product. Identifying sales performance evaluation, predicting future trends and outocmes.It also helps in optimizing price for products and know market conditions, customer perceptions, and competition.

----

### POWER BI VISUALIZATION 
![POWER BI VISUALIZATION](https://github.com/user-attachments/assets/c9bb8ac4-5dc4-4053-bcab-577b337b7403)

---
### Basic statistics about the dataset:

1. Total Sales: 2,101,090

2. Total Quantity Sold: 68,461 items

3. Number of Unique Customers: 9,921

4. Number of Product Category: 6

 -----

### INSIGHTS

Total Sales by Product : The bar chart visualization on sales reveal the revenue generated by each product and this also shows the various products overall revenue performance with Shoe ranking high with #613K as it's total sales, Shirt ranking second with sales of #486K, Hat ranked third with #316K, Gloves with 297K, Jacket with 208K and Socks with #181K seen as product with the lowest revenue.


RECOMMENDATION : For the high selling product to be maintained, minimize stockouts, overstocking and excess inventory costs.Increase marketing strategies and efforts and retain product quality.The underperforming products should be repackaged, get customer reviews on it, take it to region that generates more sales like the South and re-introduce the product, create varieties of it and restructure niche.

REGIONAL BREAKDOWN : The pie chart visualization on regional breakdown shows the rate and revenue generated by each region. South is the first ranked region with a rate of 44% and revenue of #928K generated out of total revenue of #2.1Million, then the East with 23% with #486K revenue generated, the North can be regarded as the third highest selling region with rate of 18.42% and #387K total revenue generated, and the West region with the lowest rate of 14.29% and lowest generated revenue of #300K.

RECOMMENDATION : The South has the highest generated income and rate,knowing Shoes is also the highest selling product we can say Shoes generated most of the income in the South,for other regions and products to be improved,I suggest an intensive publicity and visibility of all the products especially on social media platforms, honest customer reviews, Price review, competitor,market survey, introduce face-face sales, and extra marketing strategies in each of the regions.To improve overall revenue of products and growth.


SALES by Monthly Trends : Column charts Visualization represent the monthly and quarterly sales repectively. The monthly reveals that febuary has the highest revenue turnover and that september has the lowest revenue, the charts also reveals seasonal hikes during seasons such as Winter and Summer and drop-down during spring and autumn, the charts shows a rise during the Winter months(December, january, February) and a fall during the Spring months(March, April, May), then another rise in the Summer months(June, July, August) and finally a fall in the Autumn months(September, October, November) and December also has a range in between low and high but not as high as February.

RECOMMENDATION : Plan targeted marketing campaigns around peak sales periods to maximize engagement and offer special discounts or promotions during off-peak periods to drive sales and smooth out fluctuations. prepare contingency plans for significant trend fluctuations, and also track trending products to understand customer preferences and develop new and improved versions.

CONCLUSION
The analysis of the retail store performance provided key insights into regional performance, product performance, monthly trends.Key insights and recommendation like Inventory Optimization, customer feedback,Reorder points,Staffing and training,Competitor Pricing Analysis, Strategic Marketing and Publicity. By identifying seasonal trends and identifing high-performing products and customer segment, the retail store can make data-driven decisions to improve sales and products performance. In conclusion, this project provides recommendation and valuable insights to help retail store increase sales and overall profitability  and also improves customer satisfaction, operational decisons unlock new opportunies and stay ahead of competitors.

----

### SQL 
Using Sql to Analyze Retail Store Sales Performance

This queries provides an analysis of sales data using SQL, Each query addresses each key insights above.
```sql 
---Total sales for each product category-
```sql 
SELECT product, SUM(Total_sale) AS Total_sale
FROM SalesData
GROUP BY product;
----Number of sales transactions in each region----
```sql 
SELECT region, COUNT(*) AS transaction_count
FROM SalesData
GROUP BY region;

---Highest-selling product by total sales value---
```sql
SELECT TOP 1 product, SUM(Total_sale) AS total_sales
FROM SalesData
GROUP BY product
ORDER BY total_sales DESC;

---Total Revenue by product ----
```sql
SELECT product, SUM(Total_sale) AS total_revenue
FROM SalesData
GROUP BY product;

-----Monthly sales-----
```sql
SELECT MONTH(Orderdate) AS month,
SUM(Total_sale) AS total_sales
FROM SalesData
WHERE YEAR(Orderdate) = 2024
GROUP BY MONTH(Orderdate)
ORDER BY MONTH(Orderdate);

----Top 5 customers by total purchase---
```sql
SELECT TOP 5 customer_id, SUM(Total_sale) AS total_purchase
FROM SalesData
GROUP BY customer_id
ORDER BY total_purchase DESC;

---Percentage of total sales by each region---
```sql
SELECT region,
SUM(Total_sale) AS total_sales,
(SUM(Total_sale) / (SELECT SUM(Total_sale) FROM SalesData) * 100) AS percentage_of_total_sales
FROM SalesData
GROUP BY region;

----Products with no sales in a quarter--
```sql
SELECT product 
FROM SalesData
GROUP BY product
HAVING SUM(CASE WHEN Orderdate BETWEEN '2024-06-01' AND '2024-08-31' THEN 1 ELSE 0 END) = 0;
 End of SQL Analys


