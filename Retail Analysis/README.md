# Project Overview

This project performs an **end-to-end analysis of supermarket sales data** using **Power BI**.  
It covers the complete data analytics lifecycle, including **ETL**, **data modeling**, **business intelligence dashboards**, **exploratory data analysis (EDA)**.
The main objective is to extract **actionable insights** from retail data.

---

# Dataset Description

- **Records:** 9,800 sales transactions  
- **Granularity:** Each row represents one product sold within an order  

## Data Includes
- **Order Information:** Order ID, Order Date, Ship Date, Ship Mode  
- **Customer Information:** Customer Name, Segment, City, State, Region  
- **Product Information:** Category, Sub-Category, Product Name  
- **Sales:** Revenue per product  

---

## ETL Process (Power BI)

### Extraction
- Data loaded from an Excel file into **Power Query Editor**.

### Transformation
- Corrected data types across all columns  
- Fixed incorrect date formats (Order Date & Ship Date)  
- Replaced null values in **Postal Code** with `"Unknown"`  
- Created a **Row ID** column as a primary key  
- Applied **data normalization** to improve performance and modeling  

### Normalized Tables
- **Customers Table:** Customer details and location  
- **Products Table:** Category and product information  
- **Order Details Table:** Transactional data and sales  

### Load
- Cleaned and modeled data loaded into Power BI for analysis and reporting.

---

## DAX Measures & Calculated Columns

### Key DAX Measures
- Total Sales  
- Total Orders  
- Total Customers  
- Total Products  
- Average Shipping Duration  

### Calculated Columns
- Shipping Days  
- Year  
- Month  
- Quarter  

These columns enable **time-based analysis** and performance tracking.

---

# Exploratory Data Analysis (KNIME)

The following visualizations were created using KNIME:

- Category vs Sales (Pie Chart)  
- Sub-Category vs Total Sales (Bar Chart)  
- Order ID vs Sales (Scatter Plot)  
- Sales Distribution (Histogram)  
- Category vs Region (Heatmap)  
- Sales vs Segment (Density Plot)  

These visualizations helped identify **sales patterns**, **top-performing categories**, and **regional behavior**.

# Tools & Technologies

- **Power BI:** ETL, Data Modeling, DAX, Dashboards  
- **KNIME:** EDA, Visualization, Machine Learning  
- **Excel:** Data Source  
