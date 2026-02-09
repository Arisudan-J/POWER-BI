📊 Supply Chain and Inventory Analysis (Power BI)

Preview:
<img width="1180" height="682" alt="Overview KPI" src="https://github.com/user-attachments/assets/d2f34b9f-2708-44e9-921a-5357fc6d71ed" />

📌 Project Overview
This project focuses on analyzing supply chain and inventory data to monitor stock health, identify inefficiencies, and support data-driven decision-making. Using Power BI, the dashboard provides actionable insights into stock levels, warehouse performance, inventory turnover, and slow-moving products.

The goal of this project is to help organizations reduce holding costs, avoid stockouts, and optimize reorder strategies through interactive visual analytics.

🎯 Objectives
- Identify products with stock levels below the reorder point
- Classify inventory into Low, Optimal, and Excess stock
- Analyze warehouse-wise stock shortages
- Measure inventory turnover to assess efficiency
- Detect slow-moving products using sales and inventory data
- Design an interactive dashboard to monitor overall stock health

📈 Key Features
- Interactive Power BI Dashboard with slicers for location, product type, SKU, and supplier
- Stock Status Classification using DAX logic
- Warehouse-wise Analysis to identify frequent shortages
- Sales vs Stock Analysis to detect slow and fast-moving products
- KPI Tracking including:
  - Average Stock
  - Total Revenue
  - Inventory Turnover
  - Low & Excess Stock Percentage
  - Lead Time Analysis

🛠 Tools & Technologies
- Power BI Desktop
-  DAX (Data Analysis Expressions)
- Data Modeling & Data Cleaning
- Supply Chain & Inventory Analytics

📊 DAX Measures Used
Stock Status Classification
DAX
Stock Status = 
SWITCH (
    TRUE(),
    'supply_chain_data'[Stock levels] < 'supply_chain_data'[Reorder Point], "Low",
    'supply_chain_data'[Stock levels] > 'supply_chain_data'[Max Stock Level], "Excess",
    "Optimal"
)
