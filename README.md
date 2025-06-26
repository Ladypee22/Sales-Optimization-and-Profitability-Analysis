# Sales-Optimization-and-Profitability-Analysis
A  Microsoft Power BI Project

 ##  Project Overview 
This project analyzes retail sales and shipping data using Power BI to uncover trends in product performance, customer segments, and delivery efficiency. The goal is to identify sales drivers, detect underperforming areas, and provide insights into improving profitability and operations. An interactive dashboard was built to support data-driven decision-making for stakeholders.

 ##  Problem Statement
The retail company has experienced fluctuating profit margins and rising operational costs despite consistent sales. Leadership suspects that certain customer segments, product categories, and shipping methods may be underperforming or even generating losses. They need a strategic, data-driven review to identify:

Where profits are leaking

Which products and customer segments are the most/least profitable

Whether logistics (shipping mode, delivery timing) are hurting revenue

How to optimize regional and category performance

 ## Data Source
Retail Sales  records was used in this analysis. The dataset was imported into power query as a csv file; a single sheet (Flat schema), The sheet includes the following column; Row ID, Order ID, Order date, Ship date, Ship mode, Customer ID, Customer name, Segment, Country, City, State, Postal Code, Region, Product ID, Category, Sub category, Product name, Sales.

 ## METHODOLOGY
### Here are my analysis

### 1. Data Profiling, cleaning and preparation**
Data profiling was conducted in Power Query to assess the dataset before analysis. The Column Quality, Column Distribution, and Column Profile features were used to understand the structure and content of each column.

Duplicate Values
A unique ID was created using the CONCAT() function to help identify duplicate rows.
Due to the dataset’s structure, the built-in "Remove Duplicates" feature in Power Query was not used. Instead, duplicates were manually identified and removed using the custom unique ID.

Blanks
The Column Quality feature showed that there were no blank cells or errors in any of the columns.

Standardization
Standardization was performed to ensure that all values within each column followed a consistent format across the dataset.

Data Types & Transformations
Data Types:
Appropriate data types were assigned to each column. For example:

Date columns (e.g., Order Date, Ship Date) were set to Date type.

Categorical columns (e.g., Region, Segment, Category) were set to Text type.

Numerical columns (e.g., Sales, Postal Code) were set to Decimal/Whole Number.

Transformations Applied:

Date columns were reformatted for consistency and to enable time-based analysis.

Text columns were trimmed and converted to lowercase where necessary to eliminate formatting inconsistencies.

Unnecessary columns (e.g., Row ID) were removed to improve data cleanliness.

### 2. Data Modelling
To enhance the effectiveness of the analysis, the dataset schema was restructured from a flat schema to a star schema, improving data integrity and minimizing redundancy.
