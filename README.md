# **Sales Performance Dashboard**

**Project Overview:**  
**Sales Performance Dashboard**

**Objective**  
Developed an interactive Power BI dashboard to analyze sales performance, identify trends, and extract actionable business insights from transactional data. The dashboard enables stakeholders to make data-driven decisions by visualizing revenue patterns, product performance, customer behavior, and sales dynamics across dimensions like time, location, and product categories.

---

## **Key Features & Analyses**

### **Revenue Trend Analysis**
- Tracked revenue fluctuations over time (daily/monthly/quarterly).
- Identified growth patterns, seasonal peaks, and anomalies.

### **Product Performance**
- Ranked products by **revenue**, **units sold**, and **profitability**.
- Highlighted top-performing and underperforming products using metrics like **profit margin**.

### **Customer Segmentation**
- Segmented customers by purchase frequency, total spend, and location.
- Identified **high-value customers** for targeted marketing.

### **Total Revenue by Quarter & Category**
- Visualized revenue distribution across product categories per quarter.
- Compared category performance to optimize inventory and promotions.

### **Weekday Sales Pattern**
- Analyzed sales volume and revenue by day of the week.
- Revealed peak sales days to align staffing and marketing efforts.

### **Revenue by Customer Location**
- Mapped revenue contributions geographically.
- Pinpointed high-potential regions for business expansion.

---

## **Data Sources**

- **Sales Data** (`sales_data.csv`):  
  1,000+ transactions with fields: `Purchase Date`, `ProductID`, `CustomerCode`, `Order ID`, `Units Sold`, `Revenue`, `Cost of Goods Sold`.

- **Product Metadata** (`product.csv`):  
  Product details (e.g., category, name, price tier).

- **Customer Metadata** (`customer.csv`):  
  Customer attributes (e.g., location, segment, acquisition date).

---

## **Technical Execution**

**Tools:**  
Power BI (DAX, Power Query), Excel.

**Data Processing:**  
Cleansed data (handled duplicates, missing values, date formatting). Created calculated metrics (e.g., **profit**, **profit margin**, **customer lifetime value**).

**Data Modeling:**  
Established relationships between `sales_data`, `product`, and `customer` tables.

**Visualizations:**  
Interactive charts (line, bar, maps), matrices, slicers, and KPI cards. Dynamic filters for time, product category, and customer segments.

---

## **Key Insights Delivered**

- **Revenue Optimization:** Identified **20% higher sales on weekends**, prompting shift in promotional scheduling.  
- **Product Strategy:** Revealed **Category B** as the top revenue driver (**35% of total sales**).  
- **Customer Insights:** **Top 10% of customers contributed 45%** of revenue, highlighting VIP potential.  
- **Geographic Opportunities:** **Northeast region generated 30% higher revenue per customer** vs. national average.

---

## **Why This Matters to Employers**

- **Business Impact:** Demonstrates ability to translate raw data into strategic insights that drive revenue growth and operational efficiency.  
- **Technical Proficiency:** Showcases expertise in Power BI, data modeling, DAX, and dashboard design.  
- **Problem-Solving:** Proves capability to handle end-to-end analytics projects—from data cleaning to stakeholder-ready visualizations.  
- **Domain Knowledge:** Highlights understanding of sales analytics, customer behavior, and inventory optimization.

---

## **GitHub Repository Contents**

- Power BI File: `Sales_Performance_Dashboard.pbix` (interactive report).  
- Datasets: `sales_data.csv` (provided), `product.csv`, `customer.csv`.  
- Documentation: `README.md` with setup instructions and analysis summary.  
- Screenshots of key dashboard views.

