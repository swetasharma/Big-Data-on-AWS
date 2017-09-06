# Big-Data-on-AWS
What is Big Data?
Not sitting in relational databases and tables (Bar code scanning, Machine generated data, tweets)
where big data can be applied?
Clickstream analysis, buying patterns in ecommerce, Fraud Detection, Machine learning based investment strategies. Healthcare research, Prediction (and prevention) of equipment failure.

Wide variety of data supported
RDBMS, NOSQL, EDW, HADOOP

1. Elastic MapReduce.(Amazon's implementation of Hadoop, Highly integrated with S3, can be completely scripted, interactive command line access via SSH(secure socket shell - this is a protocol upon which we will be able to set up terminal session(- by creating a key pair) with head node in our elastic map reduce cluster)). Install SSH client e.g. Putty and configure with key pair.(puttygen - to make ppk file  from the pem file).
2. Redshift.(use Massively parallel processing technology, cloumn store data warehouse, petabyte scale, uses common relational, SQL technology, Integrated with S3 and DynamoDB).
3. DynamoDb.(use Key-value store to manage the data, Schema-less, accomodates unstructured data).
4. Data Pipleline.(Workflow system for shaping data and moving data from table to table, database to database, and various componenents in AWS, Batch oriented tool).
5. S3.(Amazons cloud based blob storage service).
6. Jaspersoft AWS.
7. Kinesis.

CAP Theorem:
Relational: Consistency, Partition Tolerance.
NoSql: Availability, Partition Tolerance.
Big Data and Nosql are interrelated(Consistency not an issue, do bulk read operations very very quickly).

What is Hadoop?
combines two things 1. processing engine (that implements a specific data processing algorithm called map reduce) along with distributed file system.

Lets see how all of these components work together:



