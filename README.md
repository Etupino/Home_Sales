# Home_Sales Challenge

# Overview
In this challenge, you'll apply your knowledge of SparkSQL to derive key metrics from home sales data. The tasks include creating temporary views, data partitioning, caching and uncaching temporary tables, and verification of table uncaching.

**Instructions**
1. File Renaming:

 * Rename the Home_Sales_starter_code.ipynb file as Home_Sales.ipynb.
2. Library Import:

 * Import the necessary PySpark SQL functions for this assignment.
3. Data Loading:

 * Read the home_sales_revised.csv data provided in the starter code into a Spark DataFrame.
4. Temporary Table Creation:

 * Create a temporary table called home_sales.
5. SparkSQL Queries:

 * Answer the following questions using SparkSQL:
    * What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.
    * What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.
    * What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.
    * What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query and round off your answer to two decimal places.
6. Caching:

 * Cache your temporary table home_sales.
 * Check if your temporary table is cached.
7. Cached Query:

 * Using the cached data, run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.
8. Partitioning:

 * Partition by the "date_built" field on the formatted parquet home sales data.
Create a temporary table for the parquet data.
9. Parquet Query:

 * Run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.
10. Uncaching:

 * Uncache the home_sales temporary table.
 * Verify that the home_sales temporary table is uncached using PySpark