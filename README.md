# 🚗 Car Sales Analysis

## 📑 Table of Contents
- [📖 Overview](#-overview)
- [📊 Key Insights](#-key-insights)
- [🛠 Tools Used](#-tools-used)
- [🗃 Dataset](#-dataset)
- [📝 SQL Queries](#-sql-queries)
- [📈 Visualizations](#-visualizations)
- [🏷️ Author](#️-author)

---

## 📖 Overview
This project analyzes car sales data using Excel (Pivot Tables), SQL, and visualizations.  
The goal is to uncover insights on sales performance by **region, gender, car type, color, engine type, and year-over-year growth**.  

---

## 📊 Key Insights
- **Total Sales Revenue:** The dataset records **$672M** in total car sales.  
- **Top Region by Sales:** **Austin** leads with **$117M**, followed by **Janesville ($106M)**.  
- **Gender Contribution:** Males dominate car purchases with **$527M** in sales, compared to **$144M** from females.  
- **Popular Body Style:** **SUVs** generated the highest sales volume (**6,374 units**), followed by **Hatchbacks (6,128 units)**.  
- **Top Colors:** **Pale White (11,256 sales)** and **Black (7,857 sales)** are the most purchased colors.  
- **Average Price by Engine:** Cars with **Double Overhead Camshaft engines** had the highest average price at **$28,249**.  
- **Yearly Growth:** Sales grew from **$300M in 2022** to **$371M in 2023**, showing a strong upward trend.  

---

## 🛠 Tools Used
- **Excel** – Pivot tables and charts for sales breakdowns.  
- **SQL** – Querying, aggregating, and analyzing structured data.  
- **Power BI / Tableau (Optional)** – For interactive dashboards.  

---

## 🗃 Dataset
The dataset used for this analysis:  
🔗 [Car Sales Dataset (CSV)](./new%20car%20dataset.csv)  

---

## 📝 SQL Queries

### Total Revenue by Region
This query calculates the total revenue generated from each sales region.  
```sql
SELECT Dealer_Region, SUM("Price ($)") AS Total_Revenue
FROM car_sales
GROUP BY Dealer_Region
ORDER BY Total_Revenue DESC;
