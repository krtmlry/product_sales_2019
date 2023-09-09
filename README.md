# Product sales data set ETL pipeline

## About the project

In this project, we will transform and model the data using Pandas and Python. We will also be using an open source ETL tool called Mage.ai to house all necessary codes for the pipeline. The output will then be exported to a cloud based Postgres database called Supabase.

The cloud database for this project is Supabase. Since I want to avoid utilizing paid cloud services for this fictional project.

> Note: The ETL process will only keep sales record for year 2019.

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
