
# 📈 AWS Kafka Stock Market Real-Time Data Engineering Pipeline

An end-to-end real-time data engineering pipeline built using Python, Amazon Web Services (AWS), Apache Kafka, Amazon EC2, Amazon S3, AWS Glue Data Catalog, and Amazon Athena.

The project demonstrates real-time event streaming, Kafka producer/consumer architecture, cloud storage, metadata cataloguing, serverless analytics, IAM security, Linux administration, and AWS cloud infrastructure.


## 🛠️ Tech Stack

**Apache Kafka:** Real-time event streaming and processing

**ZooKeeper:** Kafka broker coordination

**Python:** Producer/Consumer development

**Jupyter Notebook:** Interactive streaming development

**Amazon EC2:** Kafka broker infrastructure

**Amazon S3:** Raw cloud storage

**AWS Glue Data Catalog:** Metadata and schema catalogue

**Amazon Athena:** SQL analytics

## 🚀 Features

- Real-time stock market event streaming using Apache Kafka.
- ZooKeeper used for Kafka cluster coordination.
- Kafka broker hosted on Amazon EC2.
- Python-based Kafka producer and consumer using Jupyter Notebook.
- Raw JSON data persisted to Amazon S3.
- AWS Glue Data Catalog used for schema metadata.
- Amazon Athena used for serverless SQL analytics.
- IAM-based AWS access control.
- Kafka JVM heap tuning for resource-constrained EC2 infrastructure.
- Amazon Athena used for serverless SQL analytics.
## 🧠 Engineering Challenges & Solutions

**Kafka JVM Memory**

**Problem:** 
Kafka attempted to reserve 1 GB of memory on a 1 GB-class EC2 instance.

**Solution:** 
Reduced the Kafka JVM heap: KAFKA_HEAP_OPTS="-Xms128M -Xmx256M"



**EC2 Public IP Changes**

Stopping and starting the EC2 instance changed its automatically assigned public IPv4 address.

The Kafka advertised.listeners configuration and client connection string therefore needed to use the current public endpoint.
## 👤 Author
Wanda Mbatha

AWS Certified Data Engineer - Associate

- [Git Repo](https://github.com/drummerw)
- [LinkedIn](www.linkedin.com/in/wanda-mbatha-b5b01a8b)

