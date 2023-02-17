# Liquor-Database-Management-System

The goal of this project is to help retailers with inventory management. 
Efficient inventory management helps to reduce costs, enhance cash flow, ensure continuous supply as well as fulfillment of customer needs and demands.
Created an inventory management system which helps to track the in-demand products, manage warehouse space to reduce costs, enhance cash flow, ensure continuous supply as well as fulfillment of customer needs and demands.

The dataset used contains information on the name, type, price, quantity and location of sales of individual containers or packages of containers of liquor sold in different counties of Iowa state.

There are a total of 8 tables in the schema.
All 8 tables have either a primary key or foreign key or both present in it.
Tables are created using Postgre sql UI and while creating, declared the primary key of the table and the datatypes for all the attributes.

Created individual csv for each table and loaded them to postgre with the help of its UI to import data. After, the data was imported declared the foreign keys for each table as per the ER diagram.

The ER diagram is as shown below:
![image](https://user-images.githubusercontent.com/51898794/219795742-a90b5b55-50ef-412a-8dde-4b2485265bf6.png)

Normalization (1NF, 2NF, 3NF, BCNF) was performed on the dataset to increase data integrity and remove data redundancy if any from the tables.

Executed queries to find Total sales of liquor of a single category for all the stores in descending order, Black Friday sales for individual year, Yearly liquor revenue for Iowa state, etc. performing aggregate functions, joins, query optimization, triggers, typecasts, clauses, et. al.
