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

## Chapter 3) Loading data into target system
    Data Warehouse, Data Base, Data Lakes are various ways organization manage and store their data

    Database- 
        * Organized collection of data that are controlled using database management system(DBMS)
        * DBMS is a software that allows you to access , interact and manipulate data in database
        * Database focus on operational and transactional data and managing day to day CRUD (Create, Read, Update, Delete)operation
        * MySQL, Postgres are relational database
        * Database can be structured, un-structures or semi structured
            Structured- Uses table to store data where each table has pre-defined schema with columns and data types
            Semi-Structured- Does not fit into the table but have some organization. Ex- XML, JSON can be stored into MongoDB
            Un Structured- Does not have schema and are not organized into tabular form. These can be stored in an object oriented db
    
    Datawarehouse- 
        * Centralized systems or repositories that store data from various sources
        * Ex- transactional database system, API's, ERM System, and CRM Systems
        * It provides support to Business intelligence and provides a single and structured view in consistent format
        * It tracks historical information
    
    Data Lakes-
        * Its a flexible and scalable data storage system storing both structured and unstructured data
        * It doesn't really require pre-defined schema or structure. It is usually stored in flat file architecture
        * Easier for end user to access raw data
        * Ex- Apache Hive
    
    Sumary-
        * Database provide transactional efficiency
        * Data Warehouse are optimized for complex analytical queries that involves aggregation, grouping and reporting from various sources. It supports historical data from various sources and business Intelligence tools
        * Data Lake provide flexibility and Scalability in data Storage. It provides balance between raw storage and Structured querying
    
    SQLAlchemy- Its a SQL Toolkit library for python which allows you to connect and interact with relational databases like Postgres

    As the data moves in data pipeline it is important to ensure data quality, completness, and correctness. This can be done is various ways
        Check number of rows*columns in source as well as columns  
    
    Data Accuracy Checks- Completeness, Uniqueness, Consistency, Current
    Data Integrity Checks- Duplicates detection, Freshness, Timeliness 
