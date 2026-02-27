# supply-chain-analytics-dashboard
End-to-end Supply Chain Analytics Dashboard built using Power BI


Project Overview

This project presents a comprehensive Supply Chain Analytics Dashboard built using Power BI.
It analyzes demand performance, inventory efficiency, logistics reliability, and supplier performance to support data-driven operational and working capital decisions.

The dashboard provides end-to-end visibility across:
•	Order & Demand Performance
•	Inventory Optimization
•	Logistics & Delivery Efficiency
•	Supplier Performance Monitoring

Business Objectives
•	Monitor service level using Fill Rate & OTIF
•	Optimize inventory using Turnover & DIO
•	Reduce stockout risk
•	Improve logistics efficiency
•	Evaluate supplier reliability and performance
•	Identify working capital optimization opportunities

Dashboard Pages

Order & Demand Analysis
Focus: Demand trends & service performance
KPIs:
•	Total Orders
•	Total Order Quantity
•	Fill Rate %
•	Order Cycle Time
Insights Generated:
•	Demand concentration by product
•	Customer backlog analysis
•	Month-over-Month service level tracking
•	Category demand volatility (Electronics vs Semiconductor)

Inventory Analysis
Focus: Working capital & stock health
KPIs:
•	Inventory Value
•	Inventory Turnover
•	Days Inventory Outstanding (DIO)
•	Stockout Rate %
Key Analytics:
•	Inventory Value contribution % by product
•	ABC Classification (A/B/C segmentation)
•	Closing stock trend analysis
•	Open Orders vs Available Inventory comparison
Business Insights:
•	Low turnover indicates overstocking
•	High DIO suggests capital lock-up
•	Inventory concentration risk in A-class SKUs

Logistics & Delivery Analysis
Focus: Delivery efficiency & delay monitoring
KPIs:
•	Average Delivery Delay
•	On-Time Delivery %
•	Order Cycle Time
Technical Implementation:
•	Used AVERAGEX with context transition
•	Time intelligence using DATEADD
•	Delay calculation using promised date logic
Business Insights:
•	Identified delivery variability
•	Measured service level consistency
•	Detected potential SLA breach risks

Supplier Performance Analysis
Focus: Supplier reliability & procurement efficiency
KPIs:
•	Supplier Spend
•	OTIF (On-Time In-Full)
•	Supplier Fill Rate
•	Supplier-wise Delay %
Technical Highlights:
•	Used bridge table for supplier-product relationship
•	Managed filter propagation issues
•	Implemented contribution % using ALL
•	Corrected aggregation errors due to context flow
Business Insights:
•	Identified high-spend suppliers
•	Evaluated supplier performance risk
•	Highlighted supplier concentration risk

Technical Implementation

Data Modeling
•	Designed Star Schema
•	Built separate Date Table
•	Managed many-to-many relationships via bridge table
•	Optimized cross-filter direction

Advanced DAX Used
•	CALCULATE & Context Transition
•	SUMX, AVERAGEX (Iterators)
•	ALL, VALUES (Filter manipulation)
•	DATEADD (Time intelligence)
•	DATEDIFF (Period calculation)
•	DIVIDE (Safe calculations)
•	ABC Classification logic

Key Performance Highlights
•	Fill Rate ~88% (below industry benchmark of 95%)
•	Inventory Turnover = 66.6
•	DIO ≈ 2.83
•	Stockout Rate = 0.4% (high availability but possible overstocking)
•	Supplier performance variability observed

Business Impact
This dashboard enables:
•	Working capital optimization
•	Inventory reduction strategy
•	Service level improvement
•	Supplier risk monitoring
•	Logistics performance evaluation
•	Data-driven operational decisions

Tools & Technologies
•	Power BI Desktop
•	Power Query
•	DAX
•	Data Modeling (Star Schema)
•	Excel

Author
Priya Christina
Power BI | DAX | Supply Chain Analytics<img width="1343" height="751" alt="Order_Demand Analysis Screenshot" src="https://github.com/user-attachments/assets/c3197b88-e797-48ef-a00c-ca5953ff299a" />
<img width="1332" height="746" alt="Logistics Analysis Screenshot" src="https://github.com/user-attachments/assets/5635ddfc-e27e-4006-bb70-eb2326fb1a9f" />
<img width="1325" height="748" alt="Supplier Analysis Screenshot" src="https://github.com/user-attachments/assets/43362dc7-6d72-4117-a971-a0c4343f289b" />
<img width="1346" height="748" alt="Data Quality Screenshot" src="https://github.com/user-attachments/assets/ec07b0a4-6e4b-474f-9e09-260ccf8e7b64" />
<img width="1341" height="747" alt="Inventory Analysis" src="https://github.com/user-attachments/assets/538963ab-ee1f-4458-876b-104a31c2f579" />

