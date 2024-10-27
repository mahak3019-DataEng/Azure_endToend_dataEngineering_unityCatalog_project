# Telecom Data Transformation Project

## Overview

This project focuses on building a comprehensive data engineering solution for the telecom domain utilizing Microsoft Azure services. The goal is to analyze market share, performance metrics, and revenue generation across various dimensions, enabling data-driven decision-making.

### Key Datasets

1. **Dimension Tables**:
   - **dim_cities**: Contains information about cities, including city ID, name, and geographic details.
   - **dim_date**: Holds date-related attributes for effective time-based analysis, including day, month, and year.
   - **dim_plan**: Details about telecom plans, including plan ID, name, features, and pricing.

2. **Fact Tables**:
   - **fact_market_share**: Metrics related to market share across different telecom plans and regions.
   - **fact_metrics_share**: Performance metrics of various telecom services and their market penetration.
   - **fact_plan_revenue**: Revenue data generated from different telecom plans over specified time periods.

This project employs a range of Azure services, including Azure Data Factory, Databricks, and Azure Key Vault, to facilitate data ingestion, processing, and governance.

## Project Details

### Project Type

- **Domain:** Telecom
- **Duration:** 3 weeks
- **Azure Subscription:** Pay as You Go
- **Resources Used:** ADF, ADLS GEN2, Databricks, Logic Apps, Key Vault, Repo, DevOps, CI/CD

### Data Processing

- **Type:** 
  - Batch Data Processing

### Data Sources

- **MySQL, SFTP**

### Datasets Format

- **CSV, Parquet**

### ADF Pipelines

- **6 Pipelines**
- **Load Types**: 
  - Full Load
  - Incremental Load

### Cluster Configuration

- Interactive single node cluster
- Policy: Unrestricted
- Access Mode: No isolation shared

### Authentication

- **System Assigned Managed Identity, Service Principal, or Access Token, secret scope, Unity Catalog access**

### Performance Optimization Techniques

- Parallel Processing in ADF
- Data Compression Techniques
- Parameterization for Pipelines
- Utilizing Databricks Notebooks (Spark)
- Implementing Data Partitioning
- Incremental Data Loading

## Project Responsibilities

- Creating and managing metadata tables
- Setting up linked services and datasets
- Implementing ADF pipelines and triggers
- Utilizing Azure Logic Apps for email alerts
- Employing Azure Key Vault for secrets management
- Developing data transformation logic using Databricks notebooks
- Storing data in various layers (raw, intermediate, curated) using ADLS GEN2
- Implementing data governance with Azure Active Directory and RBAC

## Challenges Faced

- Managing small files and duplicate records
- Resolving data mismatch and pipeline run timing issues
- Addressing Spark memory management challenges
- Optimizing standard vs. partitioned tables