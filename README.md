[Udemy : this course](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/); ([Udemy : the Python course mentioned in Lecture 01](https://www.udemy.com/python-for-data-science-and-machine-learning-bootcamp/))

We will cover the following topics :

* Spark and Big Data basics [**s1**]
* Setting up Spark in various ways [**s2, s3, s4, s5, s6**]
* Python crash course [**s7**]
* Python and Spark 2.0 DataFrames [**s8**]
* PySpark project exercise [**s9**]

Then in the second half of the course :

* Introduction to Machine Learning
* Linear Regression
* Logistic Regression
* Decision Trees and Random Forests
* Gradient Boosted Trees
* K-Means Clustering
* Recommender Syatems
* Natural Language Processing
* Spark Streaming (local and Twitter)


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
* [25](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6970748?start=0) Spark DataFrames - Basics pt2 ...[*grabbing the data; creating new columns; using SQL with dataframes*] [*`df.select(['age', 'name']).show()`* ; *`df.withColumn('newage', df['age']).show()`* ; *`df.createOrReplaceTempView('people')`, `results = spark.sql("SELECT * FROM people")`*]
* [26](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6675062?start=0) Spark DataFrames - Basic Operations ...[**`from pyspark.sql import SparkSession`**; **`spark = SparkSession.builder.appName('ops').getOrCreate()`**; **`df = spark.read.csv('appl_stock.csv', inferSchema=True, header=True)`**]
* 27 Groupby and Aggregate Operations
* 28 Missing Data
* 29 Dates and Timestamps


### §9
### §10
### §11
### §12
### §13
### §14
### §15
### §16
### §17


### §18 Bonus

* [66](https://www.udemy.com/spark-and-python-for-big-data-with-pyspark/learn/v4/t/lecture/6666744?start=0) Coupons