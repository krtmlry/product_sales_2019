# Product sales data set ETL process

## About the project

In this project, we will extract,transform and load the data using Pandas and Python. We will focus on the process of ETL and later on will try to include ETL tools in the process.

The cloud database for this project is Supabase. Since I want to avoid utilizing paid cloud services for this fictional project.

> Note: The ETL pipeline will only keep sales record for year 2019.
## ipynb files
- merging_csv.ipynb - for merging csv files from January - December 2019.
- productsales_etl_01.ipynb - for the entire ETL process of this project.

## Dataset
`Product sales 2019 dataset`
url: https://raw.githubusercontent.com/krtmlry/product_sales_2019/main/data/productsales_merged_01.csv
> Please take note that this is the merged version of the dataset from January - December 2019.

## Data model
The database is designed using a star schema that consists of a fact and dimension tables. \
This type of modelling is utilized since we are trying to create an OLAP database that will be used for analysis.

![data-model](https://github.com/krtmlry/product_sales_2019/blob/main/img/db-model-01.png?raw=true)

## Project architecture
![architecture](https://github.com/krtmlry/product_sales_2019/blob/main/img/Architecture.png?raw=true)

## Technology used
- Data source: Github raw csv file
- Programming language: Python
- Code editor: Jupyterlab
- Database: Supabase
- Dashboard: Lookerstudio

## Dashboard
The sales dashboard is built on lookerstudio, google's free web based BI tool.
The dashboard is a mixed of table uploads from supabase and also some direct sql queries were done.

Since this is an end-to-end data engineering project, I focused more on the ETL part rather than the dashboarding.

Link to dashboard: https://lookerstudio.google.com/reporting/158fe66e-c3d0-4189-8af0-e3e040d3e917
> The dashboard is currently static, there are no filters added and only shows the summary of the product sales for 2019.