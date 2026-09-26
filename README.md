# Flipkart Sales Analysis – Power BI Dashboard

## 📊 Project Overview

This project is an interactive **Flipkart Sales Analysis Dashboard** developed in **Microsoft Power BI** to analyze retail sales performance, profitability, orders, product performance, customer segments, payment behavior, and sales distribution.

The dashboard provides a centralized view of key business KPIs and interactive visualizations so that users can monitor sales performance and explore customer and product-level trends.

---

## 🎯 Business Objective

The objective of this project is to provide a single interactive dashboard that helps stakeholders:

- Monitor total sales and profitability
- Track total orders and quantity sold
- Analyze monthly sales and profit trends
- Compare sales across product categories
- Identify the top-performing products
- Understand customer segment performance
- Analyze payment method usage
- Compare sales by gender
- Understand sales-channel performance
- Dynamically analyze the data using filters and slicers

---

## 📌 KPI Requirements

The dashboard contains the following key performance indicators:

| KPI | Business Purpose |
|---|---|
| **Total Orders** | Measures the total number of customer orders |
| **Total Sales** | Measures the overall revenue generated |
| **Total Profit** | Tracks overall profitability |
| **Total Quantity** | Measures the total units sold |
| **Profit Margin %** | Measures profitability relative to sales |
| **Total Customers** | Measures the customer base represented in the dataset |

---

## 📈 Visualization Requirements

### 1. Monthly Sales and Profit
**Chart Type:** Line Chart

Used to analyze monthly sales and profit trends and identify changes in performance over time.

**Measures:**
- Total Sales
- Total Profit

---

### 2. Sales by Category
**Chart Type:** Donut Chart

Used to compare sales contribution across product categories.

**Categories include:**
- Home Appliances
- Electronics
- Laptops
- Mobiles
- Home & Kitchen
- Fashion
- Sports
- Beauty
- Grocery
- Books

---

### 3. Customer Segment
**Chart Type:** Column Chart

Used to compare sales performance across different customer segments.

**Segments:**
- Regular
- New
- Premium

---

### 4. Payment Method
**Chart Type:** Donut / Pie Chart

Used to understand customer payment preferences.

**Payment methods include:**
- UPI
- Credit Card
- Debit Card
- Cash on Delivery
- Net Banking
- Wallet

---

### 5. Top 10 Products by Sales
**Chart Type:** Bar Chart

Used to identify the products generating the highest sales and highlight product-level performance.

---

### 6. Sales by Gender
**Chart Type:** Donut Chart

Used to understand how sales are distributed between male and female customers.

---

## 🎛️ Interactive Filters / Slicers

The dashboard provides interactive slicers that allow users to dynamically filter the analysis by:

- Year
- Month
- Category
- Gender
- Customer Segment
- Payment Mode
- Sales Channel

When a filter is selected, the KPI cards and visualizations update accordingly.

---

## ❓ Business Questions

The dashboard is designed to answer the following business questions:

1. What are the total sales generated?
2. What is the total profit generated?
3. How many orders have been placed?
4. How many units have been sold?
5. What is the current profit margin?
6. How many customers are represented in the data?
7. How are sales and profit changing month by month?
8. Which product categories generate the highest sales?
9. Which products are the top performers by sales?
10. Which customer segment generates the most sales?
11. Which payment methods are commonly used?
12. How are sales distributed by gender?
13. How does sales performance vary by sales channel?
14. How do KPIs and charts change when dashboard filters are selected?

---

## 🧮 Core Measures

The following measures are required for the dashboard:

### Total Orders
```DAX
Total Orders = DISTINCTCOUNT(Sales[Order_ID])
```

### Total Sales
```DAX
Total Sales = SUM(Sales[Sales])
```

### Total Profit
```DAX
Total Profit = SUM(Sales[Profit])
```

### Total Quantity
```DAX
Total Quantity = SUM(Sales[Quantity])
```

### Profit Margin %
```DAX
Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)
```

### Total Customers
```DAX
Total Customers = DISTINCTCOUNT(Sales[Customer_ID])
```

> Adjust table and column names if the source dataset uses different field names.

---

## 🗂️ Suggested GitHub Repository Structure

```text
Flipkart-Sales-Analysis-PowerBI/
│
├── README.md
│
├── PowerBI/
│   └── Flipkart_Sales_Analysis.pbix
│
├── Dataset/
│   └── Flipkart_Sales_Data.xlsx
│
├── Dashboard/
│   └── Flipkart_Sales_Dashboard.png
│
├── Documentation/
│   └── Business_Requirements.md
│
└── Screenshots/
    └── dashboard.png
```

---

## 🛠️ Tools & Technologies

- **Microsoft Power BI**
- **Power Query** – Data cleaning and transformation
- **DAX** – KPI and business measure calculations
- **Microsoft Excel** – Dataset/source data
- **GitHub** – Project documentation and version control

---

## 🔄 Project Workflow

```text
Raw Sales Data
      ↓
Data Cleaning & Transformation
      ↓
Data Modeling
      ↓
DAX Measures
      ↓
Interactive Visualizations
      ↓
Power BI Dashboard
      ↓
Business Insights
```

---

## 📊 Dashboard Components

The final dashboard includes:

- KPI Cards
- Monthly Sales & Profit Trend
- Sales by Category
- Customer Segment Analysis
- Payment Method Analysis
- Top 10 Products by Sales
- Sales by Gender
- Interactive Slicers
- Sales Channel Analysis

---

## 🎯 Expected Business Outcome

The dashboard provides stakeholders with a centralized interactive view of retail sales performance. It enables users to monitor KPIs, identify monthly trends, compare product categories and products, understand customer purchasing patterns, and evaluate payment and sales-channel behavior.

---

## 👤 Project Type

**Data Analytics / Business Intelligence Project**

**Domain:** Retail / E-commerce  
**Tool:** Microsoft Power BI  
**Dashboard:** Flipkart Sales Analysis

---

## 📷 Dashboard Preview

Add the dashboard screenshot to the repository and reference it here:

```markdown
![Flipkart Sales Analysis Dashboard](Dashboard/Flipkart_Sales_Dashboard.png)
```
