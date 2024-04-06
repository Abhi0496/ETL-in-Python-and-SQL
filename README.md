# ETL In Python and SQL

This repo contains code and notes I took from the course- ETL in Python and SQL from LinkedIn Learning

## Chapter 1)
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
