# AdventureWorks Sales Performance Dashboard

## **Project Overview**
This project involves the development of an interactive Power BI dashboard to analyze the sales performance of AdventureWorks Cycles, a fictional bicycle and accessories company. The primary goal was to transform raw sales data into actionable business intelligence, enabling stakeholders to track key metrics, identify trends, and make data-driven decisions to optimize sales strategy and customer engagement.

 ## Data Source & Description
Dataset: Microsoft's AdventureWorks sample database (Excel files).

 **Tables Used**: The data model likely integrates multiple tables, including:

* **Sales** (Order headers, details, returns)

* **Products** (Product categories, subcategories)

* **Customers** (Demographics, geographic location)

* **Calendar** (Date table for time intelligence)

# My Process & Technical Approach

## Data Acquisition & Cleaning:

* Acquired and loaded multiple Excel files from the AdventureWorks dataset into Power BI.

* Performed data cleaning and transformation in Power Query:

* Handled missing values, corrected data types, and standardized formats.

* Created calculated columns for necessary categorizations (e.g., Income Level groups).

## **Data Modeling:**

* Built a star-schema data model for optimal performance and simplicity.

* Established relationships between fact tables (e.g., Sales) and dimension tables (e.g., Products, Customers, Calendar).

* Created a dedicated Date table to enable robust time intelligence calculations.

**DAX & Measures:**

* Authored custom DAX measures to calculate core KPIs:

* Total Revenue = SUM(Sales[Sales Amount])

* Total Profit = SUM(Sales[Profit])

* Total Orders = DISTINCTCOUNT(Sales[Sales Order Number])

* Return Rate = DIVIDE([Total Returns], [Total Orders])

* **Time Intelligence:** Created measures for Month-over-Month (MoM) growth comparisons and rolling calculations.

## Visualization & Dashboard Design:

* Designed an intuitive and user-friendly layout with a logical flow of information.

* Used a combination of cards, line charts, bar charts, tables, and maps to present the data effectively.

* Implemented interactive elements (slicers, filters, cross-filtering) to enable self-service analysis and drill-down capabilities.

## Key Insights & Business Questions Answered

The dashboard provides insights into several critical business areas:

* **Overall Performance:** Track high-level KPIs like Total Revenue ($24.9M), Profit ($10.5M), and Orders (25.2K) at a glance.

* **Sales Trends:** Analyze revenue and order trends over time to identify seasonal patterns and growth.

* **Product Analysis:** Identify top-performing products (e.g., "Water Bottle - 30 oz." had 3,988 orders) and categories (Bikes and Accessories lead in volume).

* **Customer Analysis:** Understand customer value by analyzing revenue per customer and segmenting orders by customer income level and occupation.

* **Return Analysis:** Monitor return rates (2.2% overall) to identify potential product quality issues (e.g., Shorts have the highest return rate).

### How to Use / Interact with the Dashboard

* Download the .pbix file from this repository.

* Open it using Power BI Desktop (free to download from the Microsoft Store).

**Interact with the report:**

* Use the slicers (e.g., Region, Date) to filter the entire report.

* Click on any visual to cross-filter the other elements on the page (e.g., click on a product in the "Top Products" table to see its sales trend over time).

* Hover over data points to see detailed tooltips.

### **Future Enhancements**

* Incorporate inventory data to analyze stock levels and turnover rates.

* Build a customer cohort analysis to track retention and lifetime value (LTV).

* Add forecasting models to predict future sales trends directly within Power BI.

* Publish the report to the Power BI Service to enable automated refresh and sharing with stakeholders.

**Tools:** Power BI | Power Query | DAX | Data Modeling
