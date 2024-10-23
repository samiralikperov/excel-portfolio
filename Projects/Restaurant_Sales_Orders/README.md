# Restaurant Order Analysis

![gif dashboard](https://github.com/user-attachments/assets/57134f7c-80e9-4d29-8a65-c312992e0f89)


This project analyzes restaurant order data, providing insights into sales performance, order trends, and menu item popularity.

**Key Technical Steps for creating this dashboard without logging in or using any SQL Query tools:**
-  It is necessary to install the appropriate ODBC drivers.
-  Configure the System DNC to integrate the database with Excel.
-  Connect Excel to the required database.
-  Extract the relevant tables into the Excel data model.
-  Create the data model by setting up the appropriate relationships between the presented tables.
-  The data is organized across several sheets in the Excel file, each serving a different purpose.

## Overview: 
  
*This sheet presents a summary of key performance indicators (KPIs) such as total sales, total orders, average price per order, and trends over time.*  
  
![gif overview](https://github.com/user-attachments/assets/f75af4c4-7a83-4685-93de-d06279ede825)

I have displayed data on KPIs and summary charts based on pivot tables. The data changes based on the filters that are selected. I connected slicers and a timeline to the corresponding pivot tables, allowing for dynamic updates in the charts.

## Analysis:  
  
*This section includes various metrics for monitoring sales and order performance, with month-over-month comparisons and visualizations for better understanding.*
  
![gif analysis](https://github.com/user-attachments/assets/99fea541-5b5d-42d4-a4a7-e6a1472145da)

This sheet contains graphs that analyze the sales of different menu items. The graphs show data according to the filters applied. I used conditional formatting to create heatmap charts that are linked to the pivot tables.

I created three charts that show:
-  SALES BY HOUR OF DAY & DAY OF WEEK, $: This chart shows the sales figures for different hours and days.
-  AVERAGE ORDER PRICE BY HOUR OF DAY & DAY OF WEEK, $: This chart displays the average price of orders during different hours and days.
-  SALES BY HOUR OF DAY & DAY OF WEEK, Quantity: This chart represents the quantity of items sold at various times.

I also conducted an ABC-XYZ analysis, which provides specific recommendations for choosing certain dishes. Since the data was loaded into the data model, I used CUBEMEMBER and CUBEVALUE functions to ensure the information for retrieving specific dishes was accurate. I also created several DAX functions to calculate total sales values, average metrics for sales and orders, as well as the percentage share of each order compared to all orders and the average number of dishes per month.



## Orders:  
  
*Contains detailed order records, including order numbers, dates, times, categories, item names, and prices.*  
  
![gif orders](https://github.com/user-attachments/assets/ce3dddc0-e3c2-4c49-8452-bc31a1fdb1e8)


Using ActiveX controls and a combination of functions, I created a dynamic filter based on a specific order. This filter shows each item in the order and calculates the total number of items and the total amount for the entire order.
