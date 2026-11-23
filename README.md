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
   The average stock quantity was done using
   Avg Stock Qty = AVERAGE('Grocery_Inventory new v1'[Stock_Quantity])
<img width="1154" height="663" alt="Screenshot 2026-11-23 004918" src="https://github.com/user-attachments/assets/46d06458-d1d3-438c-8d26-1d2e4f58ec35" />
Seafood has the highest average stock quantity, while grains had the lowest average stock quantity. since, grain are mainly consumened, it is recommended that subsequant suplies should be focused mainly on grains


2. Which suppliers contribute the most to total product inventory?
<img width="1157" height="635" alt="Screenshot 2026-11-23 005145" src="https://github.com/user-attachments/assets/af7b848d-4e54-4a31-adc5-467033346f4b" />
 Katz, twitterwire, meevee, quartz and feedfire are our most prominent suppliers.

3. Which products have the longest shelf life before expiration, and how does that impact sales?
<img width="1141" height="639" alt="Screenshot 2026-11-23 005052" src="https://github.com/user-attachments/assets/a53a5517-5115-4d3c-8606-4a32a992a3e7" />
The business should focus on buying the right products in the right quantities, checking expiration dates, monitoring sales, and reducing expired and excess stock.

4. Which products are most likely to run out of stock based on last reorder levels?
   <img width="441" height="374" alt="Screenshot 2026-11-23 005052" src="https://github.com/user-attachments/assets/7f4e1e2c-bb2c-4585-bc8b-34b2f41b3524" />
Reorder quantities should be determined by actual sales, customer demand, product shelf life, and supplier delivery time, Rather than applying a uniform 30% This will help maintain sufficient stocks, reduced products expired products and prevent unnecessary purchases.

   
5. Can we predict seasonal demand for different product categories based on sales volume trends?
  <img width="460" height="224" alt="Screenshot 2026-11-23 005052 - Copy - Copy" src="https://github.com/user-attachments/assets/ca27418c-85cd-457d-b60d-65c8dd898d57" />


   
6. What are the optimal reorder levels for high-demand products to prevent stockouts?
    Reorder for high demand stock should be 50%

 
