[Udemy : this course](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/); ([Udemy : the Python course mentioned in Lecture 01](https://www.udemy.com/python-for-data-science-and-machine-learning-bootcamp/))

We will cover the following topics :

* Spark and Big Data basics [**s1**]
* Setting up Spark in various ways [**s2, s3, s4, s5, s6**]
* Python crash course [**s7**]
* Python and Spark 2.0 DataFrames [**s8**]
* PySpark project exercise [**s9**]

Then in the second half of the course :

* Introduction to Machine Learning [**s10**]
* Linear Regression [**s11**]
* Logistic Regression [**s12**]
* Decision Trees and Random Forests [**s13**]
* Gradient Boosted Trees
* K-Means Clustering [**s14**]
* Recommender Systems
* Natural Language Processing [**s16**]
* Spark Streaming (local and Twitter) [**s17**]


### §1 Introduction to the Course

* [01](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/5856256?start=5) Introduction
* [02](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6804318?start=0) Course Overview [[slides](https://docs.google.com/presentation/d/1pRsyibkbWbfWiKRh4hVgxUZlZ6wLKQLkxbUwkIvnauc/edit#slide=id.p)]
* [03](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6804316?start=0) Frequently Asked Questions
* [04](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6804314?start=0) What is Spark? Why Python? [[slides](https://docs.google.com/presentation/d/1u5FT9oG2lkSP6BKS9xYcHAd-MP17L3KSQFsX44nAzAY/edit#slide=id.p)] ...[*[http://spark.apache.org/](http://spark.apache.org/)*]


### §2 Setting up Python with Spark

* [05](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6681692?start=0) Setting up Python with Spark [[slides](https://docs.google.com/presentation/d/1fZErOcKjN3Yq95eD8A716_jw-XnwRAeiNFTF7q74iJM/edit#slide=id.p)] ...[*4 main installation options*]
* [06](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6813186?start=0) Note on Installation Sections


### §3 Local VirtualBox set-up [[slides](https://docs.google.com/presentation/d/1FH8-DGwxCIOrfSBUmInfFFNQ2H2oulp_HOHAjbVyCDA/edit) ...*for s3-s6*]

* [07](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6681698?start=0) Local installation VirtualBox Pt1 ...[*install VirtualBox and Ubuntu*]
* [08](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6806898?start=0) Local installation VirtualBox Pt2 ...[*install Python, Jupyter notebook, Spark*]
* [09](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/7007266?start=0) Setting up PySpark ...[*`findspark` library, to use `pyspark` from any directory*]


### §4 AWS EC2 PySpark set-up [Elastic Compute Cloud]

* [10](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6681696?start=0) AWS EC2 set-up guide ...[[aws.amazon.com](https://aws.amazon.com/)]
* [11](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/7005602?start=0) Creating the EC2 Instance [*save PEM file (which has EC2 key pair), to give you SSH access*]
* [12](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/7005604?start=0) SSH with Mac or Linux ...[**`cd` *to folder with PEM file**, (then* `chmod 400 newspark.pem` *to protect against accidental overwriting,) then* **`ssh -i newspark.pem ubuntu@<dns address of instance, from console>`**]
* [13](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/7005606?start=0) Installations on EC2 ...[`sudo apt-get update`] [*Jupyter Notebook; (Java, Scala, py4j,) Spark, (findspark); connect with PySpark --> access EC2 Jupyter Notebook in local browser @12'45*] [*Installed this Spark version* : `wget http://archive.apache.org/dist/spark/spark-2.4.0/spark-2.4.0-bin-hadoop2.7.tgz`]


### §5 Databricks set-up

* [14](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6804308?start=0) Databricks set-up ...[[https://community.cloud.databricks.com](https://community.cloud.databricks.com)] [`df = sqlContext.sql("SELECT * FROM mytable")`]


### §6 AWS EMR Cluster set-up [Elastic MapReduce]
*"EMR is a collection of EC2 instances with Hadoop (and optionally Hive and/or Pig) installed and configured on them"*

* [15](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6804310?start=0) AWS EMR set-up ...[*Quickly set-up a cluster with a Zeppelin Notebook interface.* **NOT $free**] [[zeppelin.apache.org](https://zeppelin.apache.org/)]


### §7 Python Crash Course [[slides](https://docs.google.com/presentation/d/1CuqvSGMqdMTT1dTblX5enEqZNLS8d0fHwZImQ3zzbpQ/edit)]

* [16](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6813426?start=0) Python Crash Course - Introduction
* [17](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6965316?start=0) Jupyter Notebook Overview ...[*From Q&A: "Spark is not a language, but a library"*]
* [18](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6804666?start=0) Python Crash Course - pt1 ...[*Data structures : List, Dictionary, Tuple, Set*]
* [19](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6804666?start=15) Python Crash Course - pt2 ...[*Operators : Comparison, Logic*] [*Loops : `for`, `while`*] [*range; list comprehension*]
* [20](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6813434?start=0) Python Crash Course - pt3 ...[*functions; `return`; `lambda` expression; methods (`.lower`, `.upper`, `.split`, `.pop`)*]
* [21](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6976258?start=0) Python Crash Course - Exercises
* [22](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6976260?start=15) Python Crash Course - Exercise Solutions


### §8 Spark DataFrame Basics [[slides](https://docs.google.com/presentation/d/1kItYFXxc5Zx-LG-3yizJweZMKev-joLfHLz9rGN7xAE/edit#slide=id.p)]

* [23](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6688214?start=0) Spark DataFrames - Introduction
* [24](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6674914?start=0) Spark DataFrames - Basics pt1 ...[**`from pyspark.sql import SparkSession`**; **`spark = SparkSession.builder.appName('Basics').getOrCreate()`**; **`df = spark.read.json('people.json')`**] [*`df.show()`; `df.printSchema()`; `df.columns`; `df.describe()`; `df.describe().show()`*] [*@5'08-10'25: In case you ever need to define your own schema*]
* [25](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6970748?start=0) Spark DataFrames - Basics pt2 ...[*grabbing data with `select()` (to get a df instead of 'column object'); creating new columns; using SQL with dataframes*] [*`df.select(['age', 'name']).show()`* ; *`df.withColumn('newage', df['age']).show()`* ; *`df.createOrReplaceTempView('people')`, `results = spark.sql("SELECT * FROM people")`*]
* [26](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6675062?start=0) Spark DataFrames - Basic Operations ...[**`from pyspark.sql import SparkSession`**; **`spark = SparkSession.builder.appName('ops').getOrCreate()`**; **`df = spark.read.csv('appl_stock.csv', inferSchema=True, header=True)`**] [*`df.printSchema()`; `df.show()`; `df.head(3)`*] [*Filter w. SQL : `df.filter("Close < 500").show()`; `df.filter("Close < 500").select('Open').show()`; `df.filter("Close < 500").select(['Open', 'Close']).show()`*] [*Filter w. Python : `df.filter(df['Close'] < 500).show()`; `df.filter(df['Close'] < 500).select('Volume').show()`; `df.filter( (df['Close'] < 200) & ~(df['Open'] > 200) ).show()`; `df.filter(df['Low'] == 197.16).show()`; `result = df.filter(df['Low'] == 197.16).collect()`*] [*@8'30: "In real life, you'll probably be 'collecting' more often than 'showing'..."*] [*`row = result[0]`; `row.asDict()['Volume']`*] [*@9'35-10'02:* **"So that's (kind of) your work process more realistically shown ...You'll have some sort of 'collection', off some sort of `filter()` command ... You have to actually index, to grab a particular row object ... And then off of that, if you wanted to, you can just say `asDict()`, and very easily grab the keys from the dictionary"**]
* [27](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6688216?start=0) GroupBy and Aggregate Operations ...[**`spark = SparkSession.builder. appName('aggs').getOrCreate()`**; **`df = spark.read.csv('sales_info.csv', inferSchema=True, header=True)`**] [*`df.groupBy('Company').mean().show()`; `df.groupBy('Company').count().show()`*] [*"Not all methods need a `groupBy()` call. Instead you could just call a generalised `.agg` method that will aggregate across all rows in df" : `df.agg({'Sales':'sum'}).show()`; `df.agg({'Sales':'max'}).show()`*] [*"When you call `df.select()` you can apply that function to whatever column you want, and `show()` or `collect()` the results" "`import` a function ... and you pass that in, within a `select()` call"*] [**`from pyspark.sql.functions import countDistinct, avg, stddev`** *... `df.select(avg('Sales').alias('Average Sales')).show()`*] [**`from pyspark.sql.functions import format_number`** *... `df.select(format_number(stddev('Sales'), 2).alias('std')).show()`*] [*`df.orderBy("Sales").show()` v's `df.orderBy("Sales", ascending=False).show()`*]

* [28](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6688224?start=0) Missing Data ...[[**`spark = SparkSession.builder. appName('miss').getOrCreate()`**; **`df = spark.read.csv('ContainsNull.csv', inferSchema=True, header=True)`**] [*`df.na.drop().show()`; `df.na.drop(thresh=2).show()`; `df.na.drop(how='any').show()`; `df.na.drop(how='all').show()`; `df.na.drop(subset=['Sales']).show()`; `df.na.fill('FILL VALUE').show()`; `df.na.fill(0).show()`*]
* [29](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6688226?start=0) Dates and Timestamps ...[]


### §9 Spark DataFrame Project Exercise

* [30](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6688230?start=0) DataFrame Project Exercise
* [31](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6688232?start=0) DataFrame Project Exercise Solutions


### §10 Introduction to Machine Learning with MLlib

* 32 Introduction to Machine Learning and ISLR
* 33 Machine Learning (with Spark & Python) with MLlib


### §11 Linear Regression
### §12 Logistic Regression
### §13 Decision Trees and Random Forests
### §14 K-means Clustering
### §15 Collaborative Filtering for Recommender Systems
### §16 Natural Language Processing
### §17 Spark Streaming with Python


### §18 Bonus

* [66](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6666744?start=0) Coupons