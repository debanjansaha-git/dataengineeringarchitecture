#   Data Engineering Architecture for Large Scale Data Processing

## Architect: Debanjan Saha


##  Overview
Hi there! I'm Debanjan Saha, and I'm excited to share with you about my experience leading the development and design of a complete data engineering architecture for processing and storing large volumes of data from different sources.
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

For data ingestion, I utilized Azure Data Factory, which supports various data types. Ingestion was orchestrated using an Azure Data Flow activity, which retrieved data from both private and public sources and moved it to my data lake. An example of the Data Flow activity can be seen in the following image:
![data-flow](https://github.com/debanjansaha-git/dataengineeringarchitecture/blob/main/images/ADF_DataFlow.png)

### Azure Databricks

I employed a 2-node spark cluster to process the raw data and perform different transformations. Several notebooks have been uploaded that accomplish these tasks. The following image describes the data processing workflow:
![data-processinf](https://github.com/debanjansaha-git/dataengineeringarchitecture/blob/main/images/Data%20Processing.png)

### Azure Synapse

Azure Synapse combines Spark with Azure Cloud Computing. Synapse is integrated natively with other Azure services such as Azure SQL, Cosmos DB, Azure Data Factory, Azure Databricks, Azure DevOps, among others. The scope of this project focuses on pipeline implementation of data for ride commute data.

### Pipelines

Workloads are broken down into smaller executable units, which are executed using Pipelines. Pipelines execute computations for specific objectives based on the task being performed. Pipelines can be used for tasks like copying data, zipping or unzipping files, running notebooks, running customized scripts, executing stored procedures, adhoc queries, and more. The following image displays the main pipeline used in the project:

![main-pipeline](https://github.com/debanjansaha-git/dataengineeringarchitecture/blob/main/images/Data%20Pipelines.png)

### Transformations

Various actions and transformations are performed on the data. Spark's lazy execution policy is utilized to execute actions when transformations take place. Some pipelines require advanced data transformation techniques. The following image shows an example of a transformation pipeline:
![transform_pipe](https://github.com/debanjansaha-git/dataengineeringarchitecture/blob/main/images/Transformation%20Pipeline.png)

#### Notification

A notification pipeline is attached to every notebook task, which triggers a notification email or SMS depending on the results of the former pipeline activity, which is the execution of a Databricks Notebook.
![run-pipeline](https://github.com/debanjansaha-git/dataengineeringarchitecture/blob/main/images/Run%20Validations.png)

### Power BI

Created a dashboard to display the monthly statistics
![power-bi](https://github.com/debanjansaha-git/dataengineeringarchitecture/blob/main/images/Power%20BI.png)

## Key Achievements

1. Successfully implemented a complete data engineering architecture for processing and storing large volumes of data from different sources and different data types.
2. Designed and led the batch data ingestion process, performing various transformations and validations on the data.
3. Created and maintained various pipelines for running data flows, notebooks, and various incremental load, update, and pivot processes.
4. Developed real-time interactive Power BI dashboards containing various filters, charts, graphs showing the daily transactions, as well as the timeline.

## Future Work

Currently, I'm working on the conversion of the architecture into Lake House Architecture, and I'm excited to see what the future holds in store for this project.

