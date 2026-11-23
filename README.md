# Grocery
Grocery Inventory dataset
## Description 
This project described and evaluated the inventory of a grocery store. it was sourced from kaggle.com. it comprises of 17 fields (columns) and 572 observations (row). it consisted of 5 unanswered questions meant to give data insights for future decision making. 
## Data cleaning 
Data cleaning was done using power query. simple text was done and irrelevant columns was removed.


## Procedures
The analysis was done using powerBi. Each question was answered using Data Analysis Expression (DAX).
Firstly, a date table was created from the date received field.
My_Date_table = CALENDAR(MIN('Grocery_Inventory new v1'[Date_Received]),MAX('Grocery_Inventory new v1'[Date_Received]))
the table was then marked as a date table and merged on the data model view using a 1-to-* relationship.
secondly, DAX table was created and various DAX measures added.

## Questions and findings 

1. What is the average stock quantity available per product category?
<img width="1154" height="663" alt="Screenshot 2026-11-23 004918" src="https://github.com/user-attachments/assets/46d06458-d1d3-438c-8d26-1d2e4f58ec35" />

3. Which suppliers contribute the most to total product inventory?
4. Which products have the longest shelf life before expiration, and how does that impact sales?
5. Which products are most likely to run out of stock based on last reorder levels? 
6. Can we predict seasonal demand for different product categories based on sales volume trends?
7. What are the optimal reorder levels for high-demand products to prevent stockouts? 

 
