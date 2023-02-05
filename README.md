# Data_Screening
Hi Team, Hopefully you're doing great!

<h4>Tools</h4>
Python
MySQL (RDBS)
AWS


1. Schema
Design an RDBMS table schema to store the CSV data

Database Name : Stocks_Data
MySQL Query: CREATE DATABASE IF NOT EXISTS Stock_Data; 
Select Database Query: Use Stock_Data;
Creating Table Query : 
CREATE TABLE mytable(
   Date DATE NOT NULL PRIMARY KEY,
   Open NUMERIC(10,6) NOT NULL,
   High NUMERIC(10,6) NOT NULL,
   Low  NUMERIC(10,6) NOT NULL,
   Close NUMERIC(10,6) NOT NULL,
   Adj_Close NUMERIC(10,6) NOT NULL,
   Volume INTEGER  NOT NULL
);

Displays Metadata Query: {describe mytable;}
