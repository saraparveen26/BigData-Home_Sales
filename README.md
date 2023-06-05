# Home Sales (Big Data)

This challenge is completed as requirement of Data Analytics Boot Camp at University of Toronto.

In this assignment, I have used my knowledge of SparkSQL to determine key metrics about home sales data. I have used Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached. The assignment was completed on Google Colab.


Following steps are followed to complete the requirements of the challenge:

1.  Import the necessary PySpark SQL functions for this assignment.

2.  Read the home_sales_revised.csv data into a Spark DataFrame.

    ![DataFrame](Images/Image1.png)

3.  Create a temporary table called home_sales.

4.  Answer the following questions using SparkSQL:

    -   What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.

    ![Q1](Images/Image2.png)

    -   What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.

    ![Q2](Images/Image3.png)

    -   What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.

    ![Q3](Images/Image4.png)

    -   What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.

    ![Q4](Images/Image5.png)

5.  Cache the temporary table home_sales.

6.  Check if your temporary table is cached.

7.  Using the cached data, run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

    ![Cached data](Images/Image6.png)

8.  Partition by the "date_built" field on the formatted parquet home sales data.

9.  Create a temporary table for the parquet data.

10. Run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

    ![Parquet data](Images/Image7.png)

11. Uncache the home_sales temporary table.

12. Verify that the home_sales temporary table is uncached using PySpark.



## RESULTS

The query run time for uncached data is 0.755555 seconds.

The query run time for cached data is 0.46856 seconds.

The query run time for parquet data is 0.38534 seconds.