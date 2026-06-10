# 📊 Sales Revenue Dashboard

A fully interactive **Sales Revenue Dashboard** developed using **Microsoft Excel, Power Query, and Power Pivot** to analyze sales performance, monitor revenue trends, track order status, and support data-driven business decision-making through dynamic reporting and visualizations.

---

## 🔥 Project Highlights

- ✔ Cleaned and transformed **2,000+ sales records** using Power Query
- ✔ Performed data validation and quality checks on transactional data
- ✔ Developed interactive KPI dashboards for sales performance analysis
- ✔ Built DAX measures using Power Pivot for revenue reporting
- ✔ Analyzed product performance and regional sales trends
- ✔ Created order status and payment method reports
- ✔ Designed dynamic dashboards using Pivot Charts, Slicers, and Timelines

---

## 🧠 Skills & Tools Used

### 📌 Microsoft Excel
- Advanced Excel
- Pivot Tables
- Pivot Charts
- Conditional Formatting
- Dashboard Development
- Data Validation
- Timeline Filters
- Interactive Slicers

### 📌 Power Query
- Data Cleaning
- Remove Duplicates
- Data Transformation
- Handle Null Values
- Standardize Region Names
- Standardize Order Status Values
- Revenue Validation Checks

### 📌 Power Pivot
- Data Modeling
- DAX Measures
- KPI Calculations
- Relationship Management

### 📌 Sales Analytics
- Revenue Analysis
- Customer Analysis
- Product Performance Analysis
- Regional Sales Analysis
- Order Status Monitoring
- Payment Method Analysis

---

## 🗂 Dashboard Screenshot

 <img width="1473" height="677" alt="sales dashboard" src="https://github.com/user-attachments/assets/9de38b60-38f4-4ec9-b18e-d6b8cc54a2c3" />


---

## 📈 Dashboard Features

### ➤ Sales Overview
- Total Customers
- Total Orders
- Total Revenue
- Average Order Value (AOV)
- Cancellation Rate
- Return Rate

### ➤ Product Performance Analysis
- Top 5 Products by Revenue
- Revenue Contribution by Product

### ➤ Regional Analysis
- Revenue by Region
- Region-wise Performance Comparison

### ➤ Order Analysis
- Order Status Distribution
- Cancellation Analysis
- Return Analysis

### ➤ Customer & Salesperson Analysis
- Revenue by Salesperson
- Customer Insights

### ➤ Revenue Trends
- Revenue by Month
- Sales Trend Analysis

### ➤ Payment Analysis
- Payment Method Distribution
- Preferred Payment Channels

### ➤ Interactive Filters
- Region Slicer
- Product Slicer
- Order Status Slicer
- Year Filter
- Timeline Filter

---

## 📊 DAX Measures Used

### Total Revenue

```DAX
Total Revenue :=
SUM(Sales[Revenue])
```

### Total Orders

```DAX
Total Orders :=
DISTINCTCOUNT(Sales[Order ID])
```

### Total Customers

```DAX
Total Customers :=
DISTINCTCOUNT(Sales[Customer ID])
```

### Average Order Value (AOV)

```DAX
AOV :=
DIVIDE(
    [Total Revenue],
    [Total Orders]
)
```

### Cancellation Rate

```DAX
Cancellation Rate :=
DIVIDE(
    CALCULATE(
        COUNTROWS(Sales),
        Sales[Order Status] = "Cancelled"
    ),
    COUNTROWS(Sales)
)
```

### Return Rate

```DAX
Return Rate :=
DIVIDE(
    CALCULATE(
        COUNTROWS(Sales),
        Sales[Order Status] = "Returned"
    ),
    COUNTROWS(Sales)
)
```

---

## 🧩 Data Cleaning & Transformation Performed

- Removed duplicate Order IDs
- Standardized Region Names
- Standardized Order Status values
- Removed extra spaces using TRIM()
- Converted text into Proper Case
- Handled blank and null values
- Validated Revenue calculations
- Investigated negative quantities
- Created Month, Year, and Quarter columns
- Performed sales data quality checks

---

## 🗂 Dataset Information

The dataset contains **2,000 sales transaction records** with real-world data quality issues to simulate corporate sales reporting scenarios.

### Dataset Columns

- Order ID
- Order Date
- Customer ID
- Customer Name
- Product Name
- Category
- Region
- Salesperson
- Quantity
- Unit Price
- Revenue
- Order Status
- Payment Method

### Included Data Challenges

- Duplicate Order IDs
- Blank Values
- Inconsistent Region Names
- Inconsistent Order Status Values
- Extra Spaces in Text Fields
- Revenue Errors
- Negative Quantities

---

## 📂 Project Files

### 📁 Dashboard File
[Download Dashboard]([YOUR_EXCEL_DASHBOARD_LINK_HERE](https://github.com/bhagyashrininawe/Sales-Revenue-Dashboard-Excel/blob/main/Sales%20Revenue.xlsx))

### 📁 Dataset File
[Download Dataset]([YOUR_DATASET_LINK_HERE](https://github.com/bhagyashrininawe/Sales-Revenue-Dashboard-Excel/blob/main/Corporate_Messy_Dataset_2000_Rows.csv

))

---

## 🎯 Business Value

This dashboard enables organizations to:

- Monitor overall sales performance
- Analyze revenue trends and growth patterns
- Identify top-performing products
- Evaluate regional sales performance
- Track order fulfillment and returns
- Understand customer purchasing behavior
- Support strategic sales decision-making

---

## 📌 Key Insights

- Identified top-performing products contributing to overall revenue.
- Analyzed revenue distribution across different regions.
- Monitored cancellation and return trends.
- Evaluated salesperson performance using revenue metrics.
- Delivered actionable sales insights through interactive reporting.

---

## 🚀 Future Enhancements

- Sales Forecasting Analysis
- Customer Segmentation
- Profit Margin Analysis
- Inventory Integration
- Automated Monthly Reporting
