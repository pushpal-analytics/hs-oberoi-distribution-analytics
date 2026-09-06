# Spirits Distribution Intelligence — Sales & Inventory Analytics

<p align="center">
  <img src="./Docs/Daily_MIS_Dashboard.png" alt="Spirits Distribution Daily MIS Dashboard" width="100%"/>
</p>

## Overview
Spirits beverage distributors face critical operational gaps that hinder smarter and faster decision-making:
* **Data Silos:** Sales data is scattered across multiple Excel sheets with no single source of truth.
* **Delayed Insights:** Decision-makers rely on outdated reports instead of real-time daily metrics.
* **Margin Leakage:** Lack of clear visibility into discount impacts, slow-moving inventory, and outlet profitability.

**Spirits Distribution Intelligence** is an enterprise-grade analytics solution designed to unify sales, inventory, and outlet performance into an automated Power BI dashboard system—helping business leaders eliminate manual reporting, protect net margins, and streamline inventory capital.

---

## Executive Presentation
A detailed 10-slide executive summary deck covering the business problem, star schema data engine, brand profitability, and inventory valuation is available in the documentation folder:

📁 **[View Presentation Deck (PDF)](./Docs/Spirits_Distribution_Intelligence_Case_Study.pdf)**

---

## Technical Architecture & Workflow
The data architecture is engineered for fast query speed, 100% data accuracy, and easy scalability across enterprise datasets.

* **Tech Stack Pipeline:** `Python` → `SQL Server` → `Power Query` → `Power BI`
* **Data Engine:** Automated ETL and cleaning routines using Power Query and SQL Server.
* **Data Modeling:** Modeled a Star Schema linking 1 central Fact Table to 4 Dimension Tables and a dedicated Measures table.
* **Interactivity:** Fully interactive dashboard eliminating all manual reporting workflows.

---

## Data Model (Star Schema)

<p align="center">
  <img src="./Docs/Star_Schema_Data_Model.png" alt="Spirits Distribution Star Schema Data Model" width="100%"/>
</p>

An optimized Star Schema was built inside Power BI to handle multi-dimensional analysis seamlessly:
* **Central Fact Table:** `Sales_Transactions` (tracks date, outlet_id, product_id, discount_amt, qty, and selling_price).
* **Dimension Tables:** 
  * `Product_Master` (brand_name, category, cost_price, product_id)
  * `Outlet_Master` (city, outlet_name, outlet_target)
  * `Date` (DayOfWeek, Month, MonthNum, MonthYear, Quarter, Year)
  * `Inventory_Report` (min_stock, product_id, warehouse_stock)
* **Calculated DAX Measures:** Centralized `Measures` table managing MTD Revenue, MTD Net Profit, Profit Margin %, Reorder Value, 7-Day Moving Averages, and Low Stock Alerts.

---

## Key Business Insights & Findings

1. **Daily MIS Snapshot:**
   * **MTD Performance:** Tracked **₹1.34M** MTD Revenue, **₹127.22K** Net Profit at a **10.28%** Profit Margin across **15K** total units sold.
   * **Executive Value:** Delivers a 360-degree daily health check in seconds for executive decision-makers.

2. **Brand Profitability & Discount Impact:**
   * **Margin Leakage:** Identified 4 high-revenue brands leaking net margins due to uncontrolled discounting exceeding 8%.
   * **Action Plan:** Enforce maximum discount caps per brand to safeguard overall profitability and protect the bottom line.

3. **Channel & Outlet Efficiency:**
   * **Top Retailer:** **Wine Shop K Block** generated the highest individual revenue (**₹83,080**).
   * **Channel Growth:** Retail outlets consistently outperform bar locations with a **+55% higher net profit margin**, signaling a clear focus for retail channel expansion.

4. **Warehouse Stock Health & Reorder Alerts:**
   * **Stock Alerts:** Identified **4 critical low-stock items** requiring **₹1.2L** in immediate reorder capital to prevent stock-outs.
   * **Capital Optimization:** Prevents working capital from getting locked in slow-moving inventory, freeing cash flow for high-turnover SKUs.

5. **Sales Patterns & Seasonality:**
   * **Trend Identified:** Mid-week sales (Mon–Thu) drop by **40%** compared to weekend demand surges.
   * **Action Plan:** Launch targeted mid-week promotional campaigns to smooth out demand and balance logistics inventory flow.

---

## Strategic Recommendations
* **Prioritize High-Margin Channels:** Shift field sales efforts toward retail outlets delivering 55% higher profit margins.
* **Enforce Discount Caps:** Set maximum 8% discount limits per brand to maintain target profit margins.
* **Automate Reorder Triggers:** Prevent stock-outs using automated low-stock alerts and automated reorder workflows.

---

## Author
**Pushpal Kawara**  
*Data Analyst & BI Specialist*

* **Email:** pushpalanalytics@gmail.com
