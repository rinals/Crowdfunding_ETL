# Extract Transform Load
This project is to extract data from Excel files, then transform the data using Python Pandas into CSV file. The data is then loaded into tables in PG-SQL Relational database

## Extract data from Excel (xls)
Python Pandas package provides convenient functions to load data from Excel files (xlsx)

## Transform the data using Python Dataframes into CSV
    1. Separate Category and SubCategory columns
    2. Create separate Dataframes with their own indices :
        a. contacts
        b. Category
        c. Sub Category
        d. Campaign
    3. Write the transformed Dataframes into CSV files. Each CSV file has its own index and can be loaded easily into SQL tables.

## Load the data into PG SQL
### ERD
Use [QuickDBD](https://app.quickdatabasediagrams.com/#/) to create Relational Tables for each of the CSV files.

Create tables with appropriate Primary keys and foregin keys. QBD will show the relationship and automatically create a clean diagram for all the tables.

Use the Export function to generate SQL queries for table creation.

### PG SQL
    1. Create the Database
    2. Import the SQL queries for table creation from QuickDBD
    3. After verifying the table schema, import CSV files into corresponding tables.
