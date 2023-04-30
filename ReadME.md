#   Data Engineering Architecture for Large Scale Data Processing

## Architect: Debanjan Saha


##  Overview

This project involved the development and implementation of a complete data engineering architecture for processing and storing large volumes of data from many different different sources with different types of data. The project included daily, weekly and monthly batch data ingestion, data validation and transformation, data storage, and reporting using various tools and technologies in the Azure cloud environment.

##  Responsibilities

- Designed and led the development of the complete data engineering architecture, including ingestion, transformation, storage, and reporting.
- Led the batch data ingestion (ELT) process using Azure Data Factory and Azure Databricks, performing various transformations and validations on the data.
- Worked on post-processing the data and saving it into various Data Marts for different consumers.
- Architected data storage solutions using various formats like delta, parquet, and csv, and loaded it into various Azure Synapse external tables, Synapse dedicated pool, and SFTP to clients.
- Created and maintained various pipelines for running data flows, notebooks, and various incremental load, update, and pivot processes.
- Developed real-time interactive Power BI dashboards containing various filters, charts, graphs showing the daily transactions, as well as the timeline.
- Worked on conversion of the architecture into Lake House Architecture.

## Technologies Used

### Azure Data Factory

#### Ingestion

For ingestion of the data I used Azure Data Factory which supports a wide range of data types. Here is an example of an Azure Data Flow activity which is used to orchestra data ingestion from an external source into my data lake. Here, I am ingesting data from various external sources both private and public.
![data-flow](https://github.com/debanjansaha-git/dataengineeringarchitecture/blob/main/images/ADF_DataFlow.png)

### Azure Databricks

I use a 2 node spark cluster to read the raw data and perform various data transformations on it.
I have uploaded some of the notebooks which perform these tasks and here is a visualization describing the proces
![data-processinf](https://github.com/debanjansaha-git/dataengineeringarchitecture/blob/main/images/Data%20Processing.png)

### Azure Synapse

### Pipelines

![main-pipeline](https://github.com/debanjansaha-git/dataengineeringarchitecture/blob/main/images/Data%20Pipelines.png)

#### Notification

![run-pipeline](https://github.com/debanjansaha-git/dataengineeringarchitecture/blob/main/images/Run%20Validations.png)

### Power BI

Created a dashboard to display the monthly statistics
![power-bi](https://github.com/debanjansaha-git/dataengineeringarchitecture/blob/main/images/Power%20BI.png)

## Key Achievements

1. Successfully implemented a complete data engineering architecture for processing and storing large volumes of data from over 100 different sources.
2. Designed and led the batch data ingestion process, performing various transformations and validations on the data.
3. Created and maintained various pipelines for running data flows, notebooks, and various incremental load, update, and pivot processes.
4. Developed real-time interactive Power BI dashboards containing various filters, charts, graphs showing the daily transactions, as well as the timeline.

## Future Work

Continue working on conversion of the architecture into Lake House Architecture.

