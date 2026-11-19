# 🍕 Pizza Sales Dashboard (Excel)

An interactive Excel dashboard that analyzes pizza sales for 2015 using PivotTables, PivotCharts, Slicers and a Timeline, covering sales, orders, customers, product performance and ordering patterns.

---

## 📌 Project Overview

This project turns raw pizza order data into a clean, interactive dashboard. The goal is to answer key business questions:

- How much did we sell, and how many orders and customers did we serve?
- Which months and days of the week are the busiest?
- Which pizza sizes and categories drive the most sales?
- Which pizzas are the best and worst sellers?

## 📂 Workbook Structure

| Sheet | Purpose |
|---|---|
| **Data** | Raw pizza sales data (orders, dates, pizza name, size, category, quantity, price) |
| **Pivot Table** | All PivotTables that feed the dashboard, plus the KPI cells |
| **Dashboard** | Final visual layer: KPI cards, PivotCharts, Slicers and Timeline |

---

## 🧮 Pivot Tables

![Pivot Tables](images/Pizza-Sales-Pivot.png)

| # | Pivot Table | Fields Used | What It Shows |
|---|---|---|---|
| 1 | **Monthly Orders** | Month → Count of Sales | Order volume per month (Jan–Dec) |
| 2 | **Orders by Day of Week** | Day → Count of Sales | Which weekdays are busiest |
| 3 | **Sales by Pizza Size** | Pizza Size → Sum of Sales (% of total) | Share of sales for S, M, L, XL |
| 4 | **Sales by Pizza Category** | Pizza Category → Sum of Sales (% of total, sorted) | Share of sales for Veggie, Classic, Supreme, Chicken |
| 5 | **Top 5 Best-Selling Pizzas** | Pizza Name → Sum of Sales (Top 5 filter) | The five highest-selling pizzas |
| 6 | **Bottom 5 Least-Selling Pizzas** | Pizza Name → Sum of Sales (Bottom 5 filter) | The five lowest-selling pizzas |

**KPI cells** (also in the Pivot Table sheet):

| KPI | Value |
|---|---|
| Total Sales | 8,436 |
| Total Orders | 499 |
| Total Customers | 499 |
| Total Quantity | 511 |

---

## 📊 Dashboard

![Pizza Sales Dashboard](images/Pizza-Sales-Dashboard.jpg)

### KPI Header
Four cards at the top show **Total Sales ($8,436)**, **Total Quantities (511)**, **Total Customers (499)** and **Total Orders (499)**.

### Charts

| Chart | Type | Insight |
|---|---|---|
| **Monthly Orders Trend** | Line | Orders were lowest in March (30) and peaked in June (54) |
| **Total Sales / Pizza Size** | Pie | Large pizzas lead with **47%**, then M (27%), S (22%), XL (3%) |
| **Top 5 Best-Selling** | Bar | Classic Deluxe (459), Four Cheese (433), Thai Chicken (429), Greek (402), Barbecue Chicken (384) |
| **Annual Orders by Day of Week** | Column | **Friday** leads with 91 orders; **Wednesday** is the weakest with 48 |
| **Sales Distribution by Category** | Donut | Veggie is trending at **28%**, followed by Classic 27%, Supreme 24%, Chicken 21% |
| **Bottom 5 Least-Selling** | Bar | Calabrese (167), Pepperoni, Mushroom & Peppers (123), Chicken Alfredo (88), Spinach Supreme (75), Brie Carre (47) |

### Interactive Filters
- **Slicers:** Pizza Size and Pizza Category
- **Timeline:** Order Date (filter by month)

All charts and KPIs are connected to the slicers, so the whole dashboard updates with one click.

---

## 🔍 Key Insights

1. **Friday is the busiest day** (91 orders), while **Wednesday is the slowest** (48).
2. **Large (L) pizzas generate almost half of all sales** (47%); XL contributes only 3%.
3. **Veggie is the top category** (28%), slightly ahead of Classic (27%).
4. **Classic Deluxe Pizza** is the best seller (459); **Brie Carre Pizza** is the weakest (47).
5. Order volume rises from **April to June**, then declines toward November.

## 💡 Recommendations

- Run promotions on **Wednesdays** to lift the weakest day.
- Staff and prepare more inventory for **Fridays and Saturdays**.
- Review or retire the **bottom 5 pizzas**, or rebrand and promote them.
- Look at pricing and promotion for **XL** pizzas, which have very low share.

---

## 🛠️ Tools & Features Used

- Microsoft Excel
- PivotTables and PivotCharts
- Slicers and Timeline
- Top 10 / Bottom 10 value filters
- Custom dashboard layout and formatting (KPI cards, themed colors)

## 📁 Repository Structure

```
pizza-sales-dashboard/
├── Pizza_Sales_Analysis.xlsx   # Excel workbook (Data, Pivot Table, Dashboard)
├── images/
│   ├── pivot-tables.png        # Pivot tables screenshot
│   └── dashboard.jpg           # Dashboard screenshot
└── README.md
```

## ▶️ How to Use

1. Download `Pizza_Sales_Analysis.xlsx`.
2. Open it in Microsoft Excel (2013 or later, needed for Slicers and Timeline).
3. Go to the **Dashboard** sheet and use the filters to explore the data.

---

⭐ If you find this project useful, give it a star!
