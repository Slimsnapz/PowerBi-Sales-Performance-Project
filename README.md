# **Sales Performance Dashboard**

![Dashboard Screenshot]([Screenshot 2025-08-08 100750.jpg](https://github.com/Slimsnapz/PowerBi-Sales-Performance-Project/blob/02d827eb10570f6a153b4883c3b3670ad691f121/Screenshot%202025-08-08%20100750.jpg))  

https://github.com/Slimsnapz/PowerBi-Sales-Performance-Project/blob/7d0e75d60aaeb7feecfbe01d19db7cf06d86b7c6/Screenshot%202025-08-08%20132626.jpg
  
**Project Overview:**  
**Sales Performance Dashboard**

**Objective**  
Developed an interactive Power BI dashboard to analyze sales performance, identify trends, and extract actionable business insights from transactional data. The dashboard enables stakeholders to make data-driven decisions by visualizing revenue patterns, product performance, customer behavior, and sales dynamics across dimensions like time, location, and product categories.

---

## **Key Features & Analyses**

> **Charts used** (for quick reference):  
> - **Revenue Trend Analysis:** *Line chart*  
> - **Product Performance:** *Treemap*  
> - **Customer Segmentation:** *Stacked bar chart*  
> - **Total Revenue by Quarter & Category:** *Stacked column chart*  
> - **Weekday Sales Pattern:** *Scatter chart* (and alternate view with *stacked column chart*)  
> - **Revenue by Customer Location:** *Azure map*

### **Revenue Trend Analysis** *(Line chart)*
- Tracked revenue fluctuations over time (daily / monthly / quarterly) using an interactive **line chart** with trendlines and anomaly markers.
- Metrics shown: **Revenue**, **Units Sold**, moving averages, YOY / MOM growth rates.
- Visual interactions: hover tooltips, time-range slicer, and drill-through to specific dates/orders.

### **Product Performance** *(Treemap)*
- Ranked products by area and color using a **treemap** to surface top-selling SKUs at a glance.
- Metrics shown: **Revenue**, **Units Sold**.
- Drilldown: category → sub-category → product, with ability to filter other visuals by selection.

### **Customer Segmentation** *(Stacked bar chart)*
- Segmented customers by purchase frequency and total spend using a **stacked bar chart** to compare segments across locations or acquisition cohorts.
- Metrics shown: **Customer Count**, **Total Spend**, **Average Order Value (AOV)**, **Customer Lifetime Value (CLV)**.
- Built-in slicers: segment, acquisition date range, and region.

### **Total Revenue by Quarter & Category** *(Stacked column chart)*
- Visualized contribution of each product category across quarters with a **stacked column chart** for quick comparison of seasonal/category mix.
- Metrics shown: **Quarterly Revenue**, category shares (%), growth vs. prior quarter.

### **Weekday Sales Pattern** *(Scatter chart & Stacked column chart)*
- Primary view: **scatter chart** showing transactions (or aggregated points) across weekdays with size = Revenue per unit and y-axis = gross profit margin to find outliers and distribution.
- Alternate view: **stacked column chart** that aggregates revenue and units sold by weekday to highlight peak days.
- Metrics shown: **Revenue by Weekday**, **Units Sold**, weekend vs weekday lift.

### **Revenue by Customer Location** *(Azure map)*
- Geo-visualization using **Azure map** to show revenue density and average revenue per customer by region.
- Metrics shown: **Total Revenue**, **Revenue per Customer**, **Customer Count**, hotspots for expansion.
- Interactivity: zoom, cluster, and filter by product category or segment.

---

## **Data Sources**

- **Sales Data** (`sales_data.csv`):  
with fields: `Purchase Date`, `ProductID`, `CustomerCode`, `Order ID`, `Units Sold`, `Revenue`, `Cost of Goods Sold`.

- **Product Metadata** (`product.csv`):  
 with fields: `ProductID`, `Product`, `Category`.

- **Customer Metadata** (`customer.csv`):  
  with fields: `CustomerCode`, `Customer Name`, `Custome State`, `Customer City`, `Customer Zip Code`.

> The included datasets are sample CSVs used to populate the dashboard. Update or replace with your actual files while maintaining column compatibility for seamless refresh.

---

## **Technical Execution**

**Tools:**  
Power BI Desktop (Power Query, DAX), Azure Maps (visual), Excel (ad-hoc checks).

**Data Processing:**  
- Cleaned and preprocessed data: handled duplicates and missing values, normalized date fields, and standardized product/customer keys.  
- Created calculated metrics: **Profit** (`Revenue - COGS`), **Profit Margin**, **Customer Lifetime Value (CLV)**, **Average Order Value (AOV)**, weekday indicators, quarter/year flags.

**Data Modeling:**  
- Relationships:
  - `sales_data` ←→ `product` (many-to-one)
  - `sales_data` ←→ `customer` (many-to-one)  
- Ensured correct cardinality and filter directions for accurate aggregations across visuals.

**Visualizations & UX:**  
- Interactive elements: slicers (time, category, segment), KPI cards (Total Revenue, YoY Growth, Gross Profit), drill-through pages.  
- Tooltips enriched with contextual metrics (e.g., profit margin, CLV sample) for faster insights.

---

## **Key Insights Delivered**

- **Revenue Optimization:** Identified **higher sales on Mondays and Tuesdays**, prompting rescheduling of promotions and staffing for higher conversion opportunities.  
- **Product Strategy:** **Softdrinks**, **Tea**, **Alchohol** drives **89% of total revenue** — prioritize inventory and promotions here.   


---

---

## **GitHub Repository Contents**

