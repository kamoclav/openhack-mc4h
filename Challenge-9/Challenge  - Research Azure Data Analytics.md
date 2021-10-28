
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

Use the documentation below to create a notebook in your Azure Synapse Workspace

	https://docs.microsoft.com/en-us/azure/synapse-analytics/spark/apache-spark-development-using-notebooks

In the Data Analysis and Statistical Modeling section you created parquet files for flattened FHIR resources.
To load the flattened files into Azure Synapese, add a cell to the notebook with the following code and replace the location with the location of your parquet files.
	
<pre><code>
%%sql
CREATE TABLE employees USING PARQUET
LOCATION 'parquet files storage location'

</code></pre>

### Step 3

Use the documentation below to create and link a Power BI workspace to Azure Synapse

	https://docs.microsoft.com/en-us/azure/synapse-analytics/get-started-visualize-power-bi
	
	
