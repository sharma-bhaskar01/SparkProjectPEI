# PEI_assessment
PEI assessment task for data engineering role.

The basic approch for this assignment is as follows.

Step1. Extract data from various sources:
Read the data from Order.json, Customer.xlsx, Product.csv using spark.read function. In case of xlsx file we need to install com.crealytics.spark.excel package to fetch this data without any hassels.

Step2. Clean data and columns:
Once we have this data in dataframes we need to first check and then clean the data if needed, in our case we did see a lot of NULL values and special characters in our data set hence we need to use the fill_null function and clean any special characters embedded in between customer names. Additional checks can be placed on product quantity or amount columns to make sure they are all positive.

Step3.
Add these cleaned data sets to table.

Step4. Create output tables
Create the enriched_orders table by combining the data between orders, customer and product datasets. Once we have this dataset we can also create profit_aggregate table as per given logic.

Step 5. Generate reports
Use the profit aggregate table to display reports.


-----------------------------------------------------------------------------------------------------------------------------

Assignment coding styles :

There are two approaches to code this assignment to get the results.
1. Create a package using python files which can be pushed to DBFS and then later can be used to generate result.
2. We can directly write all the functions and SQL code in databricks notebook to generate the results.

For the first approach I am adding the entire python code along with other resources in the repo which can be pulled and used in databricks notebook once we add it to our DBFS path.

For the second apporach I am adding the iPython file to show the results and the code in the notebook.



