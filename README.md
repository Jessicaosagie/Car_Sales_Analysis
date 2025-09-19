# 🚗 Car Sales Analysis

This project provides insights into car sales data using Excel (Pivot Tables & Charts), SQL, and Power BI.  
The dataset contains customer demographics, car specifications, dealer information, and sales performance across regions.

---

## 📑 Table of Contents
- [Dataset Overview](#-dataset-overview)
- [Tools Used](#-tools-used)
- [Key Insights](#-key-insights)
- [SQL Queries](#-sql-queries)
- [Visualization](#-visualization)
- [Author](#-author)

---

## 📊 Dataset Overview
- **Source:** [Car Sales Report – Kaggle](https://www.kaggle.com/datasets/missionjee/car-sales-report)  
- **Size:** 23,906 records  
- **Features:** Customer demographics, car details (company, model, engine, transmission, body style), dealer information, sales price, and region.  

### Sample Records (First 3 Transactions)

| Car_id       | Date     | Customer Name | Gender | Annual Income | Dealer_Name                           | Company  | Model     | Engine                       | Transmission | Color | Price ($) | Dealer_No  | Body Style | Phone   | Dealer_Region |
|--------------|----------|---------------|--------|---------------|----------------------------------------|----------|-----------|------------------------------|--------------|-------|-----------|------------|------------|---------|---------------|
| C_CND_000001 | 1/2/2022 | Geraldine     | Male   | 13,500        | Buddy Storbeck's Diesel Service Inc    | Ford     | Expedition| Double Overhead Camshaft     | Auto         | Black | 26,000    | 06457-3834 | SUV        | 8264678 | Middletown    |
| C_CND_000002 | 1/2/2022 | Gia           | Male   | 1,480,000     | C & M Motors Inc                       | Dodge    | Durango  | Double Overhead Camshaft     | Auto         | Black | 19,000    | 60504-7114 | SUV        | Aurora        |
| C_CND_000003 | 1/2/2022 | Gianna        | Male   | 1,035,000     | Capitol KIA                            | Cadillac | Eldorado | Overhead Camshaft            | Manual       | Red   | 31,500    | 38701-8047 | Passenger  | 7298798 | Greenville    |

---

## 🛠️ Tools Used
- **Excel** → Pivot Tables & Sales Charts  
- **SQL** → Querying and data analysis  
- **Power BI** → Interactive dashboards and advanced visuals  
- **GitHub** → Project documentation and portfolio showcase  

---

## 📌 Key Insights
- **Total Revenue:** $672M across all sales records.  
- **Top Performing Region:** Austin leads with **$117M in sales**.  
- **Best Selling Body Style:** SUVs dominate with **6,374 units sold**.  
- **Top 5 Locations by Revenue:** Austin, Janesville, Scottsdale, Aurora, and Pasco.  
- **Transmission Split:** Automatic cars contribute **$355M**, while manual cars generate **$316M**.  
- **Gender Insights:** Male customers purchased significantly more cars (**$527M vs $144M females**).  
- **Top Models:** Models "Huge", "Down", and "Explain" generated the highest sales.  
- **Car Colors:** Black and Pale White cars accounted for nearly **75% of total sales**.
  
---
## 📊 Visualizations  
  
### Charts  

<img width="646" height="251" alt="Pivot Table_Car Sales Report" src="https://github.com/user-attachments/assets/54748c6f-b903-424b-883f-f60d6a04c561" />

### Excel Pivot Tables 

---

## 💻 SQL Queries


```sql
---Total revenue by region---
SELECT Dealer_Region, SUM(Price) AS TotalRevenue
FROM car_sales
GROUP BY Dealer_Region
ORDER BY TotalRevenue DESC;
```

```sql
---Most popular car body style---
SELECT BodyStyle, COUNT(*) AS TotalSold
FROM car_sales
GROUP BY BodyStyle
ORDER BY TotalSold DESC;
```

```sql
---Revenue split by transmission type---
SELECT Transmission, SUM(Price) AS TotalRevenue
FROM car_sales
GROUP BY Transmission
ORDER BY TotalRevenue DESC;
```

---

## 🏷️ Author  

- **Name:** Jessica Osagie  
- **Email:** jessica.a.osagie@gmail.com   
- **LinkedIn:** [LinkedIn](https://linkedin.com/in/jessica-osagie/)  
