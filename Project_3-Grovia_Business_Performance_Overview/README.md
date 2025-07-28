# 🧾 Retail Sales & Customer Intelligence Dashboard (Power BI)

A comprehensive business intelligence dashboard designed for small retail businesses to transform raw sales data into actionable insights — covering sales trends, product performance, and customer behavior.

---

## 💡 Project Objective

To create a dynamic and insightful Power BI reporting solution that helps business owners:
- Monitor overall sales performance
- Understand customer demographics and buying behavior
- Identify high-performing products, categories, and stores
- Track seasonal trends and repeat purchase patterns

---

## 🛠️ Tools Used
- Power BI Desktop
- DAX (Data Analysis Expressions)
- Power Query (M Language)
- Data Modeling

---

## 📦 Data Sources
- `Customers.csv`
- `Products.csv`
- `Sales.csv`

---

## 🔄 Data Transformation Steps

1. **Data Loading**  
   Imported `Sales`, `Customers`, and `Products` tables into Power BI.

2. **Handling Missing Customer Info**  
   - Replaced blank `CustomerID` values in the Sales table with `"CASH001"`.
   - Created a new Cash Customer entry using `Enter Data`.
   - Appended this entry to the `Customers` table for proper linkage.

3. **Store Dimension Table Creation**  
   - Duplicated the Customers table.
   - Removed unnecessary columns.
   - Added new fields: `StoreID`, `Region`, `City`, `State`.
   - Converted `State` column to **Categorical** for Map visuals.

4. **Calendar Table**  
   Created using DAX for date-based analysis (Year, Month, Day, etc.).

5. **Model Relationships**  
   Established relationships between:
   - Sales ↔ Customers
   - Sales ↔ Products
   - Sales ↔ Calendar
   - Customers ↔ Stores

6. **Performance Tuning**  
   Disabled `Enable Load` on staging tables (e.g., Cash Customer Table) to optimize the model.

---

## 📊 Dashboard Pages & Visuals

### 📌 Page 1: Sales Overview

**KPIs**
- 🧮 Total Sales
- 📆 Avg. Sale per Day
- 💳 Total Transactions

**Visuals**
- Clustered Column Chart: Total Sales by Product
- Donut Chart: Total Sales by Store
- Area Chart: Monthly Sales Trend
- Line Chart: Sales Over Time

**Insights**  
Revenue trends, peak sales periods, and top-performing stores/products.

**Filters**: Date, Store, Category

---

### 📌 Page 2: Sales Analysis

**KPIs**
- 🧾 Total Transactions
- 👥 Unique Customers
- 🧺 Avg. Basket Size
- 🌟 Peak Sales Day

**Visuals**
- Line Chart: Sales by Month & Store
- Donut Chart: Sales by Product Category
- Column Chart: Transactions by Store

**Filters**: Date, Store, Products

---

### 📌 Page 3: Customer Insights

**KPIs**
- 👤 Unique Customers
- 🔁 Avg. Orders per Customer
- 💰 Avg. Revenue per Customer

**Visuals**
- Bar Chart: Top Spending Customers
- Donut Chart: Sales by Gender
- Column Chart: Unique Customers by Store
- Line Chart: Unique Customers over Time

**Insights**  
Customer loyalty, demographic patterns, repeat vs new buyers.

---

## ✅ Key Takeaways

- Designed for local retailers seeking clarity on sales and customer behavior.
- Cleaned, modeled, and visualized raw data into meaningful KPIs.
- Fully interactive with slicers for Date, Store, and Category filters.
- Business-friendly layout ready to be deployed and customized.

---

## 🧑‍💼 Suitable For

- Small business owners
- Retail managers
- Aspiring data analysts

---

## 📁 Folder Structure (Sample)

/Project_3-Grovia_Business_Performance_Overview

│

├── 📁 Data/

│ ├── customers.csv

│ ├── products.csv

│ └── sales.csv

│

├── 📁 Screenshots/

│ └── Report Page 1 - Executive Summary.JPG

│ └── Report Page 2 - Sales Analysis.JPG

│ └── Report Page 3 - Customer Insights.JPG

│

├── Grovia's Business Performance.pbix

└── README.md

---

## 🙋‍♂️ Author

**Chanush KR**  
🔗 [LinkedIn](https://www.linkedin.com/in/chanush-kr)  
🌐 [Portfolio Website](https://sites.google.com/view/chanushkr/home)  


| 💼 Aspiring Data Analyst & Power BI Consultant

---
