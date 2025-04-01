# Ride-sharing-spark-streaming

## **Prerequisites**

Before starting the assignment, ensure you have the following software installed and properly configured on your machine:

1. **Python 3.x**:
   - [Download and Install Python](https://www.python.org/downloads/)
   - Verify installation:
     ```bash
     python3 --version
     ```

2. **PySpark**:
   - Install using `pip`:
     ```bash
     pip install pyspark
     ```

3. **Apache Spark**:
   - Ensure Spark is installed. You can download it from the [Apache Spark Downloads](https://spark.apache.org/downloads.html) page.
   - Verify installation by running:
     ```bash
     spark-submit --version
     ```

4. **Faker**:
   - Install using `pip`:
     ```bash
     pip install faker
     ```

## **Setup Instructions**

### **1. Running the Analysis Tasks**

You can run the analysis tasks either locally or using Docker.

#### **Running with Docker **

1. **Start the Spark Cluster**:
   ```bash
   docker-compose up -d
   ```

2. **Run Your PySpark Scripts Using `spark-submit`**:
   Once you perform all the three tasks, run the following:
   ```bash
   spark-submit task1.py
   spark-submit task2.py
   spark-submit task3.py
   ```

3. **Verify the Outputs**:
   On your host machine, check the `output/` directory for the resulting files.

4. **Stop the Spark Cluster**:
   ```bash
   docker-compose down
   ```

## **Overview**

# Real-Time Ride-Sharing Analytics with Apache Spark

In this assignment, you will build a real-time analytics pipeline for a ride-sharing platform using Apache Spark Structured Streaming. You will process streaming data, perform real-time aggregations, and analyze trends over time.

The workflow consists of:

A Python script that simulates real-time ride-sharing data
Apache Spark (Structured Streaming) to read, clean, and analyze the incoming data.
Writing the processed results to CSV files for further analysis.
Your assignment is divided into three tasks:

Task 1: Ingest and parse real-time ride data.
Task 2: Perform real-time aggregations on driver earnings and trip distances.
Task 3: Analyze trends over time using a sliding time window.
