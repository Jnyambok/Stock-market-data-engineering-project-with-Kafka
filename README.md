# Stock Market Kafka Real Time Data Engineering Project

## Introduction 
Apache Kafka is a distributed event store and stream processing platform.

**Producer**: A single source of data in Kafka ecosystem

**Broker**: A node / worker or single member of the Kafka cluster. They are responsible for writing the data received from the producers

**Consumer**: User for the data

**Cluster**: Collection of brokers/Group of one or more brokers working together to satisfy Kafka production and Consumption

**Data Partition**: Kafka topics consist of one or more partitions. A partition is a log which provides ordering guarantees for all the data contained within it. Partitions are chosen by having key values.

A **Topic** is essentially a named channel or feed where messages (also called events or records) are published by producers and consumed by consumers.  
Streams of "related" messages in Kafka.
The producer to Topic is an **N to N** relation and there can be an unlimited number of topics
Topics in Kafka are partitioned, which is when we break a topic into multiple log files that can live on separate Kafka brokers

Think of it like a mailing list or a news feed:

1. **Producers**: These are applications or systems 
that send messages to a specific topic. For example, a web server might send user activity logs to a topic named "user_activity."   

2. **Consumers**: These are applications that subscribe to a topic and receive the messages published to it. For instance, a data analytics application might subscribe to the "user_activity" topic to analyze user behavior. 




## Architecture 
![Architecture](https://github.com/user-attachments/assets/36d61260-c2c5-437f-aa14-32944350ca36)


## Video
I was able to create a producer and consumer and siumlate stock market data which was stored in an S3 bucket
![actual prod and consumer](https://github.com/user-attachments/assets/aa1d35f8-6e90-4db1-b62a-0d8a2ec2d0b8)


## Technology Used
**AWS EC2 instance** - Deployed an instance and installed Apache Kafka on it. Used SSH to run Zookeper, Apache Server and simulate a Producer-Consumer scenario
**Google Collabs** - For experimentation
**AWS S3 Bucket**  - To store the streaming data

## Technologies yet to be incorporated
AWS Glue Crawler
AWS Glue Catalog


