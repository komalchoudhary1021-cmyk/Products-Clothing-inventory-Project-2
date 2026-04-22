# Product's Inventory & Demand Analysis Dashboard

### Dashboard Link
Not publicly available (restricted Power BI access)

---

## Problem Statement

This dashboard analyzes Product's clothing inventory, demand, and supply patterns to identify inefficiencies and optimize business performance.  

It helps businesses understand demand fluctuations, stock availability, and potential losses due to supply shortages.

---

## Steps followed 

- **Step 1: Data Preparation using SQL**
  - Started with raw dataset in Microsoft SQL Server
  - Performed data cleaning and transformations (handling inconsistencies, formatting columns)
  - Created required views (EMV) using SQL Workbench for structured analysis

- **Step 2: Data Storage & Structuring**
  - Loaded the processed data into SQL Database
  - Ensured proper schema design and relationships
  - Verified data consistency and accuracy after transformations

- **Step 3: Connecting Power BI with SQL**
  - Installed SQL Server connector
  - Connected Power BI to SQL Database
  - Imported required tables and views into Power BI

- **Step 4: Data Modeling in Power BI**
  - Created relationships between tables
  - Built calculated columns and measures using DAX
  - Structured data model for efficient reporting

- **Step 5: Data Visualization**
  - Designed interactive dashboards using Power BI
  - Created key visuals:
    - KPI Cards (Profit, Loss, Demand, Availability)
    - Line Charts & Trend Analysis
    - Bar Charts for comparison
    - Slicers for filtering and interactivity

- **Step 6: Dashboard Design**
  - Applied modern UI layout and theme
  - Ensured clear data storytelling and readability
  - Organized visuals for business insights

- **Step 7: Deployment & Sharing**
  - Published report to Power BI Service
  - Created workspace for project management
  - Set up scheduled data refresh

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
