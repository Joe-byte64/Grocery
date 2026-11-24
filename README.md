# Grocery
Grocery Inventory dataset
## Table of content
- [Introduction](#introduction)
- [Project Objectives](#project-objectives).
- [Description of Dataset](#description-of-dataset).
- [Tools](#tools).
- [Data Cleaning](#data-cleaning).
- [KPIs](#kpis).
- [Research Questions](research-questions).
- [Key Findings](#key-findings)
- [Recommendations](#recommendations).
- [Conclusion](#conclusion)

## Introduction
This project described and evaluated the inventory of a grocery store.

## Project Objectives
This project is intended to provide insights into inventory of a grocery store, as a means to influence future decision-making.

## Description of Dataset
The dataset was sourced from kaggle.com. it comprises of 17 fields (columns) and 572 observations (row). it consisted of 5 unanswered questions meant to give data insights for future decision making. 

## Tools
This project was carried out using powerBi as the analytic tool.

## Data cleaning 
Data cleaning was done using power query. simple text was done and irrelevant columns was removed. replacement of missing value and setup of columns to their appropriate data-types. 

## Kpis
Total Sales Volume *Total sale volume = SUM('Grocery_Inventory new v1'[Sales_Volume])*
Total Stock Quantity *Total Stock = DISTINCTCOUNT('Grocery_Inventory new v1'[Stock_Quantity])*
Max Date Received *My_Date_table = CALENDAR(MIN('Grocery_Inventory new v1'[Date_Received]),MAX('Grocery_Inventory new v1'[Date_Received]))*
Total number of suppliers *No of Suppliers = COUNT('Grocery_Inventory new v1'[Supplier_Name])*
Average Sales Volume *Avg Stock Qty = AVERAGE('Grocery_Inventory new v1'[Stock_Quantity])*

## Research Questions
1. What is the average stock quantity available per product category? 
2. Which suppliers contribute the most to total product inventory?
3. Which products have the longest shelf life before expiration, and how does that impact sales?
4. Which products are most likely to run out of stock based on last reorder levels? 
5. Can we predict seasonal demand for different product categories based on sales volume trends?
6. What are the optimal reorder levels for high-demand products to prevent stockouts?

## Key Findings
1. The average stock quantity ranges from 50.86 to 62.23 (Grains & Pules - Seafood).
<img width="422" height="182" alt="Screenshot 2026-11-24 041241" src="https://github.com/user-attachments/assets/066cfe9d-94b2-4bc0-a2a3-107846a09425" />

2. Katz, Twitterwire, Meevee, Quart and feed fire contributed most to the product inventory.
<img width="427" height="416" alt="Screenshot 2026-11-24 041534" src="https://github.com/user-attachments/assets/e9a58430-5f57-4f17-a8c5-de29a4208bf6" />
   
3. The products with the longest shelf-life are Garlic, Banana, Rice Flour.
<img width="447" height="374" alt="Screenshot 2026-11-24 042000" src="https://github.com/user-attachments/assets/4cbf3139-64cd-4717-90cf-13edc331d164" />
   
4. The following products are most likely to run out of stock based on last reorder level. Rice flour, coconut, raw sugar, evaporated milk amongst others.
<img width="438" height="205" alt="Screenshot 2026-11-23 005052 - Copy" src="https://github.com/user-attachments/assets/53bd5e48-9987-478a-85ce-2e2924eb557e" />

5. The seasonal demand for different product categories is expected to be between 528 and -259. This indicates that a drop in demand would reduce sale by 259.
<img width="460" height="224" alt="Screenshot 2026-11-23 005052 - Copy - Copy" src="https://github.com/user-attachments/assets/e5e7fd3a-8d9a-4b91-ac3e-62613ac122e1" />

6. The optimal reorder level is 50% of the current reorder level.

   ## Recommendations
. Reorder quantity should be increased by 50% of the current reorder level.

## Conclusion
My conclusion is that good stock management helps the business reduce losses, satisfy customers and make more profit.






   









