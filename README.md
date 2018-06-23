# DEV-Offsite-Test2
Answer for the data engineer offsite test2

## 1. Tools
* Jupyer Notebook
* Python3
  * Install python packages
    * PySpark
    * Matplotlib
    * Pandas
```
$ pip install pyspark
```
```
$ pip install matplotlib
```
```
$ pip install pandas
```
## 2. Environment Setup
- Start jupyter notebook in command line
```
$ jupyter notebook
```
- Use jupyter notebook to edit Answer Test2.ipynb
- Spark Session
    - Settings:
    - Local
    - 4 thread
    - UTC time zone
```
spark = SparkSession.builder.master('local[4]').getOrCreate()
spark.conf.set("spark.sql.session.timeZone", "UTC")
```
## 3. Data Validation
 - Date
     - 99 records have found not on 2018-05-20
- Hour
    - No invalid hour e.g null or >24 found in hour column
