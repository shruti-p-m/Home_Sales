# Home_Sales
This challenge contains one Jupyter Notebook as well as a partition of the home sales dataset as formatted parquet data. The jupyter notebook Home_Sales.ipynb reads in data from home_sales_revised.csv, which is hosted online and is read to the jupyter notebook. 

A spark session and then a temporary table with the data were created and tables were generated based on the following questions:
- What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.
- What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.
- What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.
- What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.

The temporary table was then cached and the last table was rerun to see the difference in runtimes. 

Then the data was partitioned by the "date_built", and a temporary table was created for the parquet data. The last table was again rerun to see the difference in runtimes. 

The temporary table was then uncached and verified. 
