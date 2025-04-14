# 🌿 DailyHarvest Sales and Inventory Analysis 📊

This repository contains a comprehensive Google Sheet-based solution for managing sales, inventory, and production planning across multiple regions for DailyHarvest. The system features automated data processing, forecasting, and visualization capabilities.. 📈


## Task 1: Master Data Consolidation 📝

1.  **Created "MasterData" Tab:** A new tab named "MasterData" was created in the spreadsheet. 📄
2.  **Transferred Sales Data:** Sales data for June and July from all four regions (Ajmer, Mandawa, Alwar, Tonk) were transferred into the "MasterData" tab. 🚚
3.  **Extracted Month:** The month was extracted from each sales record and added as a new column. 📅

## Task 2: Region-Wise Sales Analysis 🗺️

1.  **Created "RegionWise_Sales" Tab:** A new tab named "RegionWise_Sales" was created. 📊
2.  **Calculated Region-Wise Sales:** Region-wise sales for each product in each region were calculated. 💰
3.  **Forecasted August Sales:** August sales were forecasted using the growth rate from July. 🔮

## Task 3: Consolidated Sales Calculation 📈

1.  **Created "ConsolidatedSales" Tab:** A new tab named "ConsolidatedSales" was created. 📈
2.  **Calculated Consolidated Sales:** Consolidated sales for each product for each month were calculated using data from the "RegionWise_Sales" tab. ➕

## Task 4: Region-Wise Inventory Analysis 📦

1.  **Created "Region-wise Inventory" Tab:** A new tab named "Region-wise Inventory" was created. 📦
2.  **Calculated Inventory Metrics:** August forecast, August planned inventory, and July inventory were calculated for each product in each region. 🔢

## Task 5: Consolidated Inventory Calculation 📦

1.  **Created "Consolidated_Inventory" Tab:** A new tab named "Consolidated_Inventory" was created. 📦
2.  **Calculated Consolidated Inventory:** Consolidated inventory for each product was calculated. ➕

## Task 6: Importing August Sales Data 📥

1.  **Downloaded August Sales CSV Files:** August sales data for Ajmer, Mandawa, Alwar, and Tonk were downloaded from the provided Google Drive links. ⬇️

      Ajmer_August: https://drive.google.com/file/d/1ayo6m1YGlilXWForMHK2p-7sNJpFz7Vv/view
   
      Mandawa_August: https://drive.google.com/file/d/1Lc1eEGdqtdoBydXhxfL2Ngir89a4fS08/view
   
     Alwar_August:  https://drive.google.com/file/d/1h2D2dZS8e3CnYAOOVk2spfQrob9Q394M/view
  
     Tonk_August: https://drive.google.com/file/d/1fGxyTnMxrPAe91LgFrd0agr1ZiihFYbw/view
  
3.  **Imported Data:** The downloaded CSV files were imported into the existing spreadsheet, appending the August sales data to the respective region's existing data. 📥

## Task 7: Updating Region-Wise Sales with August Data 🔄

1.  **Updated "RegionWise_Sales" Tab:** The "RegionWise_Sales" tab was updated with the actual August sales data. ✅
2.  **Calculated August Actual Sales:** Actual August sales were calculated. 🔢
3.  **Calculated August Growth Rate:** The August growth rate was calculated. 📈
4.  **Forecasted September Sales:** September sales were forecasted using a weighted average method for recent trends and the average growth rate for stable trends. 🔮

## Task 8: Updating Consolidated Sales with August and September 🔄

1.  **Updated "ConsolidatedSales" Tab:** The "ConsolidatedSales" tab was updated with consolidated sales for August and September, using data from the "RegionWise_Sales" tab. ➕

## Task 9: Updating Region-Wise Inventory with September Data 🔄

1.  **Downloaded August Inventory CSV:** The August inventory data for PurePress Oils was downloaded from the provided Google Drive link.

      August_Inventory: https://drive.google.com/file/d/1GaW9rY8RVUkB2gI84vynqNd-obCp1DLk/view 
   
3.  **Created "InventoryDetails_August" Tab:** A new tab named "InventoryDetails_August" was created and the downloaded data was imported. 📥
4.  **Updated "Region-wise Inventory" Tab:** The "Region-wise Inventory" tab was updated with September inventory data from the "MasterData" tab. ✅
5.  **Applied Conditional Formatting:** 🎨
   
  🔴 Red: =August_Actual=0

🟡 Yellow: =AND(August_Actual>0, August_Actual<=0.5*August_Planned)

🟢 Green: =August_Actual>0.5*August_Planned
## Task 10: Updating Consolidated Inventory with August and September 🔄

1.  **Updated "Consolidated_Inventory" Tab:** The "Consolidated_Inventory" tab was updated with consolidated inventory for August and September, using data from the "Region-wise Inventory" tab. ➕

## Task 11: Region-Wise Production Plan 🏭

1.  **Created "Regionwise_ProductionPlan" Tab:** A new tab named "Regionwise_ProductionPlan" was created. 🏭
2.  **Calculated September Production Plan:** The production plan for September was calculated using data from the "RegionWise_Sales" and "Region-wise Inventory" tabs. 📝

## Task 12: Consolidated Production Plan 🏭

1.  **Created "Consolidated_ProductionPlan" Tab:** A new tab named "Consolidated_ProductionPlan" was created. 🏭
2.  **Calculated Consolidated September Production Plan:** The consolidated production plan for September was calculated using data from the "Regionwise_ProductionPlan" tab. ➕

## 🔍 Key Formulas Used

📍 Growth Rate Calculation: =(Current Month-Previous Month)/Previous Month

📍 Weighted Average Forecast: =0.5*Latest Growth + 0.3*Previous Growth + 0.2*Oldest Growth

📍 Inventory Planning: =Forecast + Safety Stock - Current Inventory

📍 Conditional Formatting: 
   =AND(August_Actual>0, August_Actual<=0.5*August_Planned)

## 📈 Business Insights
🔮 Forecasting Method: Hybrid approach combining:
   - Trend analysis when clear pattern exists
   - Weighted average for volatile products
   
📦 Inventory Strategy: 
   - Maintain 15-20% safety stock 
   - Color-coded monitoring system
   
🏭 Production Planning: 
   - Region-specific capacity constraints applied
   - Consolidated view for corporate planning



