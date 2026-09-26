# Requirements – Flipkart Data Analysis Power BI

## Software Requirements
- Microsoft Power BI Desktop
- Microsoft Excel
- Power Query (included with Power BI)
- GitHub (for project hosting/documentation)

## File Requirements
- Power BI project file: `flipcart_data_analysis.pbix`
- Source dataset: Flipkart-style e-commerce Excel dataset (`.xlsx`)
- Dashboard screenshots (`.png` or `.jpg`) – optional
- Project documentation (`.docx` or `.pdf`) – recommended

## Technical Requirements
- Windows PC capable of running Power BI Desktop
- Minimum 4 GB RAM; 8 GB or more recommended
- Internet connection for downloading/installing Power BI and optional GitHub publishing
- Sufficient storage for the PBIX file and dataset

## Power BI Skills Used
- Power Query data cleaning and transformation
- Data modeling and relationships
- DAX measures
- KPI creation
- Interactive visualizations
- Slicers and filters
- Drill/filter interactions
- Dashboard design

## Main Data Fields
Typical fields used in the project include:
- Order ID
- Customer ID
- Product ID
- Product Name
- Category
- Sub-Category
- Region
- State
- City
- Order Date
- Quantity
- Sales
- Cost
- Profit
- Discount
- Payment Method
- Order Status

## Recommended DAX Measures
```DAX
Total Sales = SUM(Sales[Sales])

Total Profit = SUM(Sales[Profit])

Total Orders = DISTINCTCOUNT(Sales[Order_ID])

Total Quantity = SUM(Sales[Quantity])

Average Order Value =
DIVIDE([Total Sales], [Total Orders])

Profit Margin =
DIVIDE([Total Profit], [Total Sales])
```

## Repository Structure

```text
Flipkart-Data-Analysis/
├── flipcart_data_analysis.pbix
├── README.md
├── requirements.md
├── Flipkart_PowerBI_Project_Documentation.docx
├── dataset/
│   └── Flipkart_Dataset.xlsx
└── screenshots/
    └── dashboard.png
```

## Notes
This project uses a simulated Flipkart-style dataset for educational and portfolio purposes. It is not an official Flipkart internal dataset.
