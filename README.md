# Data Ingestion Pipeline  

This project demonstrates the creation of a robust **data ingestion pipeline** combining **batch processing** and **real-time streaming**. The pipeline was built using **Apache Sqoop**, **Apache Flume**, and **Apache Kafka** on a local machine, with an e-commerce database as the data source.

---

## Objectives  
- Design a pipeline that integrates batch data migration and real-time data streaming.  
- Migrate historical data from MySQL to HDFS using Apache Sqoop.  
- Ingest real-time data from local files and stream it using Apache Flume and Kafka.

---

## Technologies  
- **MariaDB:** Stores structured data in relational tables for e-commerce use cases.  
- **Apache Sqoop:** Handles batch data migration from MySQL to HDFS.  
- **Apache Flume:** Manages real-time ingestion of data from local files to Kafka.  
- **Apache Kafka:** Streams and processes real-time data.  
- **HDFS:** Provides distributed storage for large-scale data.  

---

## Features  
- **E-commerce Database Setup:**  
  - Designed tables (`users`, `products`, `orders`) to mimic a real-world scenario.  
  - Inserted sample data for testing batch and real-time ingestion workflows.  

- **Batch Processing:**  
  - Migrated data from MySQL to HDFS using Sqoop, including incremental imports for changes.  

- **Real-Time Streaming:**  
  - Configured Flume to ingest real-time file data.  
  - Used Kafka to process and stream live data, verifying output with Kafka Console Consumer.  

---

## Commands and Implementation  
- **Database Setup:**  
  - Created an `ecommerce` database and populated it with sample users, products, and orders.  
  - Verified using MySQL commands (`SHOW DATABASES;`, `SHOW TABLES;`).  

- **Batch Migration:**  
  - Used Sqoop to transfer entire tables and incremental changes to HDFS directories.  

- **Real-Time Streaming:**  
  - Set up Flume agents for file ingestion.  
  - Created Kafka topics and consumed streams using `kafka-console-consumer`.  

---

## How to Run  
1. **Environment Setup:**  
   - Install required tools: MySQL, Hadoop, Sqoop, Flume, Kafka, and Zookeeper.  
   - Set up the `ecommerce` database in MariaDB.  

2. **Batch Data Processing:**  
   - Use Sqoop commands to migrate data from MySQL to HDFS.  

3. **Real-Time Data Streaming:**  
   - Configure and run Flume agents to ingest data from local files.  
   - Set up Kafka topics and consume data streams.  

4. **Verification:**  
   - Check HDFS for batch data.  
   - Use Kafka Consumer to verify real-time streams.  

---

## Conclusion  
This project successfully demonstrates the integration of batch and real-time data processing, showcasing the use of popular big data tools for efficient data handling in an e-commerce scenario.
