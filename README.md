# ETL In Python and SQL

This repo contains code and notes I took from the course- ETL in Python and SQL from LinkedIn Learning

## Chapter 1) What are ETL?
    Data Pipeline- A Set of process and technologies that describes data's journey or movement from the data source to its desitnation
    
    ETL- 
        * Extract: Moving data from source (Sources: Spreadsheet, API, DB or cloud system) (Tools: Python, AWS Glue, Azure Data Factory, Talend)
        * Transform: Cleaning and transforming the data to remove errors, duplicates or irrelevant information (Tools: Python, Spark, Azure Data Factoy)
        * Load: Loading the data to the target database, data warehouse, data lake or data mart (Tools: Python, Spark, Azure Data Factory)

    Orchestration Tools- Create and orchestrate ETL by passing parameter. Helps to shadow, monitor and manage your ETL (Tools: Apache Airflow, SQL Server Integration Services, Azure Data Factory, and AWS Database Migration Services)

    Factors to Consider- 
        * Pipeline Architecture and Tool
        * Data Sources, transformation, and destination
        * How often do we intend to pull the data
        * Data volume and velocity
        * Scalability and Performance
    
    Pandas- A open source Python Library used for data manipulation and analysis

## Chapter 2) Extracting and Transforming Data with Python
    Data Sources- It can be production database, SQL or NoSQL database, APIs, JSON files, Excel or CSV files

    Data Formats- XML, Parquet, JSON, TXT

    Transforming involves- Cleaning, Standardizing, removing duplicates and missing values. It focuses on converting raw data coming from different system into a format that is suitable for target system. Its important for data quality and consistency

        * De-Duplication- Identifying and removing duplicate data from dataset
        * Data Integration- Transforming data from various source systems  into a common format and structure  
        * Data Aggregation- The process of summarizing, grouping, or consolidating data from multiple rows or records into single value or set of values
        * Data Filtering- Remove unwanted data from entire dataset.
        * Data Cleaning- We identify and eliminate errors and inconsistencies in the data

