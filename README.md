# Data Platform Architecture

As part of the capstone project for IBM Data Engineering course provided by Coursera, I have assumed the role of an Associate Data Warehouse Engineer who has recently joined an e-commerce organisation. I was presented with a business challenge that requires building a data platform for retail data analytics. 

SoftCart uses a hybrid architecture, with some of its databases on premises and some on cloud.

Tools and Technologies:

OLTP database - MySQL

NoSql database - MongoDB

Production Data warehouse – DB2 on Cloud

Staging Data warehouse – PostgreSQL

Big data platform - Hadoop

Big data analytics platform – Spark

Business Intelligence Dashboard - IBM Cognos Analytics

Data Pipelines - Apache Airflow

Process:

SoftCart's online presence is primarily through its website, which customers access using a variety of devices like laptops, mobiles and tablets.
All the catalog data of the products is stored in the MongoDB NoSQL server.
All the transactional data like inventory and sales are stored in the MySQL database server.
SoftCart's webserver is driven entirely by these two databases.
Data is periodically extracted from these two databases and put into the staging data warehouse running on PostgreSQL.
The production data warehouse is on the cloud instance of IBM DB2 server.
BI teams connect to the IBM DB2 for operational dashboard creation. IBM Cognos Analytics is used to create dashboards.
SoftCart uses Hadoop cluster as its big data platform where all the data is collected for analytics purposes.
Spark is used to analyse the data on the Hadoop cluster.
To move data between OLTP, NoSQL and the data warehouse, ETL pipelines are used and these run on Apache Airflow.

# Summary 

Module 1: I will design the OLTP database for an e-commerce website, populate the OLTP Database with the data provided, and automate the export of the daily incremental data into the data warehouse. 

Module 2: I will set up a NoSQL database to store the catalog data for an E-Commerce website, load the E-Commerce catalog data into the NoSQL database, and query the E-Commerce catalog data in the NoSQL database. 

Module 3: I will design the schema for a data warehouse based on the schema of the OLTP and NoSQL databases. Then I will create the schema and load the data into the fact and dimension tables, automate the daily incremental data insertion into the data warehouse, and create Cubes and Rollups to make the reporting easier. 

Module 4: I will create a Business Intelligence dashboard. I will create a Cognos data source that points to a data warehouse table, create a bar chart of quarterly sales of cell phones, create a pie chart of sales of electronic goods by category, and create a line chart of total sales per month for a given year. 

Module 5: I will extract data from an OLTP, NoSQL, and MongoDB databases into CSV format. I will then transform the OLTP data to suit the data warehouse schema, and then load the transformed data into the data warehouse. Finally, I will verify that the data is loaded properly. 

Module 6: I will use my skills in Big Data Analytics to create a Spark connection to the data warehouse and then deploy a machine learning model on SparkML for making sales projections.
