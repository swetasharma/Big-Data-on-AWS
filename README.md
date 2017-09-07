# Big-Data-on-AWS
What is Big Data?
Not sitting in relational databases and tables (Bar code scanning, Machine generated data, tweets)
where big data can be applied?
Clickstream analysis, buying patterns in ecommerce, Fraud Detection, Machine learning based investment strategies. Healthcare research, Prediction (and prevention) of equipment failure.

Wide variety of data supported
RDBMS, NOSQL, EDW, HADOOP

1. Elastic MapReduce.(Amazon's implementation of Hadoop, Highly integrated with S3, can be completely scripted, interactive command line access via SSH(secure socket shell - this is a protocol upon which we will be able to set up terminal session(- by creating a key pair) with head node in our elastic map reduce cluster)). Install SSH client e.g. Putty and configure with key pair.(puttygen - to make ppk file  from the pem file).
2. Redshift.(use Massively parallel processing technology, column store data warehouse, petabyte scale, uses common relational, SQL technology, Integrated with S3 and DynamoDB).
3. DynamoDb.(use Key-value store to manage the data, Schema-less, accomodates unstructured data).
4. Data Pipeline.(Workflow system for shaping data and moving data from table to table, database to database, and various componenents in AWS, Batch oriented tool).
5. S3.(Amazons cloud based blob storage service).
6. Jaspersoft AWS.
7. Kinesis.

CAP Theorem:
Relational: Consistency, Partition Tolerance.
NoSql: Availability, Partition Tolerance.
Big Data and Nosql are interrelated(Consistency not an issue, do bulk read operations very very quickly).

What is Hadoop?
Combines two things 1. processing engine (that implements a specific data processing algorithm called map reduce) along with distributed file system. HDFS(if we have a bunch of virtual machines together that make up elastic map reduce cluster or hadoop cluster then we want a way to take all of the disk drives on each of those nodes and federate them together as one logical storage volume thats what HDFS does, HDFS make two additional copies of each file that it stores and put those copies on physically separate node, write once read many file system(files cannot be updated)).

The Hadoop Stack:
6. Log file Integration Flume (for dealing with log file and other time series data).
5. Machine Learning / Data Mining (mahout also works as abstraction layer over mapreduce).
4. RDBMS Import/Export: (sqoop which can move data back and forth between hadoop and various relational database management system most of which is used as datawarehousing platform).Implala directly over HDFS Impala works as a interactive query engine.
3. Query: HiveQL(creates sql abstraction layer over map reduce algo, Hive works as a batch system) and Pig Latin (does same thing but it uses it own language latin can be used as ETL tool).
2. Database: (NoSql HBase, hbase tables are HDFS files ..please understand..which means that hbase tables can be used the inout for mapreduce jobs or in fact the output of the map reduce jobs can create new Hbase tables).
1. Hadoop: (MapReduce, HDFS).

A MapReduce example: (Remember generating series of key value pair is call map, we are simply reading in input files and creating output files compatible with HDFS because it is write once file system.)

EMR Job Flows

Lets see how all of these components work together:



