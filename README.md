# Azure-End-to-End-NYC-DE-Project

### Overview
This repository demonstrates the implementation of the Medallion Architecture for an end-to-end Data Engineering solution using Microsoft Azure. The project showcases how Azure's robust ecosystem can address modern data engineering challenges with scalability, efficiency, and flexibility.

### Prerequisites

To run this project, ensure the following Azure services and tools are available:
* Azure Account
* Power BI Desktop Installed

### Getting Started:

 #### 1. Data Ingestion
  - Source: Data was ingested from NYC TAXI API "https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page".
  - Tool Used: Azure Data Factory (ADF) enabled seamless pipeline orchestration for retrieving and staging raw data.

 #### 2. Data Storage
  - Service: Azure Data Lake Storage (ADLS) Gen2.
  - Structure: Data is structured into three layers following the Medallion Architecture:
  - Bronze Layer: Raw data as ingested from the source.
  - Silver Layer: Cleaned and enriched data ready for analytical processing.
  - Gold Layer: Optimized datasets for reporting and business intelligence.

  #### 3. Data Transformation
  - Tool Used: Azure Databricks.
  - Process: Transformed data using PySpark to ensure high-quality, optimized datasets ready for downstream consumption.

  #### 4. Delta Lake Implementation
  - Capabilities:
     * Data versioning for maintaining historical records. 
     * Time travel to analyze data from previous states.
     * Rollback support is needed to revert to earlier data versions.
  - Benefit: Enhanced reliability and flexibility in handling large-scale data transformations.

  #### 5. Visualization
  - Tool Used: Power BI.
  - Integration: Connected to the Gold Layer to create actionable insights.
