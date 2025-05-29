
# 📚 Bookstore Sales Dashboard 

This interactive Tableau dashboard analyzes sales, inventory, and customer behavior for a fictional bookstore using data from BOOKS, CUSTOMERS, and ORDERS tables. It integrates KPIs, advanced visualizations, and calculated fields to provide business insights into revenue, best-sellers, customer segments, and stock availability.

---

## 📊 Dashboards & Key Insights

### 🔹 Sales & Orders Dashboard
- **Total Sales Revenue** – Overall revenue via `SUM(Amount)`
- **Total Orders** – `COUNTD(OrderID)` for unique orders
- **AOV (Average Order Value)** – `SUM(Amount) / COUNTD(OrderID)`
- **Monthly Orders** – Lollipop chart showing order seasonality
- **Actual vs Target Sales** – Bullet chart for goal tracking
- **Monthly Revenue Trend** – Dual-axis line and area chart

### 🔹 Books & Inventory Analysis
- **Top Genres** – Bar or pie chart for genre sales contribution
- **Best-Selling Authors** – Ranked bar chart by revenue
- **Stock Availability** – Bar chart highlighting low-stock items

### 🔹 Customer Analysis
- **Top N Customers by Country** – Bar chart showing revenue by region
- **Customer Segmentation** – Categorized into High, Medium, Low spenders
- **Returning vs New Customers** – KPI bars or comparison chart
- **Customer Locations** – Map showing unique customer count by city

---

## 🎯 KPIs and Calculated Fields

| **KPI / Field**              | **Formula**                                      |
|-----------------------------|--------------------------------------------------|
| Total Sales Revenue         | `SUM(Amount)`                                    |
| Total Orders                | `COUNTD(OrderID)`                                |
| Average Order Value (AOV)   | `SUM(Amount) / COUNTD(OrderID)`                  |
| Best-Selling Books          | `SUM(Quantity)` grouped by `[Title]`            |
| Stock Alert (Low Inventory) | `IF [Stock] < [Threshold] THEN "Low Stock"`     |
| Customer Segmentation       | `IF [Total Spend] > 500 THEN "High" ...`         |

---

## 📌 Sample Business Questions Answered

- ✅ Which genres and authors drive the most sales?
- ✅ What is the revenue trend across months and quarters?
- ✅ Are sales stronger on weekends vs weekdays?
- ✅ Which customers and regions generate the most revenue?
- ✅ How many customers are returning vs new?
- ✅ Which books need urgent restocking?

---

## 🧠 Tools & Techniques Used

- Tableau Desktop / Tableau Public
- KPI Cards, Bullet Charts, Box Plots, Dual-Axis Charts
- Filters, Set Actions, Parameters, Maps
- Calculated Fields for AOV, Segmentation, and Inventory
- Data from relational tables: BOOKS, CUSTOMERS, ORDERS

---

## 📁 Files Included

- `TABLEAU DASHBOARD.docx` – Full report with explanation
- `Bookstore_Dashboard.twbx` – Tableau workbook (optional)

---

