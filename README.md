# Mens Clothing Inventory & Demand Analysis Dashboard

### Dashboard Link
Not publicly available (restricted Power BI access)

---

## Problem Statement

This dashboard analyzes men's clothing inventory, demand, and supply patterns to identify inefficiencies and optimize business performance.  

It helps businesses understand demand fluctuations, stock availability, and potential losses due to supply shortages.

---

## Steps followed 

- Step 1: Loaded dataset into Power BI Desktop (CSV file)

- Step 2: Opened Power Query Editor and enabled:
  - Column distribution  
  - Column quality  
  - Column profile  

- Step 3: Cleaned data and handled missing values

- Step 4: Created calculated measures for:
  - Profit/Loss  
  - Demand  
  - Availability  

- Step 5: Built KPI cards:
  - Total Profit  
  - Total Loss  
  - Average Daily Loss  
  - Average Demand per Day  
  - Average Availability per Day  
  - Total Supply Shortage  

- Step 6: Designed dashboard layout with modern UI

- Step 7: Published report to Power BI Service

---

## DAX Calculations


```DAX
Total Profit = SUM([Profit/Loss])
Total Loss = CALCULATE(SUM([Profit/Loss]), [Profit/Loss] < 0)
Average Demand = AVERAGE([demand])
Average Availability = AVERAGE([availability])
Supply Shortage = SUM([demand] - [availability])
```
--- 
## Snapshot of Dashboard
![Data Model](https://raw.githubusercontent.com/komalchoudhary1021-cmyk/Mens-Clothing-inventory-Project-2/main/Men'sshirt2.png)
## Report Pages
### Business Overview
![Dashboard](https://raw.githubusercontent.com/komalchoudhary1021-cmyk/Mens-Clothing-inventory-Project-2/main/Men'sshirt.png)
### Demand & Supply Analysis
![Demand & Supply](https://raw.githubusercontent.com/komalchoudhary1021-cmyk/Mens-Clothing-inventory-Project-2/main/Men'sshirt1.png)
## Insights

- **Profit & Loss Analysis**
  - Total loss significantly exceeds profit, indicating inefficiencies in inventory management  

- **Demand vs Availability**
  - Demand is higher than availability, leading to supply shortages  

- **Supply Shortage**
  - High shortage (~61K) indicates unmet customer demand  

- **Daily Metrics**
  - Average demand (~48.65) is higher than availability (~24.70)  
  - This gap results in consistent losses  
## Conclusion

This dashboard highlights major inefficiencies in inventory and supply chain management.

Businesses can use these insights to:

Improve stock planning
Reduce losses
Align supply with demand
Tools Used
Power BI
DAX
Data Modeling
Data Visualization
