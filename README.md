# Retail Store Sales Performance Analysis
### Introduction
#### This project presents the results of analyzing the sales performance of a retail store. Uncovering insights that can help with the growth of the organization and also addressing the less productive areas of the business.

Key insights addressed;

- Highest selling product to identify product with less sales and the one topping the list.

- The total sales of each region and identifying the region with less sales.
- The quantity of each products sale.
- The total revenue earned in each month, year and quarter.
- The analysis includes deriving various objectives to understand the underlying issues and to propose actionable recommendations.

### Data Overview
- Data Source:The primary source of data used here is Lita Capstone Datasets which was provided by the Incubator Hub, an organization that supplies educational datasets for learning and training purposes. The data was provided in an excel format, making it easy to analyze on the Excel Spreadsheets.
- Tools: Microsft Excel [Download Here](https//:www.microsoft.com).
- Sql
- Power Bi

  ### Data Cleaning with Excel:
1. Removed duplicate values,checked spelling errors, blank cells: About 40,099 duplicated values were removed and this includes blank spaces, duplicated figures.
![duplicate value Screenshot 2024-11-04 131317](https://github.com/user-attachments/assets/23a094d3-2b27-4f58-9066-c4d9d66b7948)


2. Formatting: Introduced calculated revenue column to show the revenue acquired by each cell by their quantity and unit price,E.g =Quantity(cell)*Unit price(cell).Using my cursor to autofill by clicking and holding the fill handle by double clicking on the plus sign beside my cell.

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


### Basic statistics about the dataset:
Total Sales: 2,101,090

Total Quantity Sold: 68,461 items

Number of Unique Customers: 9,921

Number of Product Category: 6






