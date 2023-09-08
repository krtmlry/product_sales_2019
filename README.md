# Product sales data set ETL pipeline

## Summary
An electronics shop called cdr-queen that sells electronic products would like to know about their
sales performance for the year 2019.

Currently this company stores all of their sales records through a csv file and the owners are planning to make use of the latest technology to further enhance their operations by using data analysis.

They'd like a data engineer to design a pipeline that will extract the needed data from a csv file, clean and transform the data into fact and dimension tables and lastly, store it in a cloud based database so that their analysts can access it anytime.

## About the project

In this project, we will transform and model the data using Pandas and Python. We will also be using an open source ETL tool called Mage.ai to house all necessary codes for the pipeline. The output will then be exported to a cloud based Postgres database called Supabase.

To save costs, I've decided to utilize supabase as a datawarehouse.

> Note: The ETL pipeline will only keep sales record for year 2019.

## Dataset
`Product sales 2019 dataset`
url: https://raw.githubusercontent.com/krtmlry/pipelines/main/product_sales/data/productsales_merged_01.csv
> Please take note that this is the merged version of the dataset from January - December 2019.

## Data model
The database is designed using a star schema that consists of a fact and dimension tables. \
This type of modelling is utilized since we are trying to create an OLAP database that is only exclusive for analysis.

![image.png](attachment:4094e4bd-fbae-4382-9243-85d8aeda3d0d.png)

