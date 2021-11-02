# Challenge  - Research Azure Data Analytics

Data shared and aggregated using the FHIR standard offers rich analytics potential.

In this challenge we will utilize FHIR data for analytics. The lesson will be broken into two sections Data Analysis & Statistical Modeling and Data Visualization



## 1. Data Analysis and Statistical Modeling
### Learning Objectives
By the end of the section you will be able to
* Import Anonymized FHIR data into Azure Databricks
* Flatten the data structure to a tabular format
* Produce descriptive statistics on the dataset
* Visualize data elements within the dataset
* Perform an ANOVA test on two data elements

### Prerequisites 
* Deployed Azure API for FHIR
* Azure Databricks
* Completed Challenge - Export and Anonymize Data

### Step 1
Clone this repo 

	https://github.com/microsoft/openhack-mc4h.git

### Step 2
Open  ***Challenge  - Research Azure Data Analytics.py***  in Azure Databricks

The remaining steps in this challenge section will be walked through in the Azure Databricks notebook


 
## 2. Data Visualization and BI
### Learning Objectives
By the end of the section you will be able to 
* Write Anonymized FHIR data to Azure Synapse Analytics
* Create a Power BI dashboard summarizing metrics about the dataset

### Prerequisites 
* Deployed Azure API for FHIR
* Power BI
* Azure Synapse Analytics
* Completed Challenge - Export and Anonymize Data
* Completed section #1 Data Analysis and Statistical Modeling of this challenge

### Step 1

Clone this repo

	https://github.com/microsoft/openhack-mc4h.git


### Step 2

Open your Synapse workspace and import data from the storage account you wrote flattened parquet files to in Section 1: Data Analysis and Statistical Modeling


On the workspace homepage, click import data

![](https://)

Create a one time built in copy task

![](https://)

Define the source as the storage account containing your flattened fhir parquet files. Select the Patients parquet.

![](https://)

Name a table to create as the destination

![](https://)

Double check the column mapping

![](https://)

Create the task and let it run




### Step 3

Create a linked connection for PowerBI

![](https://)

Download the .pbids file from the SQL Analytics database

![](https://)

Grant your user Synapse Linked Data Manager access

![](https://)

Open the file in PowerBI desktop

![](https://)

Use the patient address postal codes to create a map widget

![](https://)

You've created a report for geographic analysis!
	
	
