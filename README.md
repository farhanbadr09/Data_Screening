# Data_Screening
Hi Team, Hopefully you're doing great!

<h4>Tools:</h4>
Python<br>
Jupyter Enviroment<br>
MySQL (RDBS)<br>
AWS <br>

Dependencies (Import libraries)
```
import time
from tqdm.notebook import tqdm, trange
import pandas as pd
import numpy as np
from zipfile import ZipFile
from io import BytesIO
import urllib.request as urllib2
import boto3
from boto3.s3.transfer import TransferConfig
from boto3.s3.transfer import S3Transfer
import io
import pyarrow as pa
import pyarrow.parquet as pq
```

<hr>
<b>1. Schema
Design an RDBMS table schema to store the CSV data</b>

<i>Database Name :</i> Stocks_Data<br>
<i>MySQL Query:</i> ```CREATE DATABASE IF NOT EXISTS Stock_Data;``` <br>
<i>Select Database Query:</i> ```Use Stock_Data;```<br>
<i>Creating Table Query :</i> <br>
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
<i>Displays Metadata Query:</i> ```Describe mytable;```

<hr>

<b>2 Calculation You are required to use this data and calculate the following using SQL </b><br>
<i>Weekly average of High, Low and Volume:</i> <br>
<i>Query: </i>```SELECT WEEK(Date),AVG(High),AVG(Low), AVG(Volume) FROM data group by WEEK(Date);```

<i>Monthly average of High, Low and Volume:</i> <br>
<i>Query: </i>```SELECT MONTH(Date),AVG(High),AVG(Low), AVG(Volume) FROM data group by MONTH(Date);```

<i>Yearly average of High, Low and Volume:</i> <br>
<i>Query: </i>```SELECT YEAR(Date),AVG(High),AVG(Low), AVG(Volume) FROM data group by YEAR(Date);```<br>

<i>Jupyter Source File:</i> Stock Data ETL Process Part-1.ipynb (Contains first two Questions)<br>

<hr>

Stock Data ETL Process Part-2.ipynb (Contains third Question)

Author: Farhan Badr
