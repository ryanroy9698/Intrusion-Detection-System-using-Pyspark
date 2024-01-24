# Intrusion-Detection-System-using-Pyspark
# Data Analysis and Cloud Integration Project
## Introduction
The project focused on conducting a comprehensive data analysis and integrating cloud platforms. The primary dataset for this endeavor was the KDD Cup 99 10% subset (2.1M; 75M Uncompressed), accessible from [KDD Cup 99](http://kdd.ics.uci.edu/databases/kddcup99/kddcup99.html). The project was structured into two main components: data analysis using PySpark in Databricks and exploring concepts related to cloud data platforms.

## Part A: Data Analysis with PySpark in Databricks

### 1. Understanding Intrusion Detection System
 After understanding the concept of an Intrusion Detection System (IDS) and evaluated its applicability to the KDD Cup 99 dataset. This involved understanding the workflow outlined in the provided paper.

### 2. Data Retrieval and Storage
Utilizing the Python urllib library, extracted the KDD Cup 99 data from the web and stored it in the Databricks filesystem for streamlined access.

### 3. Loading Data into Spark's RDD
Leveraging PySpark, the data was loaded from the Databricks filesystem into Spark's Resilient Distributed Datasets (RDD). This step included printing 10 values and verifying the data structure.

### 4. Data Splitting and Features
Split the data, with each entry being a comma-separated line, and determined the total number of features (columns) in the dataset.

### 5. Extracting Specific Columns
Selected columns (duration, protocol_type, service, src_bytes, dst_bytes, flag, and label) were extracted to form a new RDD and DataFrame.

### 6. Exploring Connections
Using PySpark, I identified the total number of connections based on protocol_type and service, presenting the results in ascending order. Bar graphs were plotted for visual representation.

### 7. Further Exploratory Data Analysis
To gain deeper insights, I conducted additional exploratory data analysis on various columns in the dataset, plotting at least three different charts and providing explanations.

### 8. Intrusion Detection Model
Creating a new label column for normal and attack labels, I  split the data and built a machine learning model for intrusion detection using a selected algorithm. The choice of the algorithm and results were explained thoroughly.
