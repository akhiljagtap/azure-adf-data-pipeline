# Azure Cloud Fundamentals and Data Pipeline Implementation using Azure Data Factory

## 📌 Objective

The objective of this project is to understand Azure cloud fundamentals and implement a complete data pipeline using Azure Blob Storage and Azure Data Factory (ADF). The project covers resource provisioning, data storage, pipeline creation, metadata validation, pipeline execution, and access management using Azure IAM.

---

# 🛠️ Technologies Used

- Microsoft Azure
- Azure Resource Group
- Azure Storage Account
- Azure Blob Storage
- Azure Data Factory (ADF)
- Azure IAM (Role-Based Access Control)
- CSV Dataset

---

# 📂 Project Architecture

Blob Storage (CSV File)
↓
Azure Data Factory
↓
Get Metadata
↓
Copy Data
↓
Destination Blob Storage

---

# Assignment Tasks

## Task 1 – Create Resource Group

### Description

Created an Azure Resource Group to organize and manage all Azure resources required for the project.

### Screenshot

![Task 1](screenshots/task-01-resource-group.png)

---

## Task 2 – Storage Setup

### Description

Created an Azure Storage Account, configured a Blob Container, and uploaded the source CSV file.

### Screenshot

![Task 2](screenshots/task-02-blob-container-with-csv.png)

---

## Task 3 – Azure Data Factory Basics

### [a] Linked Service

Configured a Linked Service to establish a secure connection between Azure Data Factory and Azure Blob Storage.

![Linked Service](screenshots/task-03-linked-service.png)

### Dataset

Created source and destination datasets representing the input and output CSV files used by the pipeline.

#### [bI] Input Dataset

![Input Dataset](screenshots/task-03-inputDataset.png)

#### [bII] Output Dataset

![Output Dataset](screenshots/task-03-outputDataset.png)

### [C] Get Metadata

Configured the Get Metadata activity to validate the source file by retrieving metadata such as file existence, file size, and last modified date before processing.

![Get Metadata](screenshots/task-03-get-metadata.png)

---

## Task 4 – Pipeline Development

### Description

Designed an Azure Data Factory pipeline using the Copy Data activity to transfer data from the source Blob Storage to the destination location.

![Pipeline Design](screenshots/task-04-pipeline-design.png)

---

## Task 5 – Pipeline Execution

### Description

Executed the pipeline using Debug and verified that the pipeline completed successfully.

![Pipeline Execution](screenshots/task-05-pipeline-execution-success.png)

---

## Task 6 – IAM Role Assignment

### Description

Assigned Reader and Contributor roles to the Azure Data Factory Managed Identity, allowing secure access to Azure Storage without using storage keys.

![IAM](screenshots/task-06-iam-role-assignment.png)

---

# Mini Project

## Problem Statement

Build a complete Azure Data Factory pipeline that reads a CSV file from Azure Blob Storage, validates its metadata, and copies it to another location.

### [a] Pipeline Execution

Successfully executed the pipeline.

![Pipeline Success](screenshots/mini-project-pipeline-success.png)

### [b] Output File

Verified that the CSV file was successfully copied to the destination.

![Output](screenshots/mini-project-output-file.png)

### [c] Metadata Validation

Validated the source file using the Get Metadata activity before copying.

![Metadata](screenshots/mini-project-metadata-output.png)

---

# Learning Outcomes

Through this project, I learned:

- Azure Resource Group management
- Azure Storage Account and Blob Storage
- Azure Data Factory fundamentals
- Linked Services and Datasets
- Get Metadata activity
- Copy Data activity
- Pipeline development and execution
- Azure IAM role assignment
- End-to-end data pipeline implementation

---

# Author

**Akhil Jagtap**
