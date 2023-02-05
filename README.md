# Data_Screening
Hi Team, Hopefully you're doing great!

<h4>Tools</h4>
Python
MySQL (RDBS)
AWS

<hr>
1. Schema
Design an RDBMS table schema to store the CSV data

<b>Database Name :</b><br> Stocks_Data
<b>MySQL Query:</b> CREATE DATABASE IF NOT EXISTS Stock_Data; 
<b>Select Database Query:</b> Use Stock_Data;
<b>Creating Table Query :</b> 
CREATE TABLE mytable(
   Date DATE NOT NULL PRIMARY KEY,
   Open NUMERIC(10,6) NOT NULL,
   High NUMERIC(10,6) NOT NULL,
   Low  NUMERIC(10,6) NOT NULL,
   Close NUMERIC(10,6) NOT NULL,
   Adj_Close NUMERIC(10,6) NOT NULL,
   Volume INTEGER  NOT NULL
);

<b>Displays Metadata Query:</b> {describe mytable;}
<hr>
