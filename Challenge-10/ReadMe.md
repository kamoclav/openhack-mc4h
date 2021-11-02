# Challenge  - Research Azure Data Analytics

Data shared and aggregated using the FHIR standard offers rich analytics potential.

In this challenge we will utilize FHIR data for analytics. The lesson will be broken into two sections: Data Analysis & Statistical Modeling, and Data Visualization.



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

The remaining steps in this challenge section will be walked through in the Azure Databricks notebook.


 
## 2. Data Visualization and BI
### Learning Objectives
By the end of the section you will be able to 
* Write Anonymized FHIR data to Azure Synapse Analytics
* Create a Power BI report with a widget summarizing patient geographic data

### Prerequisites 
* Deployed Azure API for FHIR
* Power BI
* Azure Synapse Analytics
* Completed Challenge - Export and Anonymize Data
* Completed section #1 Data Analysis and Statistical Modeling of this challenge

### Step 1: Loading Parquet data into Synapse

#### 1. Open your Synapse workspace and import data from the storage account you wrote flattened parquet files to in Section 1: Data Analysis and Statistical Modeling  <br />


#### 2. On the workspace homepage, click import data  <br />
<br />

![](https://github.com/kamoclav/openhack-mc4h/blob/development/docs/assets/images/Synapse-data-import-1.png) <br />
<br />
#### 3. Create a one time built in copy task <br />
<br />

![](https://github.com/kamoclav/openhack-mc4h/blob/development/docs/assets/images/Synapse-data-import-2.png) <br />
<br />

#### 4. Define the source as the storage account containing your flattened fhir parquet files. Select the Patients parquet. <br />
<br />

![](https://github.com/kamoclav/openhack-mc4h/blob/development/docs/assets/images/Synapse-data-import-3.png) <br />
<br />

#### 5. Name a table to create as the destination <br />
<br />

![](https://github.com/kamoclav/openhack-mc4h/blob/development/docs/assets/images/Synapse-data-import-6.png) <br />
<br />


#### 6. Double check the column mapping <br />
<br />

#### 7. Create the task and let it run <br />
<br />

![](https://github.com/kamoclav/openhack-mc4h/blob/development/docs/assets/images/Synapse-data-import-7.png) <br />
<br />




### Step 2: Connecting PowerBI and Creating a Report

#### 1. Create a linked connection for PowerBI <br />
 <br />

![](https://github.com/kamoclav/openhack-mc4h/blob/development/docs/assets/images/PowerBI-Connect-2.png) <br />
<br />

#### 2. Download the .pbids file from the SQL Analytics database <br />
<br />

![](https://github.com/kamoclav/openhack-mc4h/blob/development/docs/assets/images/PowerBI-Connect-4.png) <br />

#### 3. Grant your user Synapse Linked Data Manager access <br />
<br />

![](https://github.com/kamoclav/openhack-mc4h/blob/development/docs/assets/images/PowerBI-Connect-5.png)<br />
<br />

#### 4. Open the file in PowerBI desktop and use the patient address postal codes to create a map widget<br />
<br />

![](https://github.com/kamoclav/openhack-mc4h/blob/development/docs/assets/images/PowerBI-Connect-6.png)<br />
<br />

You've created a report for geographic analysis!
	
	
