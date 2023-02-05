# Data_Screening
Hi Team, Hopefully you're doing great!

<h4>Tools:</h4>
Python<br>
MySQL (RDBS)<br>
AWS <br>

<hr>
1. Schema
Design an RDBMS table schema to store the CSV data

<b>Database Name :</b> Stocks_Data<br>
<b>MySQL Query:</b> ```CREATE DATABASE IF NOT EXISTS Stock_Data;``` <br>
<b>Select Database Query:</b> ```Use Stock_Data;```<br>
<b>Creating Table Query :</b> <br>
```
CREATE TABLE mytable(
   Date DATE NOT NULL PRIMARY KEY,
   Open NUMERIC(10,6) NOT NULL,
   High NUMERIC(10,6) NOT NULL,
   Low  NUMERIC(10,6) NOT NULL,
   Close NUMERIC(10,6) NOT NULL,
   Adj_Close NUMERIC(10,6) NOT NULL,
   Volume INTEGER  NOT NULL
);
```
<b>Displays Metadata Query:</b> ```Describe mytable;```

<hr>

2 Calculation You are required to use this data and calculate the following using SQL
<b>Weekly average of High, Low and Volume:</b> <br>
```select week(Date),avg(High) from data group by week(Date);```
