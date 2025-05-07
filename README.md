# Home Sales Analysis with PySpark

## Overview

In the final challenge of the course, we used PySpark and SparkSQL in Google Colab to analyze real estate sales data. The goal is to calculate key metrics, optimize query performance, and explore techniques such as caching and partitioning in Spark for optimization.

---

## Technologies Used

- Python 3
- PySpark
- Spark SQL
- Google Colab
- AWS S3 (for data source)

---

## Data Source

- **home_sales_revised.csv**
  - Hosted on AWS S3
  - Loaded using `SparkFiles`

---

## Objectives

1. **Load and Explore Data**
   - Use Spark to read a CSV file from an S3 bucket.
   - Convert the DataFrame into a temporary SQL view.

2. **SQL-Based Analysis**
   - Calculate the average sale price of 4-bedroom homes by year.
   - Find average prices of 3 bed / 3 bath homes by year built.
   - Query average price for larger homes with 3 bed / 3 bath / 2 floors and ≥2000 sqft.
   - Identify view ratings with average home prices ≥ $350,000.

3. **Optimization Techniques**
   - Cache and uncache the `home_sales` temporary view.
   - Measure and compare query runtime before and after caching.

4. **Data Partitioning**
   - Write the data to Parquet files partitioned by `date_built`.
   - Run optimized queries using the partitioned data and compare runtimes.

5. **Validation**
   - Confirm caching and uncaching with `spark.catalog.isCached()`.

---

## How to Run

1. Open the `Home_Sales.ipynb` notebook in Google Colab.
2. Run all cells in order.
3. Query results and runtimes will be printed in the output cells.
4. Upload the final `.ipynb` file to your "Home_Sales" GitHub repository.

---

## Author

**Manuel Guevara**  
Data Analytics Final Project | 2025
