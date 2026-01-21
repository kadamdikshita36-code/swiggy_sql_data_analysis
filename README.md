# Swiggy SQL Data Analysis Project

## Project Overview
This is an end-to-end SQL data analysis project based on Swiggy food delivery data. 
The project focuses on data cleaning, data modeling using a star schema, and performing analytical queries to extract meaningful business insights.
I used SQL Server to transform raw csv data into a structured data warehouse and analyzed orders, revenue, restaurants, categories, and ratings.

---
## Tools Used
- SQL Server
-  SQL Server Management Studio (SSMS)
- GitHub

---
## Dataset
- **swiggy_raw_data.csv**
  This is the raw dataset containing order-level information such as:
  - Order date
  - Location
  - Restaurant
  - Category
  - Dish
  - Price
  - Ratings

---
## Data Architecture
The data model is designed using a **STAR SCHEMA** approach.

### Fact Table
- 'fact_swiggy_orders'

### Dimension Tables
- 'dim_date'
- 'dim_location'
- 'dim_restaurant'
- 'dim_category'
- 'dim_dish'

The ERD diagram for the star schema is available in:
- **ERD_star_schema.png**

---
## Data Cleaning & validation
- Checked for NULL values in important columns
- Identified blank and empty string values
- Ensured data consistency before creating dimension and fact tables

All data cleaning and validation logic is written in:
-**swiggy_sql_script**

---
## Analysis Performed
- Total number of orders
- Orders and revenue by city and location
- Top-performing restaurants based on order count
- category-wise demand analysis
- Rating count distribution

---
## Key Outcomes & Insights
- Identified cities with the highest number of Swiggy orders.
- Found top restaurants contributing the most to total orders.
- Analyzed which food categories are most popular among customers.
- Observed patterns between price,ratings, and order volume.
- Implemented a star schema to support efficient analytical queries.
