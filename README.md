##🛍️ BrightPath Retail Data Analysis & Dashboard
---
### 📊 **Overview**

This project analyzes retail performance for a fictional company, BrightPath Consulting, using SQLite and Excel. The objective was to design a small-scale business intelligence system capable of transforming raw transactional data into actionable insights through SQL queries and interactive dashboards.

---

### ⚙️ **Tech Stack**

* **SQLite** – for database creation, data import, and SQL analysis
* **Excel** – for KPI visualization and dashboard design


---

### 🗂️ **Data Files**

| File           | Description                                                             |
| -------------- | ----------------------------------------------------------------------- |
| `stores.csv`   | Store details (StoreID, StoreName, Region, OpeningDate, ManagerID)      |
| `products.csv` | Product catalog (ProductID, ProductName, Category, UnitPrice)           |
| `sales.csv`    | Transactional data (SaleID, SaleDate, StoreID, ProductID, QuantitySold) |

All CSV files were imported into an SQLite database (`BrightPathRetail.db`) to build the analytical foundation.

---
### 🧠 **SQL Analysis Tasks**

1. **Q1 – Regional Store Listing:**
   Retrieve all stores located in the *West* region.
   → *Used to assess geographic distribution and coverage.*

2. **Q2 – High-Value Electronics:**
   List all *Electronics* products with unit price >\ $500.
   → *Identifies premium products contributing to revenue growth.*

3. **Q3 – Store Revenue Ranking:**
   Calculate total revenue per store (`SUM(QuantitySold × UnitPrice)`).
   → *Highlights top-performing stores for benchmarking.*

4. **Q4 – Top 5 Products by Revenue:**
   Rank products by total revenue across all stores.
   → *Reveals high-demand products for sales strategy optimization.*

5. **Q5 – Mature High-Sales Stores:**
   Find stores opened before 2020 that sold >\ 500 units.
   → *Identifies stable, long-term performers in the portfolio.*

---
### 📈 **Excel Dashboard Features**

**File:** `BrightPath_Dashboard.xlsx`

**Visual Components**

* **KPI Cards:** Total Revenue | Total Units Sold | Total Transactions
* **Monthly Revenue Trend** ( Line Chart )
* **Top 10 Products by Revenue** ( Horizontal Bar Chart )
* **Store Revenue Comparison** ( Column Chart )
* **Category Mix by Region** ( 100% Stacked Column Chart )

**Interactivity**

* 3 Slicers: *Region*, *Category*, *Month/Year* (filter all charts simultaneously)
* BrightPath warm color palette (`FFF8E1`, `F57C00`, `E65100`) for a cohesive, modern look

---

### 💡 **Key Insights**

* Stores H-33 and N-39 lead overall revenue generation.
* *Electronics Monitor 45* and *TV 44* are the top-grossing products.
* Mature stores opened before 2016 continue to perform strongly, suggesting loyal customer bases and efficient operations.

---

### 🚀 **How to Use**

1. Open **`BrightPathRetail.db`** in **DB Browser for SQLite**.
2. Run the SQL scripts under the *Execute SQL* tab.
3. Export the final combined dataset as `Combined_Sales_Data.csv`.
4. Open **`BrightPath_Dashboard.xlsx`** to explore the interactive dashboard.

---

### 🧭 **Learning Outcomes**

* Designing relational data models
* Writing analytical SQL queries (JOIN, GROUP BY, HAVING, ORDER BY)
* Building interactive KPI dashboards in Excel
* Applying storytelling design in data visualization

---

### 📌 **Future Improvements**

* Automate ETL process with Python (pandas + sqlite3)
* Deploy dashboard via Power BI or Tableau for web interactivity
* Integrate predictive sales forecasting

---

