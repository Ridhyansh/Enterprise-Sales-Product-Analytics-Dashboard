# 📊 Enterprise Sales & Product Analytics Dashboard

> A comprehensive data analytics project featuring SQL data cleaning, PowerBI visualization, and interactive dashboard creation using the AdventureWorks dataset.

[![SQL](https://img.shields.io/badge/SQL-Server-blue)](https://www.microsoft.com/sql-server)
[![PowerBI](https://img.shields.io/badge/PowerBI-Dashboard-yellow)](https://powerbi.microsoft.com/)
[![Status](https://img.shields.io/badge/Status-Completed-success)]()

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Project Features](#-project-features)
- [Technologies Used](#-technologies-used)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
- [Data Pipeline](#-data-pipeline)
- [Dashboard Pages](#-dashboard-pages)
- [Project Files](#-project-files)
- [Dataset Information](#-dataset-information)
- [Future Enhancements](#-future-enhancements)

---

## 🎯 Overview

This portfolio project demonstrates end-to-end data analytics capabilities, from raw data cleaning using SQL to creating interactive, multi-page dashboards in PowerBI. The project utilizes the AdventureWorks Data Warehouse dataset to analyze sales performance, customer behavior, and product metrics.

**Key Highlights:**
- ✅ SQL-based data cleaning and transformation
- ✅ Multi-dimensional data modeling
- ✅ Interactive 3-page PowerBI dashboard
- ✅ Static PDF export for reporting
- ✅ Comprehensive sales and product analytics

---

## ✨ Project Features

- **Data Cleaning & Transformation**: SQL queries to clean, sort, and export relevant columns
- **Data Modeling**: Star schema implementation with fact and dimension tables
- **Interactive Dashboards**: Three comprehensive pages covering different analytical perspectives
- **Export Capabilities**: PDF export for static reporting and stakeholder distribution
- **Professional Visualization**: Modern, user-friendly dashboard design

---

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| **Microsoft SQL Server** | Database management and data cleaning |
| **SQL Server Management Studio (SSMS)** | Database restoration and query execution |
| **PowerBI Desktop** | Data visualization and dashboard creation |
| **Power Query** | Data transformation and ETL processes |
| **Excel** | Budget data management |

---

## 📁 Project Structure

```
portfolio_1-sql_powerbi-main/
│
├── Data Tables/
│   ├── portfolio_1-data_table-DimCustomer.csv      # Customer dimension table
│   ├── portfolio_1-data_table-DimDate.csv          # Date dimension table
│   ├── portfolio_1-data_table-DimProduct.csv       # Product dimension table
│   ├── portfolio_1-data_table-FactInternetSales.csv # Sales fact table
│   └── portfolio_1-data_table-SalesBudget.xlsx     # Budget data
│
├── Analysis & Visualization/
│   ├── portfolio_1-project-analysis.sql            # SQL cleaning queries
│   ├── portfolio_1-project-visualization_powerbi.pbix # PowerBI dashboard
│   └── portfolio_1-project-visualization_pdf.pdf   # Static dashboard export
│
└── README.md                                       # Project documentation
```

---

## 🚀 Getting Started

### Prerequisites

- Microsoft SQL Server (2019 or later)
- SQL Server Management Studio (SSMS)
- PowerBI Desktop
- Microsoft Excel

### Dataset Setup

1. **Download the AdventureWorks Dataset**
   - Download the AdventureWorks Data Warehouse 2019 backup file:
     - **Direct Link**: [AdventureWorksDW2019.bak](https://github.com/Microsoft/sql-server-samples/releases/download/adventureworks/AdventureWorksDW2019.bak)
   - Original source: [Microsoft SQL Server Samples](https://github.com/Microsoft/sql-server-samples)

2. **Restore the Database**
   - Open SQL Server Management Studio
   - Restore the `.bak` file to create the AdventureWorksDW2019 database

3. **Update Dataset Dates** (Optional but Recommended)
   - Run the update script from TechTalkCorner to modernize date columns:
     - **Script**: [Update AdventureWorksDW Data](https://github.com/techtalkcorner/SampleDemoFiles/blob/master/Database/AdventureWorks/Update_AdventureWorksDW_Data.sql)

4. **Execute SQL Queries**
   - Open `portfolio_1-project-analysis.sql` in SSMS
   - Execute queries to clean and export data tables as CSV files

5. **Import to PowerBI**
   - Open PowerBI Desktop
   - Import the 4 CSV files and 1 Excel file
   - Open `portfolio_1-project-visualization_powerbi.pbix` to view the dashboard

---

## 🔄 Data Pipeline

### Step 1: SQL Data Cleaning
The SQL script (`portfolio_1-project-analysis.sql`) performs:
- Column selection and filtering
- Data sorting and organization
- Export to CSV format for PowerBI consumption

### Step 2: Data Modeling
In PowerBI, the data model is structured as a **star schema**:

![Data Model](https://user-images.githubusercontent.com/122973220/213426036-5aa569b0-9f8d-4b82-bbb2-2d242e2c7e09.jpg)

**Fact Table:**
- `FactInternetSales` - Sales transactions

**Dimension Tables:**
- `DimCustomer` - Customer information
- `DimDate` - Time dimension
- `DimProduct` - Product catalog
- `SalesBudget` - Budget targets

### Step 3: Power Query Transformation
- Column renaming for clarity
- Data type conversions
- Format standardization
- Calculated measures creation

### Step 4: Visualization
- Interactive dashboard creation
- Multi-page report design
- PDF export generation

---

## 📊 Dashboard Pages

### Page 1: AdventureWorks Sales Overview
A high-level executive dashboard providing key sales metrics and trends.

![Sales Overview Dashboard](https://user-images.githubusercontent.com/122973220/213424939-2e4614c7-28f2-4b25-9691-e53f7aa9f368.jpg)

**Key Metrics:**
- Total sales revenue
- Sales trends over time
- Regional performance
- Budget vs. actual comparisons

---

### Page 2: Sales by Customer
Detailed customer analytics and segmentation analysis.

![Sales by Customer Dashboard](https://user-images.githubusercontent.com/122973220/213426418-36348415-aa68-42e7-90a2-81b0306cd30f.jpg)

**Key Insights:**
- Top customers by revenue
- Customer segmentation
- Purchase patterns
- Customer lifetime value

---

### Page 3: Sales by Product
Product performance analysis and inventory insights.

![Sales by Product Dashboard](https://user-images.githubusercontent.com/122973220/213426517-39db89b9-88e1-4241-9844-bd65cfadb686.jpg)

**Key Metrics:**
- Product sales performance
- Category analysis
- Product trends
- Revenue by product line

---

## 📦 Project Files

### Analysis Files
- **`portfolio_1-project-analysis.sql`** - SQL queries for data cleaning and transformation

### Visualization Files
- **`portfolio_1-project-visualization_powerbi.pbix`** - Interactive PowerBI dashboard (requires PowerBI Desktop)
- **`portfolio_1-project-visualization_pdf.pdf`** - Static PDF export of the dashboard

### Data Files
- **`portfolio_1-data_table-DimCustomer.csv`** - Customer dimension data
- **`portfolio_1-data_table-DimDate.csv`** - Date dimension data
- **`portfolio_1-data_table-DimProduct.csv`** - Product dimension data
- **`portfolio_1-data_table-FactInternetSales.csv`** - Sales fact table
- **`portfolio_1-data_table-SalesBudget.xlsx`** - Budget and target data

> **Note**: The original AdventureWorks dataset (99 MB) exceeds GitHub's 25 MB file size limit and is not included in this repository. Please download it using the link provided in the [Getting Started](#-getting-started) section.

---

## 📚 Dataset Information

### AdventureWorks Data Warehouse
- **Version**: 2019
- **Source**: Microsoft SQL Server Samples
- **Size**: 99 MB (backup file)
- **Format**: `.bak` (SQL Server backup file)
- **License**: Microsoft Sample Database License

### Data Tables Used
1. **DimCustomer** - Customer demographics and information
2. **DimDate** - Calendar and time dimension
3. **DimProduct** - Product catalog and categories
4. **FactInternetSales** - Internet sales transactions
5. **SalesBudget** - Budget and forecast data

---

## 🔮 Future Enhancements

### Automation Pipeline (In Progress)
The goal is to create a fully automated analytics pipeline using Python:

**Planned Features:**
- 🔄 **Automated Data Extraction**: Pull data directly from database
- 🧹 **Automated Data Cleaning**: Python-based ETL processes
- 📊 **Automated Dashboard Generation**: Programmatic PowerBI report creation
- 📧 **Automated Reporting**: Scheduled PDF generation and email distribution
- ✅ **Quality Checks**: Automated validation and error detection

**Technology Stack (Planned):**
- Python (pandas, sqlalchemy, pyodbc)
- PowerBI REST API / Python SDK
- Email automation (smtplib, email libraries)
- Task scheduling (Windows Task Scheduler / cron)

**Target Completion**: End of 2023 (as of January 2023 resolution)

---

## 📝 Notes

- This project serves as a portfolio demonstration of SQL and PowerBI skills
- All data transformations are documented in the SQL script
- The PowerBI dashboard is fully interactive and can be customized
- PDF export provides a static version for presentations and reports

---

## 🤝 Contributing

This is a portfolio project, but suggestions and feedback are welcome!

---

## 📄 License

This project uses the AdventureWorks sample database, which is provided by Microsoft under their sample database license terms.

---

## 👤 Author

Portfolio Project - Data Analytics & Business Intelligence

---

**Last Updated**: 2023

---

*Built with ❤️ using SQL and PowerBI*
