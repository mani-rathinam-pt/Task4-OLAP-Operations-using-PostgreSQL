# Sales Data Analysis - OLAP Operations

## Project Overview
A comprehensive OLAP (Online Analytical Processing) operations project using PostgreSQL/Redshift to analyze sales data through multiple dimensions. The system demonstrates advanced analytical capabilities including Drill Down, Rollup, Cube, Slice, and Dice operations for in-depth sales performance analysis.

## Database Structure

### Database
* **Database Name:** sales_database (PostgreSQL)
### Table

#### sales_sample
Stores sales transaction data across multiple dimensions.

**Columns:**
* `Product_Id` (Integer) - Product Identifier
* `Region` (Varchar(50)) - Sales Region (East, West, North, South, etc.)
* `Date` (Date) - Transaction Date
* `Sales_Amount` (Integer/Numeric) - Sales Revenue

## Features

### 1. Database Setup
* Created dedicated sales analytics database
* Designed dimensional sales table
* Implemented proper data types for analytical queries
* Structured data for OLAP operations

### 2. Data Entry
* Inserted 10 sample sales records
* Diverse data covering multiple products, regions, and dates
* Representative sales amounts for analysis
* Test data spanning different time periods

### 3. OLAP Operations

#### a) Drill Down
**Objective:** Analyze sales data at granular levels

* Drill down from Region to Product level
* Understand detailed sales performance
* Identify top-performing products within regions
* Analyze sales trends at the most detailed level

**Query Capability:**
* View sales broken down by Region and Product
* Examine individual product performance
* Identify best and worst performers

#### b) Rollup
**Objective:** Summarize data at higher aggregation levels

* Roll up from Product to Region level
* View total sales by region
* Aggregate product-level data for regional insights
* Hierarchical data summarization

**Query Capability:**
* Calculate total sales per region
* Compare regional performance
* Simplify complex product data into regional summaries

#### c) Cube
**Objective:** Multi-dimensional analysis

* Analyze sales across Product, Region, and Date simultaneously
* Create comprehensive data cube
* View all possible aggregation combinations
* Enable complex analytical queries

**Query Capability:**
* Generate subtotals for all dimension combinations
* Perform cross-dimensional analysis
* Create comprehensive summary reports
* Use GROUPING SETS or CUBE function

#### d) Slice
**Objective:** Extract specific data subsets

* Filter data by specific region
* Extract sales for particular date ranges
* View single-dimension snapshots
* Focus analysis on specific criteria

**Query Capability:**
* Sales for specific region (e.g., "East" region only)
* Sales within date range (e.g., Q1 2024)
* Filtered views for targeted analysis

#### e) Dice
**Objective:** Multi-criteria data extraction

* Extract data based on multiple conditions simultaneously
* View specific combinations of Product, Region, and Date
* Complex filtering for precise analysis
* Multi-dimensional data subsetting

**Query Capability:**
* Sales for specific products in specific regions
* Date range with region and product filters
* Complex WHERE clause combinations
* Precise analytical focus

## Technologies Used
* **Database:** PostgreSQL or Amazon Redshift
* **Language:** SQL
* **Analytical Method:** OLAP (Online Analytical Processing)

## Key SQL Concepts Demonstrated
* Database creation for analytical workloads
* Dimensional data modeling
* GROUP BY with multiple columns
* Aggregate functions (SUM, COUNT, AVG, MAX, MIN)
* GROUPING SETS for flexible aggregations
* ROLLUP for hierarchical summaries
* CUBE for multi-dimensional analysis
* WHERE clause for Slice operations
* Multiple AND/OR conditions for Dice operations
* Date filtering and range queries
* ORDER BY for result sorting
* Subqueries for complex analytics

## Project Files
* `OLAP Operations.sql` - Complete SQL code with all OLAP operations
* `output screenshots/` - Folder containing output images for all queries

## How to Use
1. Create the sales database using the provided script
2. Execute table creation statement for sales_sample
3. Insert sample sales data into the table
4. Run Drill Down queries to analyze detailed product-level sales
5. Execute Rollup queries for regional summaries
6. Perform Cube operations for multi-dimensional analysis
7. Use Slice queries to filter by specific dimensions
8. Apply Dice operations for complex multi-criteria filtering
9. Compare results across different OLAP operations
10. Generate comprehensive analytical reports

## Sample Query Categories

### Drill Down Queries
* Sales by Region and Product
* Detailed product performance within regions
* Granular time-based analysis

### Rollup Queries
* Total sales by Region
* Aggregate product sales
* Hierarchical summaries

### Cube Queries
* All combinations of Product, Region, Date
* Comprehensive subtotals
* Grand totals with intermediate summaries

### Slice Queries
* Sales for specific region
* Sales within date range
* Single-dimension filters

### Dice Queries
* Specific products in specific regions
* Date range with regional filter
* Multi-criteria combinations

## Learning Outcomes
* Understanding OLAP concepts and operations
* Implementing Drill Down for detailed analysis
* Performing Rollup for data summarization
* Creating data Cubes for multi-dimensional analysis
* Executing Slice operations for data subsetting
* Applying Dice operations for complex filtering
* Working with dimensional data models
* Using advanced GROUP BY features
* Writing complex analytical queries
* Generating business intelligence reports
* Comparing aggregation methods
* Optimizing queries for analytical workloads

## Business Applications
* Sales performance analysis
* Regional comparison and benchmarking
* Product performance evaluation
* Trend analysis over time
* Revenue forecasting support
* Strategic planning insights
* Market segmentation analysis
* KPI tracking and reporting

## Author
[MANIRATHINAM]

## Date
December 2025
