# Home_Sales

This project analyzes a dataset of home sales to answer several specific questions using PySpark and SQL queries. The data is processed and queried to uncover trends related to the characteristics and prices of homes sold.

# Data

The dataset home_sales_revised.csv is used for this analysis. It is read into a Spark DataFrame and a temporary table called home_sales is created for querying.

#Queries

The project answers the following questions using SparkSQL:

Average price for a four-bedroom house sold each year.
Average price of a home each year it was built, for homes with three bedrooms and three bathrooms.
Average price of a home each year it was built, for homes with three bedrooms, three bathrooms, two floors, and are at least 2,000 square feet.
Average price of a home per "view" rating for homes with an average price of at least $350,000.

# Performance Optimization

Caching: The temporary table home_sales is cached to optimize the performance of queries.
Partitioning: The dataset is partitioned by the "date_built" field to improve the efficiency of data processing.

# Analysis

After conducting the SQL queries, the runtime for each is noted to compare the performance between cached and uncached data states.

