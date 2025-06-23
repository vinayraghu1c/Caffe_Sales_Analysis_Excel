# ☕ Caffe Sales Analysis Dashboard - Excel Project

## Project Overview
This project presents a detailed **Sales Analysis Dashboard** for a coffee shop using **Microsoft Excel 2013**. The dashboard provides key business metrics such as total revenue, total orders, average spent per person, hourly/monthly/day-wise sales, location insights, and category-wise distributions.

Developed entirely in Excel with **Pivot Tables**, **Power Query**, and **Slicers**, this interactive dashboard allows business stakeholders to understand their sales trends and top-performing products quickly.

---

## Dataset Structure

The raw dataset contains the following columns:

| Column Name         | Description                                   |
|---------------------|-----------------------------------------------|
| `transaction_id`     | Unique ID for each transaction               |
| `transaction_date`   | Date of the transaction                      |
| `transaction_time`   | Time of the transaction                      |
| `transaction_qty`    | Quantity of product purchased                |
| `store_id`           | Unique ID of the store                       |
| `store_location`     | Physical store location                      |
| `product_id`         | Unique ID of the product                     |
| `unit_price`         | Price per unit of the product                |
| `product_category`   | Product category (e.g., Tea, Coffee, etc.)   |
| `product_type`       | Type of product                              |
| `product_detail`     | Additional product detail                    |

---

## Dataset Source

This dataset was sourced from Kaggle:

**[Coffee Sales Dataset on Kaggle](https://www.kaggle.com/datasets/ahmedabbas757/coffee-sales?select=Coffee+Shop+Sales.xlsx)**

---

## Data Cleaning and Transformation (Power Query)

Performed via **Power Query Editor** in Excel.

### 1. Removed Unwanted Data
- **Removed Null Values**: All rows with any null values in essential columns were removed.
- **Removed Duplicates**: Duplicate rows based on `transaction_id` and other identical columns were removed to ensure data consistency.

### 2. Column Transformations
Added the following new columns for better analysis and filtering:

- `Size`: Extracted from `product_detail` .
- `Hour`: Extracted from `transaction_time` using `Time.Hour()` to analyze **hourly sales**.
- `Month Name`: Extracted from `transaction_date` using `Date.MonthName()` for **monthly trend analysis**.
- `Day Name`: Extracted from `transaction_date` using `Date.DayOfWeekName()` for **day-wise breakdown**.
- `Day of Week`: Added using `Date.DayOfWeek()` to help sort weekday data properly in visuals.
- `Total Price`: Calculated using `transaction_qty * unit_price` to represent **revenue per transaction**.

---

## Dashboard Screenshot

Below is the snapshot of the final dashboard created in Excel:

![Dashboard Screenshot](https://github.com/vinayraghu1c/Caffe_Sales_Analysis_Excel/blob/main/Dashboard.png)

---

## Dashboard Features

### KPIs (Top Section)
- **Total Revenue**: `$698,812.33`
- **Total Orders**: `214,470`
- **Avg. Spent Per Person**: `$4.69`
- **Top Selling Product**: `Ethiopia`

### Visuals and Charts

- **Hourly Sales**: Line chart displaying sales by hour of the day.
- **Day-wise Sales**: Bar chart showing total orders by weekday.
- **Monthly Revenue**: Revenue trend across months.
- **Category-wise Sales Distribution**: Pie chart with sales share by product category.
- **Location-wise Sales**: Total sales across different store locations.
- **Top 6 Selling Products**: Bar chart of best-performing products.

### Interactivity
- Fully interactive with **slicers** for:
  - Day Name
  - Month Name

---

## Tools Used

| Tool | Purpose |
|------|---------|
| Microsoft Excel | Main dashboarding and calculations |
| Power Query | Data cleaning and transformation |
| Pivot Tables | Aggregations for visualizations |
| Slicers & Timeline | Interactivity and filtering |
| Custom Formatting | Themed styling for visuals |

---

## Project Insights

- **Most Revenue-Generating Month**: June
- **Busiest Hour**: Between 9 AM – 11 AM
- **Top Product**: Ethiopia
- **Top Category**: Coffee
- **Peak Weekdays**: Monday, Friday

---

##  Analysis By - **Vinay Raghuwanshi**  

Email - vinayraghuwanshi206@gmail.com

LinkedIn - https://www.linkedin.com/in/vinay-raghuwanshi

---
