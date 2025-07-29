Superstore Sales Performance Dashboard (Excel) - Elevvo Pathways Internship Task 1

Overview

This project, completed as the first task for the Elevvo Pathways Data Analytics Internship (July 2025), creates a professional sales performance dashboard in Microsoft Excel using the Superstore Sales Dataset. The dashboard provides actionable business insights through data cleaning, pivot tables, charts, and key performance indicators (KPIs). It analyzes sales trends, category performance, regional contributions, and month-over-month (MoM) growth, demonstrating foundational data analytics skills.

Dataset





Source: Superstore Sales Dataset (super store sale (Recovered).xlsx)



Type: Retail transactional data



Fields:





Order Date, Ship Date, Ship Mode



Customer ID, Customer Name, Segment



City, State, Postal Code, Region



Product ID, Category, Sub-Category, Product Name



Sales, Quantity, Discount, Profit, Delivery Time



Records: 9,994 transactions from 2011 to 2014



Key Metrics:





Total Sales: $2,297,200.86



Total Profit: $286,397.02



Total Units Sold: 37,873



Average Profit Margin: 12.47%

Data Cleaning

The dataset was cleaned to ensure accuracy and reliability:





Duplicates: Removed duplicate rows to prevent data skew.



Blank Entries: Eliminated or imputed missing values where necessary.



Date Formatting: Standardized Order Date and Ship Date to proper date formats for time-based analysis.



Numeric Consistency: Corrected inconsistencies in numeric fields, such as negative profits caused by high discounts.



Month-Year Extraction: Added a Month-Year column derived from Order Date (e.g., Jan-2011) for trend analysis.

Excel Features Used







Feature



Purpose





Pivot Tables



Aggregated sales, profit, and quantity by Year, Month, Region, and Category.





Pivot Charts



Visualized monthly sales trends, category performance, and regional sales.





Slicers



Enabled interactive filtering by Region (e.g., West, East) and Category (e.g., Technology).





Formulas



Calculated KPIs like Total Sales, Total Profit, and MoM Growth %.





Conditional Formatting



Highlighted significant sales, profit margins, and growth rate variations.

Key Charts & Visuals

The dashboard includes the following visualizations:





Sales Trend by Month: Line chart displaying monthly sales trends from 2011 to 2014.



Sales by Category: Bar chart comparing sales across Furniture, Office Supplies, and Technology.



Sales by Region: Pie chart showing revenue distribution across South, West, Central, and East regions.



MoM Growth (%): Line chart illustrating month-over-month sales growth.



KPI Cards: Highlight Total Sales ($2,297,200.86), Best Month (November 2014: $349,120.07), and Highest MoM Growth (e.g., 94.08% from August to September 2014).

MoM Growth Calculation

Month-over-Month (MoM) Growth % was calculated using:

MoM Growth % = ((Current Month Sales - Previous Month Sales) / Previous Month Sales) * 100

Example:





August 2014 Sales: $159,589.45



September 2014 Sales: $309,770.10



MoM Growth: ((309,770.10 - 159,589.45) / 159,589.45) * 100 = 94.08%

Key Insights





Peak Sales Months: November 2014 ($349,120.07) and September 2014 ($309,770.10) recorded the highest sales.



MoM Growth: Significant growth observed in September 2014 (94.08%) and from February to March 2013 (231.16%).



Category Performance: Technology ($145,454.95 profit) and Office Supplies ($122,490.80 profit) outperformed Furniture ($18,451.27 profit).



Regional Contributions: West (e.g., California: $457,687.63) and East (e.g., New York: $310,876.27) were top revenue contributors.



Profit Margins: Technology had the highest profit margin (36.40%), followed by Office Supplies (31.30%), with Furniture at 32.30%.

Deliverables





Excel File: super store sale (Recovered).xlsx includes:





Cleaned transactional data in the Superstore sheet.



Pivot tables in the Pivot Table sheet for sales, profit, and quantity summaries.



Year-over-year and month-over-month analysis in the yoy&mom sheet.



Interactive dashboard with charts, slicers, and KPI cards in the Dashboard sheet.



Screenshot: A snapshot of the final dashboard (to be included in the repository).



Documentation: This README file outlining the project details.
